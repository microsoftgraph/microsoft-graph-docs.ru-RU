---
title: Отслеживание изменений в данных Microsoft Graph с помощью разностного запроса
description: Delta query enables applications to discover newly created, updated, or deleted entities without performing a full read of the target resource with every request. Microsoft Graph applications can use delta query to efficiently synchronize changes with a local data store.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 7e969858b7537ea36189d24c449803d2a00b125e
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "44990040"
---
# <a name="use-delta-query-to-track-changes-in-microsoft-graph-data"></a>Отслеживание изменений в данных Microsoft Graph с помощью разностного запроса

Delta query enables applications to discover newly created, updated, or deleted entities without performing a full read of the target resource with every request. Microsoft Graph applications can use delta query to efficiently synchronize changes with a local data store.

> [!div class="nextstepaction"]
> [Руководство: использование уведомлений об изменениях и отслеживание изменений с помощью Microsoft Graph](/learn/modules/msgraph-changenotifications-trackchanges)

## <a name="use-delta-query-to-track-changes-in-a-resource-collection"></a>Отслеживание изменений в коллекции ресурсов с помощью запроса изменений

Ниже представлен типичный шаблон вызова.

1. Для начала приложение выполняет запрос GET с функцией delta для нужного ресурса.
2. Microsoft Graph отправит ответ, содержащий нужный ресурс и [маркер состояния](#state-tokens).

     a.  If a `nextLink` URL is returned, there may be additional pages of data to be retrieved in the session. The application continues making requests using the `nextLink` URL to retrieve all pages of data until a `deltaLink` URL is returned in the response.

     b.  If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned. For future requests, the application uses the `deltaLink` URL to learn about changes to the resource.

3. When the application needs to learn about changes to the resource, it makes a new request using the `deltaLink` URL received in step 2. This request *may* be made immediately after completing step 2 or when the application checks for changes.
4. Microsoft Graph возвращает описание изменений ресурса с момента последнего запроса вместе с URL-адресом `nextLink` или `deltaLink`.

>**Примечание.** Ресурсы, хранящиеся в Azure Active Directory (например, пользователи и группы), поддерживают сценарии "синхронизировать с этого момента". Это позволит пропустить действия 1 и 2 (если вы не хотите получать полное состояние ресурса) и запросить последнюю `deltaLink`. Добавьте `$deltaToken=latest` к функции `delta`, и ответ будет содержать ссылку `deltaLink`, но не будет содержать данные ресурсов.

>**Примечание:** Функция запроса изменений обычно упоминается путем добавления `/delta` к имени ресурса. Тем не менее, `/delta` - это сокращение для полного имени`/microsoft.graph.delta`, которое вы видите в запросах, генерируемых Microsoft Graph SDK.

>**Примечание:** Исходный запрос функции Дельта-запроса (без разницы или пропущенного маркера) возвратит ресурсы, которые в данный момент существуют в коллекции. Ресурсы, созданные и удаленные перед первоначальным разностным запросом, не будут возвращены. Обновления, выполненные перед первоначальным запросом, обобщены по отношению к ресурсу, возвращенному в качестве его последнего состояния.

### <a name="state-tokens"></a>Маркеры состояния

A delta query GET response always includes a URL specified in a `nextLink` or `deltaLink` response header.
The `nextLink` URL includes a _skipToken_, and a `deltaLink` URL includes a _deltaToken_.

These tokens are opaque to the client. The following details are what you need to know about them:

- Каждый маркер отражает состояние и представляет моментальный снимок ресурса в этом цикле отслеживания изменений.

- The state tokens also encode and include other query parameters (such as `$select`) specified in the initial delta query request. Therefore, it's not required to repeat them in subsequent delta query requests.

- Совершая запрос изменений, вы можете скопировать и применить URL-адрес `nextLink` или `deltaLink` при следующем вызове функции **delta**, не проверяя содержимое URL-адреса, в том числе маркер состояния.

### <a name="optional-query-parameters"></a>Необязательные параметры запросов

If a client uses a query parameter, it must be specified in the initial request. Microsoft Graph automatically encodes the specified parameter into the `nextLink` or `deltaLink` provided in the response. The calling application only needs to specify the query parameters once upfront. Microsoft Graph adds the specified parameters automatically for all subsequent requests.

Обратите внимание на общую ограниченную поддержку следующих необязательных параметров запроса:

- `$orderby`

    Не считайте, что разностный запрос возвращает определенную последовательность ответов. Предполагайте, что один и тот же элемент может встречаться в любом месте последовательности `nextLink`, и учитывайте это в логике объединения.
- `$top`

    Число объектов на каждой странице зависит от типа ресурса и типа изменений, внесенных в ресурс.

См. сведения о [поддержке параметров разностного запроса](delta-query-messages.md#use-query-parameters-in-a-delta-query-for-messages) для ресурса [message](/graph/api/resources/message?view=graph-rest-1.0).

Для ресурсов [user](/graph/api/resources/user?view=graph-rest-1.0) и [group](/graph/api/resources/group?view=graph-rest-1.0) действуют ограничения на применение некоторых параметров запроса:

- Параметр `$expand` не поддерживается.
- Параметр `$top` не поддерживается.
- Параметр `$orderby` не поддерживается.
- If a `$select` query parameter is used, the parameter indicates that the client prefers to only track changes on the properties or relationships specified in the `$select` statement. If a change occurs to a property that is not selected, the resource for which that property changed does not appear in the delta response after a subsequent request.
- `$select` также поддерживает навигационные свойства `manager` и `members` для пользователей и групп соответственно. Выбор этих свойств позволяет отслеживать изменения руководства и участия в группах для пользователя.

- Фильтры области позволяют отслеживать изменения одного или нескольких конкретных пользователей или групп с помощью идентификатора объекта. Например, следующий запрос возвращает изменения для групп, соответствующих идентификаторам, указанным в фильтре запроса.

<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->
```http
https://graph.microsoft.com/beta/groups/delta/?$filter=id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ae5f' or id eq '004d6a07-fe70-4b92-add5-e6e37b8acd8e'
```

## <a name="resource-representation-in-the-delta-query-response"></a>Представление ресурсов в отклике на разностный запрос

- Новые экземпляры поддерживаемого ресурса представлены в ответе на запрос изменений с помощью стандартных свойств.

- Обновленные экземпляры представлены **id** и *по крайней мере* обновленными свойствами, но могут быть включены и другие свойства.

- Relationships on users and groups are represented as annotations on the standard resource representation. These annotations use the format `propertyName@delta`. The annotations are included in the response of the initial delta query request.

Удаленные экземпляры представлены только свойством **id** и объектом `@removed`. Объект `@removed` может содержать дополнительные сведения о том, почему удален экземпляр. Например, "@removed": {"reason": "changed"}.

Возможные причины @removed: *changed* или *deleted*.

- *changed* указывает, что элемент удален и может быть восстановлен из [deletedItems](/graph/api/resources/directory).

- *deleted* указывает, что элемент удален и не может быть восстановлен.

The `@removed` object can be returned in the initial delta query response and in tracked (deltaLink) responses. Clients using delta query requests should be designed to handle these objects in the responses.

>**Примечание:** Возможно, что одна сущность будет содержаться в ответе несколько раз, если эта сущность менялась несколько раз и при определенных условиях. Запрос изменений позволяют вашему приложению перечислять все изменения, но не могут гарантировать, что объекты объединены в одном ответе.

## <a name="supported-resources"></a>Поддерживаемые ресурсы

Разностные запросы поддерживаются для указанных ниже ресурсов.

| **Коллекция ресурсов**                                        | **API**                                                                                                                                                                                          |
|:---------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Приложения                                                   | Функция [delta](/graph/api/application-delta) ресурса [application](/graph/api/resources/application)                                                                                   |
| Административные единицы (предварительная версия)                                 | Функция [delta](/graph/api/administrativeunit-delta) ресурса [administrativeUnit](/graph/api/resources/administrativeunit) (предварительная версия)                                                    |
| Сообщения чата в канале (предварительная версия)                           | Функция [delta](/graph/api/chatmessage-delta) [chatMessage](/graph/api/resources/chatmessage)                                                                                            |
| Классы (предварительная версия)                                              | Функция [delta](/graph/api/educationclass-delta) ресурса [educationClass](/graph/api/resources/educationclass) (предварительная версия)                                                                |
| Объекты каталога (предварительная версия)                                    | Функция [delta](/graph/api/directoryobject-delta) ресурса [directoryObject](/graph/api/resources/directoryobject) (предварительная версия)                                                             |
| Перечисление ролей каталога                                                | Функция [delta](/graph/api/directoryrole-delta?view=graph-rest-1.0) ресурса [directoryObjects](/graph/api/resources/directoryrole?view=graph-rest-1.0)                                     |
| Элементы на диске\*                                                  | Функция [delta](/graph/api/driveitem-delta?view=graph-rest-1.0) ресурса [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0)                                                 |
| Пользователи образовательных учреждений (предварительная версия)                                      | Функция [delta](/graph/api/educationuser-delta) ресурса [educationUser](/graph/api/resources/educationuser) (предварительная версия)                                                                   |
| События в представлении (диапазоне дат) основного календаря | Функция [delta](/graph/api/event-delta?view=graph-rest-1.0) ресурса [event](/graph/api/resources/event?view=graph-rest-1.0)                                                             |
| Группы                                                         | Функция [delta](/graph/api/group-delta?view=graph-rest-1.0) ресурса [group](/graph/api/resources/group?view=graph-rest-1.0)                                                             |
| Папки почты                                                   | Функция [delta](/graph/api/mailfolder-delta?view=graph-rest-1.0) ресурса [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0)                                              |
| Сообщения в папке                                           | Функция [delta](/graph/api/message-delta?view=graph-rest-1.0) ресурса [message](/graph/api/resources/message?view=graph-rest-1.0)                                                       |
| Контакты организации                                        | функция[delta](/graph/api/orgcontact-delta?view=graph-rest-1.0) ресурса [orgContact](/graph/api/resources/orgcontact?view=graph-rest-1.0)                                              |
| OAuth2PermissionGrants (предварительная версия)                               | Функция [delta](/graph/api/oauth2permissiongrant-delta?view=graph-rest-beta) ресурса [oauth2permissiongrant](/graph/api/resources/oauth2permissiongrant?view=graph-rest-beta) (предварительная версия) |
| Папки личных контактов                                       | Функция [delta](/graph/api/contactfolder-delta?view=graph-rest-1.0) ресурса [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0)                                     |
| Личные контакты в папке                                  | Функция [delta](/graph/api/contact-delta?view=graph-rest-1.0) ресурса [contact](/graph/api/resources/contact?view=graph-rest-1.0)                                                       |
| Элементы Planner\*\* (предварительная версия)                                    | Функция [delta](/graph/api/planneruser-list-delta) всего сегмента ресурса [plannerUser](/graph/api/resources/planneruser) (предварительный просмотр)                                                     |
| Учебные заведения (предварительная версия)                                              | Функция [delta](/graph/api/educationschool-delta) ресурса [educationSchool](/graph/api/resources/educationschool) (предварительная версия)                                                             |
| Субъекты-службы (предварительная версия)                                   | Функция [delta](/graph/api/serviceprincipal-delta) ресурса [servicePrincipal](/graph/api/resources/serviceprincipal) (предварительная версия)                                                          |
| Users                                                          | Функция [delta](/graph/api/user-delta?view=graph-rest-1.0) ресурса [user](/graph/api/resources/user?view=graph-rest-1.0)                                                                |


> \* Небольшие различия в использовании ресурсов OneDrive и других поддерживаемых ресурсов касаются синтаксиса. Разностный запрос для ресурсов drive будет обновлен в соответствии с запросами для других типов ресурсов.  Дополнительные сведения о текущем синтаксисе см. в статье [Отслеживание изменений для drive](/graph/api/driveitem-delta?view=graph-rest-1.0).

> \*\* Шаблон использования ресурсов Planner незначительно отличается от шаблонов использования других поддерживаемых ресурсов.  Дополнительные сведения см. в [этой статье](/graph/api/planneruser-list-delta).

## <a name="limitations"></a>Ограничения

### <a name="properties-stored-outside-of-the-main-data-store"></a>Свойства, хранящиеся вне основного хранилища данных

Некоторые ресурсы содержат свойства, которые хранятся вне основного хранилища данных для ресурса (например, ресурс user в основном хранится в системе Azure AD, в то время как некоторые свойства, такие как **skills**, хранятся в SharePoint Online). В настоящее время эти свойства не поддерживаются как часть отслеживания изменений; изменение одного из этих свойств не приведет к отображению объекта в отклике на разностный запрос. В настоящее время только свойства, хранящиеся в главном хранилище данных, активируют изменения в разностном запросе.

Чтобы проверить, можно ли использовать свойство в разностном запросе, попробуйте выполнить обычную операцию `GET` в коллекции ресурсов и выберите интересующее вас свойство. Например, вы можете попробовать использовать свойство **skills** в коллекции пользователей.

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/?$select=skills
```

Так как свойство **skills** хранится вне Azure AD, отклик будет следующим.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 501 Not Implemented
Content-type: application/json

{
    "error": {
        "code": "NotImplemented",
        "message": "This operation target is not yet supported.",
        "innerError": {
            "request-id": "...",
            "date": "2019-09-20T21:47:50"
        }
    }
}
```

Это говорит о том, что свойство **skills** не поддерживается для разностного запроса в ресурсе **user**.

### <a name="navigation-properties"></a>Свойства навигации

Свойства навигации не поддерживаются. Например, вы не можете отслеживать изменения в коллекции пользователей, включающие изменения их свойства **photo**; **photo** — это свойство навигации, которое хранится вне сущности пользователя, и внесенные в него изменения не приводят к включению объекта "пользователь" в отклик с различиями.

### <a name="processing-delays"></a>Задержка обработки

Ожидайте различные задержки между моментом, когда изменения вносятся в экземпляр ресурса, который может быть через интерфейс приложения или API, и временем, когда отслеживаемое изменение отражается в ответе запроса изменений.

### <a name="national-clouds"></a>Национальные облачные развертывания

Запросы изменений доступны для клиентов, размещенных в общедоступном облаке и Microsoft Graph China, управляемых только 21Vianet.

### <a name="token-duration"></a>Длительность маркера

Токены изменений действительны только в течение определенного периода, прежде чем клиентскому приложению потребуется снова выполнить полную синхронизацию. Для объектов Directory (**Application**, **administrativeUnit**, **directoryObject**, **directoryRole**, **Group**, **orgContact**, **oauth2permissiongrant**, **servicePrincipal**и **User**) максимальное значение составляет 7 дней. Для объектов образования (**educationSchool**, **educationUser**и **educationClass**) лимит составляет 7 дней.

## <a name="prerequisites"></a>Необходимые компоненты

Выполнение разностных запросов для определенного ресурса требует тех же [разрешений](./permissions-reference.md), что и его чтение.

## <a name="delta-query-request-examples"></a>Примеры разностных запросов

- [Получение добавочных изменений для событий в представлении календаря](delta-query-events.md)
- [Получение добавочных изменений сообщений в папке](./delta-query-messages.md)
- [Получение добавочных изменений групп](./delta-query-groups.md)
- [Получение добавочных изменений пользователей](./delta-query-users.md)
