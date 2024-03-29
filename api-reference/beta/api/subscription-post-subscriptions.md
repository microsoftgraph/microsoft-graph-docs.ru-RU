---
title: Создание подписки
description: Подписывает приложение прослушивателя на получение уведомлений об изменениях при изменении данных в ресурсе Microsoft Graph.
ms.localizationpriority: medium
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: e64abb2c70c0f51a8b2942ba0b165f047a596c01
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66445211"
---
# <a name="create-subscription"></a>Создание подписки

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [todo-deprecate-basetaskapi-sharedfeature](../includes/todo-deprecate-basetaskapi-sharedfeature.md)]

Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления об изменениях определенного типа в указанном ресурсе в Microsoft Graph.

Список ресурсов, поддерживающих подписку на уведомления об изменениях, см. в таблице раздела [Разрешения](#permissions).

Некоторые ресурсы поддерживают возможность включить зашифрованные данные ресурсов в уведомления об изменениях. К этим ресурсам относятся [chatMessage](../resources/chatmessage.md), [контакт](../resources/contact.md), [событие](../resources/event.md), [сообщение](../resources/message.md), [onlineMeetings](../resources/onlinemeeting.md) и [сведения о присутствии](../resources/presence.md). Дополнительные сведения см. в статьях [Настройка уведомлений об изменениях, включающих данные ресурсов](/graph/webhooks-with-resource-data) и [Уведомления об изменениях, связанных с ресурсами Outlook, в Microsoft Graph](/graph/outlook-change-notification-overview).

## <a name="permissions"></a>Разрешения

Для создания подписки требуется разрешение на чтение ресурса. Например, чтобы получать уведомления об изменениях в сообщениях, приложению необходимо разрешение Mail.Read. 

В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API. Чтобы узнать больше, в том числе, [как соблюдать осторожность ](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений, найдите следующие разрешения в [Разрешениях](/graph/permissions-reference).

| Поддерживаемый ресурс | Делегированное (рабочая или учебная учетная запись) | Делегированное (личная учетная запись Майкрософт) | Приложение |
|:-----|:-----|:-----|:-----|
|[baseTask](../resources/basetask.md) (не рекомендуется) | Tasks.ReadWrite | Tasks.ReadWrite | Не поддерживается |
|[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords) | Не поддерживается | Не поддерживается | CallRecords.Read.All  |
|[channel](../resources/channel.md) (/teams/getAllChannels — все каналы в организации) | Не поддерживается  | Не поддерживается | Channel.ReadBasic.All, ChannelSettings.Read.All |
|[channel](../resources/channel.md) (/teams/{id}/channels) | Channel.ReadBasic.All, ChannelSettings.Read.All  | Не поддерживается | Channel.ReadBasic.All, ChannelSettings.Read.All  |
|[чат](../resources/chat.md) (/чаты — все чаты в организации) | Не поддерживается | Не поддерживается | Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All |
|[чат](../resources/chat.md) (/chats/{id}) | Chat.ReadBasic, Chat.Read, Chat.ReadWrite | Не поддерживается | ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All |
|[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages) | ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All | Не поддерживается | ChannelMessage.Read.Group*, ChannelMessage.Read.All  |
|[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации) | Не поддерживается | Не поддерживается | ChannelMessage.Read.All  |
|[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages) | Chat.Read, Chat.ReadWrite | Не поддерживается | Chat.Read.All  |
|[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации) | Не поддерживается | Не поддерживается | Chat.Read.All  |
|[chatMessage](../resources/chatmessage.md) (/users/{id}/chats/getAllMessages — сообщения чата для всех чатов, в которые входит определенный пользователь) | Chat.Read, Chat.ReadWrite | Не поддерживается | Chat.Read.All, Chat.ReadWrite.All |
|[contact](../resources/contact.md) | Contacts.Read | Contacts.Read | Contacts.Read |
|[conversationMember](../resources/conversationmember.md) (/chats/getAllMembers) | Не поддерживается | Не поддерживается | ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All |
|[conversationMember](../resources/conversationmember.md) (/chats/{id}/members) | ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite | Не поддерживается | ChatMember.Read.Chat *, Chat.Manage.Chat*, ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All |
|[conversationMember](../resources/conversationmember.md) (/teams/getAllMembers) | Не поддерживается | Не поддерживается | TeamMember.Read.All, TeamMember.ReadWrite.All |
|[conversationMember](../resources/conversationmember.md) (/teams/{id}/members) | TeamMember.Read.All | Не поддерживается | TeamMember.Read.All |
|[conversationMember](../resources/conversationmember.md) (/teams/{id}/channels/getAllMembers) | Не поддерживается | Не поддерживается | ChannelMember.Read.All |
|[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя) | Не поддерживается | Files.ReadWrite | Не поддерживается |
|[driveItem](../resources/driveitem.md) (OneDrive для бизнеса) | Files.ReadWrite.All | Не поддерживается | Files.ReadWrite.All |
|[event](../resources/event.md) | Calendars.Read | Calendars.Read | Calendars.Read |
|[group](../resources/group.md) | Group.Read.All | Не поддерживается | Group.Read.All |
|[group conversation](../resources/conversation.md) | Group.Read.All | Не поддерживается | Не поддерживается |
|[list](../resources/list.md) | Sites.ReadWrite.All | Не поддерживается | Sites.ReadWrite.All |
|[message](../resources/message.md) | Mail.ReadBasic, Mail.Read | Mail.ReadBasic, Mail.Read | Mail.Read |
|[собрание по сети](../resources/onlinemeeting.md) | Не поддерживается | Не поддерживается | OnlineMeetings.Read.All, OnlineMeetings.ReadWrite.All |
|[presence](../resources/presence.md) | Presence.Read.All | Не поддерживается | Не поддерживается |
|[printer](../resources/printer.md) | Не поддерживается | Не поддерживается | Printer.Read.All, Printer.ReadWrite.All |
|[printTaskDefinition](../resources/printtaskdefinition.md) | Не поддерживается | Не поддерживается | PrintTaskDefinition.ReadWrite.All |
|[security alert](../resources/alert.md) | SecurityEvents.ReadWrite.All | Не поддерживается | SecurityEvents.ReadWrite.All |
|[teams](../resources/team.md) (/teams — все команды в организации) | Не поддерживается | Не поддерживается | Team.ReadBasic.All, TeamSettings.Read.All |
|[team](../resources/team.md) (/teams/{id}) | Team.ReadBasic.All, TeamSettings.Read.All | Не поддерживается | Team.ReadBasic.All, TeamSettings.Read.All |
|[todoTask](../resources/todotask.md) | Tasks.ReadWrite | Tasks.ReadWrite | Не поддерживается |
|[user](../resources/user.md) | User.Read.All | User.Read.All | User.Read.All |

Рекомендуется использовать разрешения, как описано в предыдущей таблице. Из-за ограничений безопасности подписки Microsoft Graph не будут поддерживать разрешения на запись, если необходимы только разрешения на чтение.

> **Примечание**. Разрешения, помеченные звездочкой (*), используют [согласие для конкретных ресурсов](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a>driveItem

Дополнительные ограничения применяются к подпискам на элементы OneDrive. Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.

В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище. В OneDrive для бизнеса можно подписаться только на корневую папку. Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии. Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.

OneDrive для бизнеса и SharePoint поддерживают отправку уведомлений приложений о событиях безопасности, которые происходят в **driveItem**. Чтобы подписаться на эти события, добавьте заголовок `prefer:includesecuritywebhooks` в запрос на создание подписки. После создания подписки вы будете получать уведомления об изменениях разрешений для элемента. Этот заголовок можно использовать в SharePoint и OneDrive для бизнеса, но не в учетных записях потребителей в OneDrive.

### <a name="contact-event-and-message"></a>contact, event и message

Вы можете подписаться на изменения в ресурсах контактов **, событий** или сообщений Outlook и при необходимости указать в полезных данных запроса POST, следует ли включать зашифрованные данные ресурсов в уведомления.

[!INCLUDE [outlook-subscription-notes](../../includes/outlook-subscription-notes.md)]

### <a name="onlinemeetings-presence"></a>onlineMeetings, presence

Для подписок **на onlineMeetings** и **presence** требуется свойство **encryptionCertificate** и **encryptionCertificateId** при [](/graph/webhooks-with-resource-data#creating-a-subscription) создании подписки для уведомлений с зашифрованными данными ресурсов. Дополнительные сведения см. [в статье о настройке уведомлений об изменениях для получения данных о ресурсах](/graph/webhooks-with-resource-data).
Дополнительные сведения о подписках на собрания по сети см. в статье ["Получение уведомлений об изменениях для собраний по сети"](/graph/changenotifications-for-onlinemeeting).

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `201 Created` отклика [и объект](../resources/subscription.md) подписки в тексте отклика.

Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.
Поля `clientState` и `latestSupportedTlsVersion` необязательны.

Этот запрос создает подписку для уведомлений об изменениях новых сообщений, полученных текущим пользователем, выполнившего вход.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-type: application/json

{
   "changeType": "created",
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

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-subscription-from-subscriptions-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-subscription-from-subscriptions-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON. Поля `clientState` и `latestSupportedTlsVersion` не являются обязательными.

#### <a name="resources-examples"></a>Примеры ресурсов

Ниже приведены допустимые значения для свойства ресурса.

| Тип ресурса | Примеры |
|:------ |:----- |
|[baseTask](../resources/basetask.md) (не рекомендуется) | `/me/tasks/lists/{Id}/tasks`
|[Записи звонков](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[Каналами](../resources/channel.md)|`/teams/getAllChannels`, `/teams/{id}/channels`|
|[Чат](../resources/chat.md)|`/chats`, `/chats/{id}`|
|[Сообщение чата](../resources/chatmessage.md) | `chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages` |
|[Контакты](../resources/contact.md)|`me/contacts`|
|[ConversationMember](../resources/conversationmember.md)|`/chats/{id}/members`, `/chats/getAllMembers`, `/teams/{id}/members`, `/teams/getAllMembers`, `/teams/{id}/channels/getAllMembers`|
|[Беседы](../resources/conversation.md)|`groups('{id}')/conversations`|
|[Диски](../resources/driveitem.md)|`me/drive/root`|
|[События](../resources/event.md)|`me/events`|
|[Группы](../resources/group.md)|`groups`|
|[Список](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[Почта](../resources/message.md)|`me/mailfolders('inbox')/messages`, `me/messages`|
|[OnlineMeetings](../resources/onlinemeeting.md)|`/communications/onlineMeetings/?$filter=JoinWebUrl eq '{JoinWebUrl}'`|
|[Присутствие](../resources/presence.md)| `/communications/presences/{id}` (один пользователь), `/communications/presences?$filter=id in ('{id}','{id}',…)` (несколько пользователей)|
|[printer](../resources/printer.md) |`print/printers/{id}/jobs`|
|[PrintTaskDefinition](../resources/printtaskdefinition.md)|`print/taskDefinitions/{id}/tasks`|
|[Teams](../resources/team.md)|`/teams`, `/teams/{id}`|
|[Пользователи](../resources/user.md)|`users`|
|[todoTask](../resources/todotask.md) | `/me/todo/lists/{todoTaskListId}/tasks`
|[Оповещение безопасности](../resources/alert.md)|`security/alerts?$filter=status eq 'NewAlert'`|

> **Примечание.** Любой путь, начинающийся с `me`, также можно использовать с `users/{id}` вместо `me`, чтобы указать определенного пользователя, а не текущего пользователя.

### <a name="response"></a>Отклик

Ниже показан пример отклика. 

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
  "id": "7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource": "me/mailFolders('Inbox')/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType": "created",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2",
  "notificationContentType": "application/json"
}
```

#### <a name="notification-endpoint-validation"></a>Проверка конечной точки уведомлений

Конечная точка уведомления о подписке (указанная в свойстве **notificationUrl** ) должна отвечать на запрос проверки, как описано в разделе "Настройка уведомлений об изменениях в данных [пользователя"](/graph/webhooks#notification-endpoint-validation). Если проверка завершилась сбоем, запрос на создание подписки возвращает ошибку 400 (неверный запрос).

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

