---
title: Отслеживание изменений в данных Microsoft Graph с помощью разностного запроса
description: Запросы изменений позволяют приложениям обнаруживать новые, обновленные и удаленные сущности, не считывая целевой ресурс полностью при каждом запросе. Приложения Microsoft Graph могут использовать запросы изменений, чтобы эффективно синхронизировать изменения с локальным хранилищем данных.
author: davidmu1
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 2a684d593458b2f40a6b45f7c326f45f37e1cc4a
ms.sourcegitcommit: adc36691fd77544eeb1ec061ccfa59abffbfea9a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/31/2020
ms.locfileid: "48819669"
---
# <a name="use-delta-query-to-track-changes-in-microsoft-graph-data"></a>Отслеживание изменений в данных Microsoft Graph с помощью разностного запроса

Запросы изменений позволяют приложениям обнаруживать новые, обновленные и удаленные сущности, не считывая целевой ресурс полностью при каждом запросе. Приложения Microsoft Graph могут использовать запросы изменений, чтобы эффективно синхронизировать изменения с локальным хранилищем данных.

> [!div class="nextstepaction"]
> [Руководство. Использование уведомлений об изменениях и функции отслеживания изменений в Microsoft Graph](/learn/modules/msgraph-changenotifications-trackchanges)

## <a name="use-delta-query-to-track-changes-in-a-resource-collection"></a>Отслеживание изменений в коллекции ресурсов с помощью запроса изменений

Ниже представлен типичный шаблон вызова.

