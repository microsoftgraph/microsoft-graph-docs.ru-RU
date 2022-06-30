---
title: Перечисление подписок
description: Получение свойств и связей подписок на веб-перехватчики с учетом идентификатора приложения, пользователя и его роли в клиенте.
ms.localizationpriority: high
author: Jumaodhiss
ms.prod: change-notifications
doc_type: apiPageType
ms.openlocfilehash: 8cfe80146aaf6f23069e83245541cfa221190a78
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2022
ms.locfileid: "66555900"
---
# <a name="list-subscriptions"></a>Перечисление подписок

Пространство имен: microsoft.graph

Получение свойств и связей подписок на веб-перехватчики с учетом идентификатора приложения, пользователя и его роли в клиенте.

Содержимое ответа зависит от контекста, в котором вызывается приложение; подробные сведения см. в разделе [Разрешения](#permissions).

## <a name="permissions"></a>Разрешения

Этот API поддерживает перечисленные ниже области разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).

| Поддерживаемый ресурс | Делегированное (рабочая или учебная учетная запись) | Делегированное (личная учетная запись Майкрософт) | Application |
|:-----|:-----|:-----|:-----|
|[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords) | Не поддерживается | Не поддерживается | CallRecords.Read.All  |
|[channel](../resources/channel.md) (/teams/getAllChannels — все каналы в организации) | Не поддерживается  | Не поддерживается | Channel.ReadBasic.All, ChannelSettings.Read.All |
|[channel](../resources/channel.md) (/teams/{id}/channels) | Channel.ReadBasic.All, ChannelSettings.Read.All, Subscription.Read.All  | Не поддерживается | Channel.ReadBasic.All, ChannelSettings.Read.All  |
|[чат](../resources/chat.md) (/чаты — все чаты в организации) | Не поддерживается | Не поддерживается | Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All |
|[чат](../resources/chat.md) (/chats/{id}) | Chat.ReadBasic, Chat.Read, Chat.ReadWrite, Subscription.Read.All | Не поддерживается | ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All |
|[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages) | ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All, Subscription.Read.All | Не поддерживается | ChannelMessage.Read.Group*, ChannelMessage.Read.All  |
|[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации) | Не поддерживается | Не поддерживается | ChannelMessage.Read.All  |
|[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages) | Chat.Read, Chat.ReadWrite, Subscription.Read.All | Не поддерживается | Chat.Read.All  |
|[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации) | Не поддерживается | Не поддерживается | Chat.Read.All  |
|[chatMessage](../resources/chatmessage.md) (/users/{id}/chats/getAllMessages — сообщения чата для всех чатов, в которые входит определенный пользователь) | Chat.Read, Chat.ReadWrite | Не поддерживается | Chat.Read.All, Chat.ReadWrite.All |
|[contact](../resources/contact.md) | Contacts.Read, Subscription.Read.All | Contacts.Read, Subscription.Read.All | Contacts.Read |
|[conversationMember](../resources/conversationmember.md) (/teams/{id}/channels/getAllMembers) | Не поддерживается | Не поддерживается | ChannelMember.Read.All |
|[conversationMember](../resources/conversationmember.md) (/chats/getAllMembers) | Не поддерживается | Не поддерживается | ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All |
|[conversationMember](../resources/conversationmember.md) (/chats/{id}/members) | ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite, Subscription.Read.All | Не поддерживается | ChatMember.Read.Chat *, Chat.Manage.Chat*, ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All |
|[conversationMember](../resources/conversationmember.md) (/teams/{id}/members) | TeamMember.Read.All, Subscription.Read.All | Не поддерживается | TeamMember.Read.All |
|[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя) | Не поддерживается | Files.ReadWrite, Subscription.Read.All | Не поддерживается |
|[driveItem](../resources/driveitem.md) (OneDrive для бизнеса) | Files.ReadWrite.All, Subscription.Read.All | Не поддерживается | Files.ReadWrite.All |
|[event](../resources/event.md) | Calendars.Read, Subscription.Read.All | Calendars.Read, Subscription.Read.All | Calendars.Read |
|[group](../resources/group.md) | Group.Read.All, Subscription.Read.All | Не поддерживается | Group.Read.All |
|[group conversation](../resources/conversation.md) | Group.Read.All, Subscription.Read.All | Не поддерживается | Не поддерживается |
|[list](../resources/list.md) | Sites.ReadWrite.All, Subscription.Read.All | Не поддерживается | Sites.ReadWrite.All |
|[message](../resources/message.md) | Mail.ReadBasic, Mail.Read, Subscription.Read.All | Mail.ReadBasic, Mail.Read, Subscription.Read.All | Mail.Read |
|[presence](../resources/presence.md) | Presence.Read.All, Subscription.Read.All | Не поддерживается | Не поддерживается |
|[printer](../resources/printer.md) | Не поддерживается | Не поддерживается | Printer.Read.All, Printer.ReadWrite.All |
|[printTaskDefinition](../resources/printtaskdefinition.md) | Не поддерживается | Не поддерживается | PrintTaskDefinition.ReadWrite.All |
|[security alert](../resources/alert.md) | SecurityEvents.ReadWrite.All, Subscription.Read.All | Не поддерживается | SecurityEvents.ReadWrite.All |
|[teams](../resources/team.md) (/teams — все команды в организации) | Не поддерживается | Не поддерживается | Team.ReadBasic.All, TeamSettings.Read.All |
|[team](../resources/team.md) (/teams/{id}) | Team.ReadBasic.All, TeamSettings.Read.All, Subscription.Read.All | Не поддерживается | Team.ReadBasic.All, TeamSettings.Read.All |
|[todoTask](../resources/todotask.md) | Tasks.ReadWrite, Subscription.Read.All | Tasks.ReadWrite, Subscription.Read.All | Не поддерживается |
|[user](../resources/user.md) | User.Read.All, Subscription.Read.All | User.Read.All | User.Read.All |

