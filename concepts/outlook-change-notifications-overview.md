---
title: Уведомления об изменениях, связанных с ресурсами Outlook, в Microsoft Graph
description: Узнайте, как получать уведомления об изменениях (создание, обновление и удаление) ресурсов в Outlook с помощью API Microsoft Graph
author: abheek-das
ms.localizationpriority: high
ms.prod: outlook
ms.custom: scenarios:getting-started
ms.openlocfilehash: 04361ff86fc4106d0792b43b2ea7638a41e04b7c
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337924"
---
# <a name="change-notifications-for-outlook-resources-in-microsoft-graph"></a>Уведомления об изменениях, связанных с ресурсами Outlook, в Microsoft Graph

API Microsoft Graph позволяет подписаться на изменения в ресурсе, включая создание, обновление или удаление ресурса, и получать уведомления через веб-перехватчики. [Подписка](/graph/api/resources/webhooks) указывает нужные типы изменений для отслеживания для определенного ресурса и URL-адрес конечной точки для получения уведомлений об этих изменениях. Настройка подписки снижает накладные расходы, поскольку в противном случае приходится запрашивать и сравнивать ресурсы для получения каких-либо изменений. При желании можно указать в запросе на подписку шифрование и включить в уведомление измененные данные ресурса, сохранив отдельный последующий вызов API для получения полезных данных ресурса.

Существует максимальное ограничение в 1000 активных подписок на ресурсы Outlook на почтовый ящик для всех приложений. Вы можете подписаться на изменения контактов, событий или сообщений в почтовом ящике.

## <a name="subscribe-to-changes-in-contacts-calendar-or-mail"></a>Подписка на изменения контактов, календаря или почты

Чтобы подписаться на уведомления об изменении ресурсов Outlook, сначала создайте [подписку](/graph/api/resources/subscription).

Следующие ресурсы Outlook поддерживают подписки с данными ресурсов или без них в полезных данных [уведомлений об изменениях](/graph/api/resources/changenotification).

- [contact](/graph/api/resources/contact)
- [event](/graph/api/resources/event)
- [message](/graph/api/resources/message)

## <a name="create-a-subscription"></a>Создание подписки

