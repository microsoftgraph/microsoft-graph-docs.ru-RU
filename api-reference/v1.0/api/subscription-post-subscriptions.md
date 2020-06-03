---
title: Создание подписки
description: Подписывает приложение прослушивателя на получение уведомлений об изменениях при изменении данных в Microsoft Graph.
localization_priority: Priority
author: baywet
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 28053ccd79b8cbab521f3cbd702dd46835d14ecb
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491835"
---
# <a name="create-subscription"></a>Создание подписки

Пространство имен: microsoft.graph

Подписывает приложение прослушивателя на получение уведомлений об изменениях, когда запрошенный тип изменений выполняется для указанного ресурса в Microsoft Graph.

## <a name="permissions"></a>Разрешения

 Создание подписки требует наличия области чтения для ресурса. Например, чтобы получать уведомления об изменениях для сообщений, ваше приложение должно иметь `Mail.Read` разрешение. 
 
 В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Поддерживаемый ресурс | Делегированное (рабочая или учебная учетная запись) | Делегированное (личная учетная запись Майкрософт) | Для приложений |
|:-----|:-----|:-----|:-----|
|[каллрекорд](../resources/callrecords-callrecord.md) (/коммуникатионс/каллрекордс) | Не поддерживается | Не поддерживается | CallRecords.Read.All  |
|[contact](../resources/contact.md) | Contacts.Read | Contacts.Read | Contacts.Read |
|[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя) | Не поддерживается | Files.ReadWrite | Не поддерживается |
|[driveItem](../resources/driveitem.md) (OneDrive для бизнеса) | Files.ReadWrite.All | Не поддерживается | Files.ReadWrite.All |
|[event](../resources/event.md) | Calendars.Read | Calendars.Read | Calendars.Read |
|[group](../resources/group.md) | Group.Read.All | Не поддерживается | Group.Read.All |
|[group conversation](../resources/conversation.md) | Group.Read.All | Не поддерживается | Не поддерживается |
|[list](../resources/list.md) | Sites.ReadWrite.All | Не поддерживается | Sites.ReadWrite.All |
|[message](../resources/message.md) | Mail.ReadBasic, Mail.Read | Mail.ReadBasic, Mail.Read | Mail.ReadBasic, Mail.Read |
|[security alert](../resources/alert.md) | SecurityEvents.ReadWrite.All | Не поддерживается | SecurityEvents.ReadWrite.All |
|[user](../resources/user.md) | User.Read.All | User.Read.All | User.Read.All |

> **Примечание.** Существуют дополнительные ограничения для подписок на элементы OneDrive и Outlook. Ограничения применяются для создания, а также управления подписками (получение, обновление и удаление подписок).

- В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище. В OneDrive для бизнеса можно подписаться только на корневую папку. Уведомления об изменениях отправляются для запрошенных типов изменений в подписанной папке, а также любых файлов, папок или других экземпляров **driveItem** в иерархии. Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.

- В Outlook делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, вошедшего в систему. Это означает, например, что нельзя использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.
- Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:

  - Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.
  - Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках. 


## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `201 Created` и объект [subscription](../resources/subscription.md) в теле отклика.
Сведения о том, как возвращаются ошибки, приведены в разделе [ошибочные ответы][error-response].

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

Ниже приведен пример запроса на отправку уведомления об изменении при получении пользователем новой почты.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-type: application/json

{
   "changeType": "updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue",
   "latestSupportedTlsVersion": "v1_2"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.
Поля `clientState` и `latestSupportedTlsVersion` необязательны.

##### <a name="resources-examples"></a>Примеры ресурсов

Ниже приведены допустимые значения свойства ресурса для подписки.

| Тип ресурса | Примеры |
|:------ |:----- |
|Mail|me/mailfolders('inbox')/messages<br />me/messages|
|Contacts|me/contacts|
|Calendars|me/events|
|Users|users|
|Groups|groups|
|Conversations|groups('*{id}*')/conversations|
|Drives|me/drive/root|
|Список|sites/{site-id}/lists/{list-id}|
|Оповещение безопасности|security/alerts?$filter=status eq 'New'|
|Записи звонков|связь/Каллрекордс|

##### <a name="response"></a>Отклик

Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 252

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscriptions/$entity",
  "id": "7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource": "me/mailFolders('Inbox')/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType": "updated",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2"
}
```

## <a name="notification-endpoint-validation"></a>Проверка конечной точки уведомлений

Конечная точка уведомления подписки (указанная в свойстве `notificationUrl`) должна поддерживать ответ на запрос проверки, как описано в статье [Настройка уведомлений об изменениях в пользовательских данных](/graph/webhooks#notification-endpoint-validation). Если проверка завершилась сбоем, запрос на создание подписки возвращает ошибку 400 (неверный запрос).

[error-response]: /graph/errors

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