1. Для начала приложение выполняет запрос GET с функцией delta для нужного ресурса.
2. Microsoft Graph отправит ответ, содержащий нужный ресурс и [маркер состояния](#state-tokens).

     -  Если возвращается URL-адрес `nextLink`, это означает, что во время сеанса могли быть получены не все страницы данных. Для получения всех страниц данных приложение продолжает отправлять запросы, используя URL-адрес `nextLink`, пока в отклик не будет включен URL-адрес `deltaLink`.

     - Если возвращается URL-адрес `deltaLink`, это означает, что больше нет данных о текущем состоянии ресурса. В последующих запросах приложение использует URL-адрес `deltaLink`, чтобы узнавать об изменениях ресурса.

3. Когда приложению требуется узнать об изменениях ресурса, оно совершает новый запрос, используя URL-адрес `deltaLink`, полученный на шаге 2. Этот запрос *может* быть совершен сразу по завершении шага 2 или когда приложение проверяет наличие изменений.
4. Microsoft Graph возвращает описание изменений ресурса с момента последнего запроса вместе с URL-адресом `nextLink` или `deltaLink`.

>**Примечание.** Ресурсы, хранящиеся в Azure Active Directory (например, пользователи и группы), поддерживают сценарии "синхронизировать с этого момента". Это позволит пропустить действия 1 и 2 (если вы не хотите получать полное состояние ресурса) и запросить последнюю `deltaLink`. Добавьте `$deltaToken=latest` к функции `delta`, и ответ будет содержать ссылку `deltaLink`, но не будет содержать данные ресурсов. Ресурсы в OneDrive и SharePoint также поддерживают эту функцию. Для ресурсов в OneDrive и SharePoint вместо этого добавьте `token=latest`.

>**Примечание:** Функция запроса изменений обычно упоминается путем добавления `/delta` к имени ресурса. Тем не менее, `/delta` - это сокращение для полного имени`/microsoft.graph.delta`, которое вы видите в запросах, генерируемых Microsoft Graph SDK.

>**Примечание.** Исходный запрос к функции разностного запроса (без разностного маркера или с игнорируемым маркером) возвращает ресурсы, которые в настоящее время существуют в коллекции. Ресурсы, созданные и удаленные до исходного разностного запроса, не возвращаются. Обновления, внесенные до исходного запроса, обобщаются в возвращаемом ресурсе в их последнем состоянии. 

### <a name="state-tokens"></a>Маркеры состояния

Ответ GET на запрос изменений всегда включает URL-адрес, указанный в заголовке `nextLink` или `deltaLink`. URL-адрес `nextLink` включает маркер _skipToken_ , а URL-адрес `deltaLink` — _deltaToken_ .

Эти маркеры непрозрачны для клиента. Вот что вам нужно знать о них:

- Каждый маркер отражает состояние и представляет моментальный снимок ресурса в этом цикле отслеживания изменений.

- Маркеры состояния также кодируют и включают другие параметры запроса (такие как `$select`), указанные в исходном запросе изменений. Таким образом, не обязательно повторять их в последующих запросах изменений.

- Совершая запрос изменений, вы можете скопировать и применить URL-адрес `nextLink` или `deltaLink` при следующем вызове функции **delta** , не проверяя содержимое URL-адреса, в том числе маркер состояния.

### <a name="optional-query-parameters"></a>Необязательные параметры запросов

Если клиент использует параметр запроса, он должен быть указан в исходном запросе. Microsoft Graph автоматически кодирует указанный параметр в ссылке `nextLink` или `deltaLink`, указанной в ответе. Вызывающему приложению достаточно один раз указать параметры запроса. Microsoft Graph автоматически добавляет указанные параметры для всех последующих запросов.

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
- Если используется параметр запроса `$select`, это означает, что клиент предпочитает отслеживать изменения только для тех свойств или связей, которые указаны в операторе `$select`. При изменении свойства, которое не было выбрано, соответствующий ресурс не появится в отклике с различиями при последующем запросе.
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

- Связи между пользователями и группами представлены в виде заметок к стандартному представлению ресурса. Эти заметки представлены в формате `propertyName@delta`. Они включаются в отклик на исходный разностный запрос.

Удаленные экземпляры представлены только свойством **id** и объектом `@removed`. Объект `@removed` может содержать дополнительные сведения о том, почему удален экземпляр. Например, "@removed": {"reason": "changed"}.

Возможные причины @removed: *changed* или *deleted* .

- *changed* указывает, что элемент удален и может быть восстановлен из [deletedItems](/graph/api/resources/directory).

- *deleted* указывает, что элемент удален и не может быть восстановлен.

Объект `@removed` может возвращаться в отклике на исходный разностный запрос и в отслеживаемых откликах (deltaLink). Клиенты, использующие разностные запросы, должны иметь возможность обрабатывать эти объекты в откликах.

>**Примечание:** Возможно, что одна сущность будет содержаться в ответе несколько раз, если эта сущность менялась несколько раз и при определенных условиях. Запрос изменений позволяют вашему приложению перечислять все изменения, но не могут гарантировать, что объекты объединены в одном ответе.

## <a name="supported-resources"></a>Поддерживаемые ресурсы

Разностные запросы поддерживаются для указанных ниже ресурсов. Обратите внимание, что у некоторых ресурсов, доступных в версии 1.0, соответствующие функции **delta** по-прежнему находятся в предварительном состоянии (как указано).

| **Коллекция ресурсов**                                        | **API**                                                                                                                                                                                          |
|:---------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Приложения                                                   | Функция [delta](/graph/api/application-delta) ресурса [application](/graph/api/resources/application)                                                                                   |
| Административные единицы (предварительная версия)                         | Функция [delta](/graph/api/administrativeunit-delta) (предварительная версия) ресурса [administrativeUnit](/graph/api/resources/administrativeunit)                                                    |
| Сообщения чата в канале                            | Функция [delta](/graph/api/chatmessage-delta) (предварительная версия) ресурса [chatMessage](/graph/api/resources/chatmessage)                                                                                            |
| Классы                                               | Функция [delta](/graph/api/educationclass-delta) (предварительная версия) ресурса [educationClass](/graph/api/resources/educationclass)                                                                 |
| Объекты каталога                                     | Функция [delta](/graph/api/directoryobject-delta) (предварительная версия) ресурса [directoryObject](/graph/api/resources/directoryobject)                                                              |
| Перечисление ролей каталога                                                | Функция [delta](/graph/api/directoryrole-delta?view=graph-rest-1.0) ресурса [directoryObjects](/graph/api/resources/directoryrole?view=graph-rest-1.0)                                     |
| Элементы на диске\*                                                  | Функция [delta](/graph/api/driveitem-delta?view=graph-rest-1.0) ресурса [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0)                                                 |
| Пользователи образовательных учреждений                                       | Функция [delta](/graph/api/educationuser-delta) (предварительная версия) ресурса [educationUser](/graph/api/resources/educationuser)                                                                    |
| События в представлении (диапазоне дат) основного календаря | Функция [delta](/graph/api/event-delta?view=graph-rest-1.0) ресурса [event](/graph/api/resources/event?view=graph-rest-1.0)                                                             |
| Группы                                                         | Функция [delta](/graph/api/group-delta?view=graph-rest-1.0) ресурса [group](/graph/api/resources/group?view=graph-rest-1.0)                                                             |
| Папки почты                                                   | Функция [delta](/graph/api/mailfolder-delta?view=graph-rest-1.0) ресурса [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0)                                              |
| Сообщения в папке                                           | Функция [delta](/graph/api/message-delta?view=graph-rest-1.0) ресурса [message](/graph/api/resources/message?view=graph-rest-1.0)                                                       |
| Контакты организации                                        | функция[delta](/graph/api/orgcontact-delta?view=graph-rest-1.0) ресурса [orgContact](/graph/api/resources/orgcontact?view=graph-rest-1.0)                                              |
| OAuth2PermissionGrants                               | Функция [delta](/graph/api/oauth2permissiongrant-delta) ресурса [oauth2permissiongrant](/graph/api/resources/oauth2permissiongrant) |
| Папки личных контактов                                       | Функция [delta](/graph/api/contactfolder-delta?view=graph-rest-1.0) ресурса [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0)                                     |
| Личные контакты в папке                                  | Функция [delta](/graph/api/contact-delta?view=graph-rest-1.0) ресурса [contact](/graph/api/resources/contact?view=graph-rest-1.0)                                                       |
| Элементы Planner\*\* (предварительная версия)                                    | Функция [delta](/graph/api/planneruser-list-delta) (предварительная версия) всего сегмента ресурса [plannerUser](/graph/api/resources/planneruser)                                                      |
| Учебные заведения                                               | Функция [delta](/graph/api/educationschool-delta) (предварительная версия) ресурса [educationSchool](/graph/api/resources/educationschool)                                                              |
| Субъекты-службы                                   | Функция [delta](/graph/api/serviceprincipal-delta) ресурса [servicePrincipal](/graph/api/resources/serviceprincipal)                                                          |
| Задачи в списке задач                                           | Функция [delta](/graph/api/todotask-delta) ресурса [todoTask](/graph/api/resources/todotask)                                                         |
| Списки задач                                                     | Функция [delta](/graph/api/todotasklist-delta) ресурса [todoTaskList](/graph/api/resources/todotasklist)                                                         |
| Пользователи                                                          | Функция [delta](/graph/api/user-delta?view=graph-rest-1.0) ресурса [user](/graph/api/resources/user?view=graph-rest-1.0)                                                                |


> \* Небольшие различия в использовании ресурсов OneDrive и других поддерживаемых ресурсов касаются синтаксиса. Разностный запрос для ресурсов drive будет обновлен в соответствии с запросами для других типов ресурсов.  Дополнительные сведения о текущем синтаксисе см. в статье [Отслеживание изменений для drive](/graph/api/driveitem-delta?view=graph-rest-1.0).

> \*\* Шаблон использования ресурсов Planner незначительно отличается от шаблонов использования других поддерживаемых ресурсов.  Дополнительные сведения см. в [этой статье](/graph/api/planneruser-list-delta).

## <a name="limitations"></a>Ограничения

### <a name="properties-stored-outside-of-the-main-data-store"></a>Свойства, хранящиеся вне основного хранилища данных

Некоторые ресурсы содержат свойства, которые хранятся вне основного хранилища данных для ресурса (например, ресурс user в основном хранится в системе Azure AD, в то время как некоторые свойства, такие как **skills** , хранятся в SharePoint Online). В настоящее время эти свойства не поддерживаются как часть отслеживания изменений; изменение одного из этих свойств не приведет к отображению объекта в отклике на разностный запрос. В настоящее время только свойства, хранящиеся в главном хранилище данных, активируют изменения в разностном запросе.

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

Это говорит о том, что свойство **skills** не поддерживается для разностного запроса в ресурсе **user** .

### <a name="navigation-properties"></a>Свойства навигации

Свойства навигации не поддерживаются. Например, вы не можете отслеживать изменения в коллекции пользователей, включающие изменения их свойства **photo** ; **photo** — это свойство навигации, которое хранится вне сущности пользователя, и внесенные в него изменения не приводят к включению объекта "пользователь" в отклик с различиями.

### <a name="processing-delays"></a>Задержка обработки

Ожидайте различные задержки между моментом, когда изменения вносятся в экземпляр ресурса, который может быть через интерфейс приложения или API, и временем, когда отслеживаемое изменение отражается в ответе запроса изменений.

### <a name="national-clouds"></a>Национальные облачные развертывания

Запросы изменений доступны для клиентов, размещенных в общедоступном облаке и Microsoft Graph China, управляемых только 21Vianet.

### <a name="replays"></a>Повторения

Ваше приложение должно быть готово к повторениям, которые происходят, когда одинаковое изменение возникает в последующих откликах. Хотя разностный запрос является оптимальным средством сокращения повторений, они по-прежнему возможны.

### <a name="synchronization-reset"></a>Сброс синхронизации

Разностный запрос может возвращать код отклика `410 (gone)` и заголовок **Location** , содержащий URL-адрес запроса с пустым разностным маркером (аналогично исходному запросу). Это означает, что приложение требуется перезапустить с полной синхронизацией целевого клиента. Обычно это происходит, чтобы предотвратить несоответствие данных из-за внутреннего обслуживания или миграции целевого клиента.

### <a name="token-duration"></a>Длительность маркера

Токены изменений действительны только в течение определенного периода, прежде чем клиентскому приложению потребуется снова выполнить полную синхронизацию. Для объектов каталога ( **application** , **administrativeUnit** , **directoryObject** , **directoryRole** , **group** , **orgContact** , **oauth2permissiongrant** , **servicePrincipal** и **user** ) ограничение составляет 7 дней. Для образовательных объектов ( **educationSchool** , **educationUser** и **educationClass** ) ограничение составляет 7 дней. Для объектов Outlook ( **message** , **mailFolder** , **event** , **contact** , **contactFolder** , **todoTask** и **todoTaskList** ) верхнее ограничение не фиксировано; оно зависит от размера внутреннего кэша разностного маркера. Хотя новые разностные маркеры непрерывно добавляются в кэш, после превышения емкости кэша старые разностные маркеры удаляются.

## <a name="prerequisites"></a>Предварительные требования

Выполнение разностных запросов для определенного ресурса требует тех же [разрешений](./permissions-reference.md), что и его чтение.

## <a name="delta-query-request-examples"></a>Примеры разностных запросов

- [Получение добавочных изменений для событий в представлении календаря](delta-query-events.md)
- [Получение добавочных изменений сообщений в папке](./delta-query-messages.md)
- [Получение добавочных изменений групп](./delta-query-groups.md)
- [Получение добавочных изменений пользователей](./delta-query-users.md)
