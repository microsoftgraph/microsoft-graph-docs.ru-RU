---
title: Создание подписки
description: Подписывает приложение прослушивателя на получение уведомлений об изменениях при изменении данных в ресурсе Microsoft Graph.
localization_priority: Normal
author: baywet
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 3e9873d8def179bfdbe8d77767d5a521af5cebf3
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353261"
---
# <a name="create-subscription"></a>Создание подписки

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Подписывает приложение прослушивателя на получение уведомлений об изменениях, когда запрошенный тип изменений выполняется для указанного ресурса в Microsoft Graph.

## <a name="permissions"></a>Разрешения

Для создания подписки необходимо разрешение на чтение ресурса. Например, чтобы получать уведомления об изменениях для сообщений, вашему приложению требуется разрешение mail. Read. 
 
 В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Поддерживаемый ресурс | Делегированное (рабочая или учебная учетная запись) | Делегированное (личная учетная запись Майкрософт) | Для приложений |
|:-----|:-----|:-----|:-----|
|[каллрекорд](../resources/callrecords-callrecord.md) (/коммуникатионс/каллрекордс) | Не поддерживается | Не поддерживается | CallRecords.Read.All  |
|[chatMessage](../resources/chatmessage.md) (/теамс/{ИД}/чаннелс/{ИД}/мессажес) | Не поддерживается | Не поддерживается | ChannelMessage.Read.All  |
|[chatMessage](../resources/chatmessage.md) (/теамс/аллмессажес--все сообщения каналов в организации) | Не поддерживается | Не поддерживается | ChannelMessage.Read.All  |
|[chatMessage](../resources/chatmessage.md) (/ЧАТС/{ИД}/мессажес) | Не поддерживается | Не поддерживается | Chat.Read.All  |
|[chatMessage](../resources/chatmessage.md) (/ЧАТС/аллмессажес--все сообщения чата в организации) | Не поддерживается | Не поддерживается | Chat.Read.All  |
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

### <a name="chatmessage-microsoft-teams"></a>chatMessage (Microsoft Teams)

для подписок на **chatMessage** требуется [Шифрование](/graph/webhooks-with-resource-data). Если [енкриптионцертификате](../resources/subscription.md) не указан, создание подписки завершится с ошибками. Перед созданием подписки на **chatMessage** необходимо запросить доступ. Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis). 

> **Примечание:** `/teams/allMessages` и `/chats/allMessages` в настоящее время находятся в предварительной версии. Во время предварительной версии вы можете использовать этот API без сборов в соответствии с [условиями использования API Майкрософт](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context). Однако пользователям приложений, использующих API, может потребоваться подписка на конкретные решения Microsoft 365. После общедоступной доступности Корпорация Майкрософт может потребовать от вас или ваших клиентов взимать дополнительные сборы на основе объема данных, доступ к которым осуществляется через API.

### <a name="driveitem-onedrive"></a>driveItem (OneDrive)

Дополнительные ограничения применяются к подпискам на элементы OneDrive. Ограничения применяются к созданию и управлению (получению, обновлению и удалению) подписок.

В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище. В OneDrive для бизнеса можно подписаться только на корневую папку. Уведомления об изменениях отправляются для запрошенных типов изменений в подписанной папке, а также любых файлов, папок или других экземпляров **driveItem** в иерархии. Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.

### <a name="contact-event-and-message-outlook"></a>Contact, Event и Message (Outlook)

Дополнительные ограничения применяются для подписок на элементы Outlook. Ограничения применяются к созданию и управлению (получению, обновлению и удалению) подписок.

- Делегированное разрешение поддерживает подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход. Это означает, например, что нельзя использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.
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

В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [Subscription](../resources/subscription.md) в тексте отклика.

Сведения о том, как возвращаются ошибки, приведены в разделе [ошибочные ответы][error-response].

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.
Поля `clientState` и `latestSupportedTlsVersion` необязательны.

Этот запрос создает подписку на уведомления об изменениях новой почты, полученной в текущий момент, когда пользователь выполнил вход.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/beta/subscriptions
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

---


Ниже приведены допустимые значения свойства Resource.

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
|Оповещение безопасности|security/alerts?$filter=status eq ‘New’|
|Записи звонков|связь/Каллрекордс|

### <a name="response"></a>Отклик

Ниже показан пример отклика. 

>**Примечание.** Представленный здесь объект ответа может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions/$entity",
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

Конечная точка уведомления о подписке (указанная в свойстве **notificationUrl** ) должна иметь возможность отвечать на запрос проверки, как описано в статье [Настройка уведомлений для изменений в пользовательских данных](/graph/webhooks#notification-endpoint-validation). Если проверка завершилась сбоем, запрос на создание подписки возвращает ошибку 400 (неверный запрос).

[error-response]: /graph/errors

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