Чтобы [создать подписку](webhooks.md#creating-a-subscription), укажите ресурс Outlook и тип изменений (создание, обновление или удаление), для которых вы хотите получать уведомления. См. [пример](#example-1-create-a-subscription-to-get-change-notifications-without-resource-data-when-the-user-receives-a-new-message).

### <a name="request-permissions"></a>Запрос разрешений

[!INCLUDE [outlook-subscription-notes](../includes/outlook-subscription-notes.md)]

В зависимости от ресурса разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.

| Ресурс| Поддерживаемые пути ресурсов| Делегированные (рабочая или учебная учетная запись)| Делегированное (личная учетная запись Майкрософт)| Для приложений|
|:--------|:------------------------|:----------------------------------|:--------------------------------------|:-----------|
|[contact](/graph/api/resources/contact) | Изменения всех личных контактов в почтовом ящике пользователя: <br>`/me/contacts`<br>`/users/{id}/contacts`<br>Изменения контактов в contactFolder пользователя:<br>`/users/{id}/contactFolders/{id}/contacts` | Contacts.Read | Contacts.Read | Contacts.Read |
|[event](/graph/api/resources/event)     | Изменения всех событий в почтовом ящике пользователя: <br>`/me/events`<br>`/users/{id}/events` | Calendars.Read | Calendars.Read | Calendars.Read |
|[message](/graph/api/resources/message) | Изменения во всех сообщениях в почтовом ящике пользователя: <br>`/me/messages`<br>`/users/{id}/messages`<br>Изменения в сообщениях в mailFolder пользователя:<br>`/users/{id}/mailFolders/{id}/messages` | Mail.ReadBasic, Mail.Read | Mail.ReadBasic, Mail.Read | Mail.ReadBasic, Mail.Read |

### <a name="include-resource-data-in-notification-payload-preview"></a>Включить данные ресурсов в полезных данных уведомлений (предварительная версия)

> [!NOTE]
> Уведомления с данными ресурсов для ресурсов Outlook в настоящее время доступны только в конечной точке бета-версии Microsoft Graph. 

Чтобы включить данные ресурсов в уведомления об изменениях, **требуется** указать следующие свойства в дополнение к тем, которые обычно включаются при [создании подписки](webhooks.md#creating-a-subscription):

- **includeResourceData**. Установите для этого свойства значение `true` для явного запроса данных ресурсов.
- **resource**. Это свойство указывает URL-адрес ресурса. Обязательно используйте параметр запроса `$select`, чтобы явно указать свойства ресурса Outlook, которые необходимо включить в полезные данные уведомления.
  > **Примечание:** Не включайте в URL-адрес свойства `$top`, `$skip`, `$orderby`, `$select=Body,UniqueBody`, а также `$expand`, кроме **singleValueExtendedProperties** или **multiValueExtendedProperties**.
- **encryptionCertificate**. Это свойство содержит только открытый ключ, используемый Microsoft Graph для шифрования данных ресурса. Сохраняйте соответствующий закрытый ключ для [расшифровки контента](webhooks-with-resource-data.md#decrypting-resource-data-from-change-notifications).
- **encryptionCertificateId**. Это свойство является вашим собственным идентификатором для сертификата. Используйте этот идентификатор для определения в каждом уведомлении об изменениях сертификата, используемого для расшифровки.

См. [пример](#example-2-create-a-subscription-to-get-change-notifications-with-resource-data-when-the-user-receives-a-new-message-preview) подписки на уведомления об изменениях с данными ресурса для ресурса **message**.


### <a name="refine-the-conditions-for-a-notification"></a>Уточнение условий для уведомления
Вы можете дополнительно уточнить условия для уведомления, используя `$filter` параметр запроса. См. [пример](#example-3-create-a-subscription-to-get-change-notifications-with-resource-data-for-a-message-based-on-a-condition-preview).

Одним из распространенных применений `$filter` является получение уведомлений об изменении определенного свойства ресурса. Например, можно использовать `$filter` для подписки на непрочитанные сообщения в папке (свойство **isRead** — `false`) и включить все типы изменений:
- Сообщение, добавленное или помеченное непрочитанным в папке, вызовет `Created` уведомление.
- Чтение сообщения или его маркировка, считанное в папке, вызовет `Deleted` уведомление.
- Изменение любого свойства, кроме **isRead**, ресурса **message** в папке вызовет уведомление `Updated`.

Если при создании подписки не используется `$filter`:
- Добавление сообщения в папку приведет к `Created` уведомлению.
- Чтение сообщения в папке, маркировка сообщения как прочитанного или изменение любого другого свойства сообщения в этой папке приведет к `Updated` уведомлению.
- Удаление сообщения приведет к `Delete` уведомлению.

### <a name="subscribe-to-lifecycle-notifications"></a>Подписка на уведомления жизненного цикла
Ресурсы Outlook **contact**, **event** и **message** также поддерживают подписку на уведомления жизненного цикла. Уведомления жизненного цикла необходимы в том случае, если ваше приложение удалит подписки или пропустит некоторые уведомления об изменениях. В приложениях должна быть реализована логика определения потерь и восстановления после них, а также возобновления непрерывного потока уведомлений об изменениях. Дополнительные сведения см. в разделе [Подписка на уведомления жизненного цикла](webhooks-lifecycle.md).

### <a name="keep-track-of-subscription-lifetime"></a>Отслеживание срока действия подписки
Не забудьте [продлить](/graph/api/subscription-update) подписку до истечения ее срока действия. Максимальный срок действия подписки без данных ресурсов Outlook составляет 4230 минут (менее 3 дней) и 1 день с данными ресурсов. 

Если вы потеряете разрешение, предоставленное ранее для подписки, а срок действия подписки тем временем истекает, запросите разрешение еще раз, чтобы [создать](/graph/api/subscription-post-subscriptions) новую подписку.

## <a name="receive-notification-payloads"></a>Получение полезных данных уведомлений

В зависимости от подписки уведомления могут включать данные о ресурсах. Подписки с данными ресурсов позволяют получать полезные данные ресурса вместе с уведомлением, избегая накладных расходов на отдельный вызов API для получения измененных данных ресурса.

### <a name="receive-notifications-with-resource-data-preview"></a>Получение уведомлений с данными ресурсов (предварительная версия)

Ниже приведен пример полезных данных уведомления с данными ресурса ресурса **message**. Свойства **resource** и **resourceData** соответствуют экземпляру **message**, который вызвал уведомление. Используйте свойство **encryptedContent** для расшифровки данных ресурса.

```json
{
    "value": [
      {
        "subscriptionId": "dfd11b2f-8222-4189-9545-4205c95d6235",
        "subscriptionExpirationDateTime": "2021-12-31T16:16:44.9907405+05:30",
        "changeType": "created",
        "resource": "Users('722effaf-0433-4272-9ac4-d5ec11c3cd77')/messages('AAMkAGUwNjQ4ZjIxLTQ3Y2Y8AAA=')",
        "clientState": "<<--SpecifiedClientState-->>",
        "tenantId": "<<--TenantForWhichNotificationWasSent-->>",
        "encryptedContent": {
          "data": "<<--EncryptedContent-->>",
          "dataKey": "<<--EnryptedDataKeyUsedForEncryptingContent-->>",        
          "dataSignature": "Qw/9ubWeUYJPWWXvNiGgct2FkNG2MXTRm/BLUpJM66k=",
          "encryptionCertificateId": "<<--IdOfTheCertificateUsedForEncryptingDataKey-->>",
          "encryptionCertificateThumbprint": "<<--ThumbprintOfTheCertificateUsedForEncryptingDataKey-->>"
        },
        "resourceData": {
          "@odata.type": "#microsoft.graph.message",
          "@odata.id": "Users('722effaf-0433-4272-9ac4-d5ec11c3cd77')/messages('AAMkAGUwNjQ4ZjIxLTQ3Y2Y8AAA=')",
          "@odata.etag": "W/\"CQAAABYAAACQ2fKdhq8oSKEDSVrdi3lRAAGDUR8n\"",
          "id": "AAMkAGUwNjQ4ZjIxLTQ3Y2Y8AAA="
        }
      }
    ]
    "validationTokens": ["<<--ValidationTokens-->>"]
}
```

Дополнительные сведения о проверке маркеров и расшифровке полезных данных см. в статье [Настройка уведомлений об изменениях, включающих данные ресурсов](webhooks-with-resource-data.md).

Ниже приводится пример расшифрованных полезных данных уведомления. Расшифрованные полезные данные соответствуют схеме [message](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true) Outlook. Полезные данные похожи на результаты, возвращаемые операцией [GET message](/graph/api/message-get?view=graph-rest-beta&preserve-view=true). Однако полезные данные уведомления содержат только те свойства, которые указаны с помощью параметра `$select` в свойстве **resource** подписки. Полезные данные уведомлений для других ресурсов Outlook, таких как [contact](/graph/api/resources/contact?view=graph-rest-beta&preserve-view=true) и [event](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true), следуют соответствующим схемам. 

```json
{
    "receivedDateTime@odata.type":"#DateTimeOffset",
    "receivedDateTime":"2021-12-30T10:53:35Z",
    "subject":"TEST MESSAGE FOR RICH NOTIFICATIONS",
    "bodyPreview":"Hello,\r\n\r\nWhat\u2019s up?\r\n\r\nThanks\r\nMegan",
    "importance@odata.type":"#microsoft.graph.importance",
    "importance":"normal",
    "from": {
        "@odata.type":"#microsoft.graph.recipient",
        "emailAddress": {
            "@odata.type":"#microsoft.graph.emailAddress",
            "name":"Megan Brown",
            "address":"Megan.Brown@microsoft.com"
        }
    }
}
```

### <a name="receive-notifications-without-resource-data"></a>Получение уведомлений без данных ресурса

Уведомления без данных ресурса предоставляют достаточно сведений, чтобы выполнить вызов GET для получения ресурса. Для подписок на уведомления без данных ресурса не требуется сертификат шифрования (так как фактические данные ресурса не передаются).

В следующем примере показаны полезные данные уведомления, соответствующего ресурсу **message** Outlook. Оно включает свойства **resource** и **resourceData**, представляющие ресурс, который вызвал уведомление. Используйте свойства **resource** и **@odata.id** для вызовов в Microsoft Graph, чтобы получить полезные данные ресурса.

> **Примечание**. Вызовы GET всегда возвращают текущее состояние ресурса. Если ресурс изменяется между моментом отправки уведомления и моментом извлечения ресурса, операция возвращает состояние ресурса при извлечении.


```json
"value": [
 {
   "subscriptionId": "c6126aa3-0ed8-412f-a988-71e6cee627c4",
   "subscriptionExpirationDateTime": "2022-01-02T03:12:18.2257768+05:30",
   "changeType": "created",    
   "resource": "Users/622eaaff-0683-4862-9de4-f2ec83c2bd98/Messages/AAMkAGUwNjQ4ZjIxAAA=",
   "resourceData": {      
     "@odata.type": "#Microsoft.Graph.Message",
     "@odata.id": "Users/622eaaff-0683-4862-9de4-f2ec83c2bd98/Messages/AAMkAGUwNjQ4ZjIAAA=",
     "@odata.etag": "W/\"CQAAABYAAACQ2fKdhq8oSKEDSVrdi3lRAAGDUUXn\"",
     "id": "AAMkAGUwNjQ4ZjIxAAA="
   },
   "clientState": "<<--SpecifiedClientState-->>",
   "tenantId": "<<--TenantForWhichNotificationWasSent-->>"
 }
]
```


## <a name="examples"></a>Примеры

### <a name="example-1-create-a-subscription-to-get-change-notifications-without-resource-data-when-the-user-receives-a-new-message"></a>Пример 1. Создание подписки для получения уведомлений об изменениях без данных ресурсов, когда пользователь получает новое сообщение
В следующем примере запрашивается уведомление о создании сообщения в почтовом ящике пользователя.

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "create_subscription_withoutresourcedata_for_message_resource"
}-->

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-type: application/json

{
    "changeType": "created",
    "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
    "resource": "users/622eaaff-0683-4862-9de4-f2ec83c2bd98/messages",
    "expirationDateTime": "2021-07-07T21:42:18.2257768+00:00",
    "clientState": "secretClientState"
}
```

#### <a name="response"></a>Отклик
Ниже приведен пример отклика. 
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions/$entity",
    "id": "5522bd62-7c96-4530-85b0-00b916f6151a",
    "resource": "users/622eaaff-0683-4862-9de4-f2ec83c2bd98/messages",
    "applicationId": "507c3b9a-67b8-463d-88a2-15a8cefb2111",
    "changeType": "created",
    "clientState": "secretClientState",
    "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
    "notificationQueryOptions": null,
    "notificationContentType": null,
    "lifecycleNotificationUrl": null,
    "expirationDateTime": "2022-01-01T21:42:18.2257768Z",
    "creatorId": "a4c7bd34-4f3b-46b7-a25d-b63c1e2a2842",
    "includeResourceData": null,
    "latestSupportedTlsVersion": "v1_2",
    "encryptionCertificate": null,
    "encryptionCertificateId": null,
    "notificationUrlAppId": null
}
```

### <a name="example-2-create-a-subscription-to-get-change-notifications-with-resource-data-when-the-user-receives-a-new-message-preview"></a>Пример 2. Создание подписки для получения уведомлений об изменениях с данными ресурсов, когда пользователь получает новое сообщение (предварительная версия)
В следующем примере выполняется подписка на уведомления с данными ресурсов для сообщения, создаваемого в почтовом ящике пользователя. Свойства ресурса **message**, которые должны быть включены в полезные данные уведомления, указываются с помощью параметра запроса `$select`.

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "create_subscription_withresourcedata_for_message_resource"
}-->

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-type: application/json

{ 
    "changeType": "created",
    "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
    "resource": "users/622eaaff-0683-4862-9de4-f2ec83c2bd98/messages?$select=Subject,bodyPreview,importance,receivedDateTime,from",
    "expirationDateTime": "2022-01-01T21:42:18.2257768+00:00",
    "clientState": "secretClientValue",
    "includeResourceData": true,
    "encryptionCertificate": "MIIDMzCCAhugAwIBAgIQE7D+++Dk1hKQBqWA==",
    "encryptionCertificateId": "testCertificateId"
}
```

#### <a name="response"></a>Отклик
Ниже приведен пример отклика. 
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions/$entity",
    "id": "178eec5f-cf3c-4e7e-8a9c-8640deb5b5c5",
    "resource": "users/622eaaff-0683-4862-9de4-f2ec83c2bd98/messages?$select=Subject,bodyPreview,importance,receivedDateTime,from",
    "applicationId": "507c3b9a-67b8-463d-88a2-15a8cefb2111",
    "changeType": "created",
    "clientState": "secretClientValue",
    "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
    "notificationQueryOptions": null,
    "notificationContentType": null,
    "lifecycleNotificationUrl": null,
    "expirationDateTime": "2022-01-01T12:32:35.1582696Z",
    "creatorId": "a4c7bd34-4f3b-46b7-a25d-b63c1e2a2842",
    "includeResourceData": true,
    "latestSupportedTlsVersion": "v1_2",
    "encryptionCertificate": "MIIDMzCCAhugAwIBAgIQE7D+++Dk1hKQBqWA==",
    "encryptionCertificateId": "testCertificateId",
    "notificationUrlAppId": null
}
```

### <a name="example-3-create-a-subscription-to-get-change-notifications-with-resource-data-for-a-message-based-on-a-condition-preview"></a>Пример 3. Создание подписки для получения уведомлений об изменениях с данными ресурсов для сообщения на основе условия (предварительная версия)
В следующем примере выполняется подписка на уведомления с данными ресурсов для сообщения, создаваемого в папке «Черновики», содержащего одно или несколько вложений и имеющих высокую важность.

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "create_subscription_withresourcedata_for_message_resource_basedonfilter"
}-->

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-type: application/json

{ 
    "changeType": "created",
    "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
    "resource": "me/mailfolders('Drafts')/messages?$select=Subject,bodyPreview&$filter=hasAttachments eq true AND importance eq 'High'",
    "expirationDateTime": "2022-01-01T21:42:18.2257768+00:00",
    "clientState": "secretClientValue",
    "includeResourceData": true,
    "encryptionCertificate": "MIIDMzCCAhugAwIBAgIQE7D+++Dk1hKQBqWA==",
    "encryptionCertificateId": "testCertificateId"
}
```

#### <a name="response"></a>Отклик
Ниже приведен пример отклика. 
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions/$entity",
    "id": "239dbc5f-cf3c-4e7e-8c9c-3340abc5b5c5",
    "resource": "me/mailfolders('Drafts')/messages?$select=Subject,bodyPreview&$filter=hasAttachments eq true AND importance eq 'High'",
    "applicationId": "507c3b9a-67b8-463d-88a2-15a8cefb2111",
    "changeType": "created",
    "clientState": "secretClientValue",
    "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
    "notificationQueryOptions": null,
    "notificationContentType": null,
    "lifecycleNotificationUrl": null,
    "expirationDateTime": "2022-01-20T12:32:35.1582696Z",
    "creatorId": "a4c7bd34-4f3b-46b7-a25d-b63c1e2a2842",
    "includeResourceData": true,
    "latestSupportedTlsVersion": "v1_2",
    "encryptionCertificate": "MIIDMzCCAhugAwIBAgIQE7D+++Dk1hKQBqWA==",
    "encryptionCertificateId": "testCertificateId",
    "notificationUrlAppId": null
}
```

## <a name="see-also"></a>См. также
- [Уведомления об изменениях в Microsoft Graph](webhooks.md)
- [Настройка уведомлений об изменениях, включающих данные ресурсов](webhooks-with-resource-data.md)
- [Обзор API почты Outlook](outlook-mail-concept-overview.md)
- [Обзор API для личных контактов Outlook](outlook-contacts-concept-overview.md)
- [Обзор API календаря Outlook](outlook-calendar-concept-overview.md)