> **Примечание**. Разрешения, помеченные звездочкой (*), используют [согласие для конкретных ресурсов](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).

Результаты отклика основаны на контексте приложения, отправившего вызов. В следующих разделах описываются общие сценарии.

### <a name="basic-scenarios"></a>Основные сценарии

Чаще всего приложению нужно получить подписки, изначально созданные им для текущего пользователя или для всех пользователей в каталоге (рабочих или учебных учетных записей). В этих сценариях не требуется никаких особых разрешений, помимо тех, которые приложение изначально использовало для создания своих подписок.

| Контекст приложения, отправившего вызов | Состав отклика |
|:-----|:---------------- |
| Приложение отправляет вызов от имени вошедшего пользователя (делегированное разрешение). <br/>-и-<br/>У приложения есть исходное разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md).<br/><br/>Примечание. Это относится как к личным учетным записям Майкрософт, так и к рабочим и учебным учетным записям. | Подписки, созданные **этим приложением** только для вошедшего пользователя. |
| Приложение отправляет вызов от своего имени (разрешение приложения).<br/>-и-<br/>У приложения есть исходное разрешение, необходимое для [создания подписки](subscription-post-subscriptions.md).<br/><br/>**Примечание:** Это относится только к рабочим и учебным учетным записям.| Подписки, созданные **этим приложением** для себя или для любого пользователя в каталоге.|

### <a name="advanced-scenarios"></a>Расширенные сценарии

В некоторых случаях приложению нужно получить подписки, созданные другими приложениями. Например, пользователь хочет просмотреть все подписки, созданные каким-либо приложением от его имени. Администратору может потребоваться просмотреть все подписки из всех приложений в своем каталоге.
В таких сценариях требуется делегированное разрешение Subscription.Read.All.

| Контекст приложения, отправившего вызов | Состав отклика |
|:-----|:---------------- |
| Приложение отправляет вызов от имени вошедшего пользователя (делегированное разрешение). *Пользователь не является администратором*. <br/>-и-<br/>У приложения есть разрешение Subscription.Read.All<br/><br/>Примечание. Это относится как к личным учетным записям Майкрософт, так и к рабочим и учебным учетным записям. | Подписки, созданные **любым приложением** только для вошедшего пользователя. |
| Приложение отправляет вызов от имени вошедшего пользователя (делегированное разрешение). *Пользователь является администратором*.<br/>-и-<br/>У приложения есть разрешение Subscription.Read.All<br/><br/>Примечание. Это относится только к рабочим или учебным учетным записям. | Подписки, созданные **любым приложением** для **любого пользователя** в каталоге.|

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод не поддерживает [параметры запроса OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и список объектов [subscription](../resources/subscription.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/subscriptions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-subscriptions-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-subscriptions-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример ответа.  

>**Примечание:** Ответ, показанный здесь, может быть сокращен для читаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscriptions",
  "value": [
    {
      "id": "0fc0d6db-0073-42e5-a186-853da75fb308",
      "resource": "Users",
      "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
      "changeType": "updated,deleted",
      "clientState": null,
      "notificationUrl": "https://webhookappexample.azurewebsites.net/api/notifications",
      "lifecycleNotificationUrl":"https://webhook.azurewebsites.net/api/send/lifecycleNotifications",
      "expirationDateTime": "2018-03-12T05:00:00Z",
      "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
      "latestSupportedTlsVersion": "v1_2",
      "encryptionCertificate": "",
      "encryptionCertificateId": "",
      "includeResourceData": false,
      "notificationContentType": "application/json"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List subscriptions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

> **Примечание.** Значение свойства `clientState` не возвращается в целях безопасности.

Когда запрос возвращает несколько страниц данных, отклик включает свойство `@odata.nextLink`, помогающее управлять результатами. Дополнительные сведения см. в статье [Разбиение данных Microsoft Graph по страницам в приложении](/graph/paging).
