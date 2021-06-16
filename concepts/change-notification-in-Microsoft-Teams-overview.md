---
title: Уведомления об изменениях ресурсов Microsoft Teams с использованием Microsoft Graph
description: Узнайте, как получать уведомления об изменениях (создание, обновление и удаление) ресурсов в Microsoft Teams с помощью API Microsoft Graph
author: anandab-msft
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 9433a4c5ee000fa34e125440168b865f1bb16172
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941568"
---
# <a name="change-notifications-for-microsoft-teams-resources-using-microsoft-graph"></a><span data-ttu-id="b2e7a-103">Уведомления об изменениях ресурсов Microsoft Teams с использованием Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b2e7a-103">Change notifications for Microsoft Teams resources using Microsoft Graph</span></span>

<span data-ttu-id="b2e7a-104">Уведомления об изменениях позволяют подписаться на изменения (создание, обновление и удаление) ресурса.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-104">Change notifications enable you to subscribe to changes (create, update, and delete) to a resource.</span></span> <span data-ttu-id="b2e7a-105">Уведомления об изменениях обеспечивают модель с низкой задержкой, позволяя управлять [подпиской](/graph/api/resources/webhooks?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="b2e7a-105">Change notifications provide a low latency model by allowing you to maintain a [subscription](/graph/api/resources/webhooks?preserve-view=true).</span></span> <span data-ttu-id="b2e7a-106">Кроме того, вы можете получать данные ресурсов в уведомлениях и, следовательно, избегать вызова API, чтобы получить полезные данные.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-106">You can also get the resource data in the notifications and therefore avoid calling the API to get the payload.</span></span>

> <span data-ttu-id="b2e7a-107">**Примечание.** Максимальный срок действия подписки составляет 60 минут. Однако подписки можно продлевать, пока у вызывающий не получит разрешения на доступ к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-107">**Note:** The maximum time a subscription can last is 60 minutes; however, subscriptions can be renewed until the caller has permissions to access to resource.</span></span>

## <a name="change-notification-types"></a><span data-ttu-id="b2e7a-108">Типы уведомлений об изменениях</span><span class="sxs-lookup"><span data-stu-id="b2e7a-108">Change notification types</span></span>
<span data-ttu-id="b2e7a-109">Microsoft Teams поддерживает два типа уведомлений об изменениях:</span><span class="sxs-lookup"><span data-stu-id="b2e7a-109">Microsoft Teams supports two types of change notifications:</span></span>
- <span data-ttu-id="b2e7a-110">**Уведомление об изменении для отслеживания всех изменений, связанных с ресурсом в клиенте**. Например, вы можете подписаться на изменения сообщений любого канала в клиенте и получать уведомления при создании, обновлении или удалении сообщения в любом канале в клиенте.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-110">**Change notification to track all changes related to a resource across the tenant** - for example, you can subscribe to changes in messages in any channel across the tenant and get notified whenever a message is created, updated, or deleted in any channel in the tenant.</span></span>
- <span data-ttu-id="b2e7a-111">**Уведомление об изменении для отслеживания всех изменений определенного ресурса**. Например, вы можете подписаться на изменения сообщений определенного канала и получать уведомления при создании, обновлении или удалении сообщения в этом канале.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-111">**Change notification to track all changes for a specific resource** - for example, you can subscribe to changes in messages in a particular channel and get notified whenever a message is created, updated, or deleted in that channel.</span></span>

<span data-ttu-id="b2e7a-112">Дополнительные сведения о том, какие ресурсы поддерживают определенные типы уведомлений об изменениях, см. в статье [Уведомления об изменениях Microsoft Graph](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="b2e7a-112">For details about which resources support which types of change notifications, see [Microsoft Graph change notifications](webhooks.md).</span></span>
 

## <a name="notification-payloads"></a><span data-ttu-id="b2e7a-113">Полезные данные уведомлений</span><span class="sxs-lookup"><span data-stu-id="b2e7a-113">Notification payloads</span></span>

<span data-ttu-id="b2e7a-114">В зависимости от вашей подписки вы можете получать уведомление с данными ресурсов или без них.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-114">Depending on your subscription, you can either get the notification with resource data, or without resource data.</span></span> <span data-ttu-id="b2e7a-115">Подписка с данными ресурсов позволяет получать полезные данные сообщения вместе с уведомлением, что устраняет необходимость обратного вызова и получения содержимого.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-115">Subscribing with resource data allows you to get the message payload along with the notification, which removes the need to call back and get the content.</span></span>

### <a name="notifications-with-resource-data"></a><span data-ttu-id="b2e7a-116">Уведомления с данными ресурсов</span><span class="sxs-lookup"><span data-stu-id="b2e7a-116">Notifications with resource data</span></span>

<span data-ttu-id="b2e7a-117">Для уведомлений с данными ресурсов полезные данные выглядят следующим образом.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-117">For notifications with resource data, the payload looks like the following.</span></span>  <span data-ttu-id="b2e7a-118">Эти полезные данные предназначены для уведомления, соответствующего ресурсу сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-118">This payload is for a notification corresponding to the chat message resource.</span></span> <span data-ttu-id="b2e7a-119">Фактическое уведомление включает свойства **resource** и **resourceData**, представляющие ресурс, который вызвал уведомление.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-119">The actual notification includes the **resource** and **resourceData** properties, which represent the resource that has triggered the notification.</span></span>

```json
{
    "value": [{
        "subscriptionId": "10493aa0-4d29-4df5-bc0c-ef742cc6cd7f",
        "changeType": "created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-02-02T10:30:34.9097561-08:00",
        "resource": "chats('19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces')/messages('1612289765949')",
        "resourceData": {
            "id": "1612289765949",
            "@odata.type": "#Microsoft.Graph.chatMessage",
            "@odata.id": "chats('19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces')/messages('1612289765949')"
        },
        "encryptedContent": {
            "data": "<<--EncryptedContent-->",
            "dataKey": "<<--EnryptedDataKeyUsedForEncryptingContent-->>",
            "encryptionCertificateId": "<<--IdOfTheCertificateUsedForEncryptingDataKey-->>",
            "encryptionCertificateThumbprint": "<<--ThumbprintOfTheCertificateUsedForEncryptingDataKey-->>"
        },
        "tenantId": "<<--TenantForWhichNotificationWasSent-->>"
    }],
    "validationTokens": ["<<--ValidationTokens-->>"]
}
```

<span data-ttu-id="b2e7a-120">Дополнительные сведения о проверке маркеров и расшифровке полезных данных см. в статье [Настройка уведомлений об изменениях, включающих данные ресурсов](webhooks-with-resource-data.md).</span><span class="sxs-lookup"><span data-stu-id="b2e7a-120">For details about how to validate tokens and decrypt the payload, see [Set up change notifications that include resource data](webhooks-with-resource-data.md).</span></span>

<span data-ttu-id="b2e7a-121">Расшифрованные полезные данные уведомления выглядят следующим образом.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-121">The decrypted notification payload looks like the following.</span></span> <span data-ttu-id="b2e7a-122">Расшифрованные полезные данные в предыдущем примере соответствуют схеме [chatMessage](/graph/api/resources/chatMessage?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="b2e7a-122">The decrypted payload for the previous example conforms to the [chatMessage](/graph/api/resources/chatMessage?preserve-view=true) schema.</span></span> <span data-ttu-id="b2e7a-123">Полезные данные похожи на результаты, возвращаемые операциями GET.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-123">The payload is similar to that returned by GET operations.</span></span>

```json
{
  "id": "1612289992105",
  "replyToId": null,
  "etag": "1612289992105",
  "messageType": "message",
  "createdDateTime": "2021-02-02T18:19:52Z",
  "lastModifiedDateTime": "2021-02-02T18:19:52.105Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": "19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces",
  "importance": "normal",
  "locale": "en-us",
  "webUrl": null,
  "from": {
    "application": null,
    "device": null,
    "user": {
      "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
      "displayName": "Ramjot Singh",
      "userIdentityType": "aadUser"
    },
    "conversation": null
  },
  "body": {
    "contentType": "text",
    "content": "test"
  },
  "channelIdentity": null,
  "attachments": [],
  "mentions": [],
  "policyViolation": null,
  "reactions": [],
  "replies": [],
  "hostedContents": []
}
```

### <a name="notifications-without-resource-data"></a><span data-ttu-id="b2e7a-124">Уведомления без данных ресурса</span><span class="sxs-lookup"><span data-stu-id="b2e7a-124">Notifications without resource data</span></span>

<span data-ttu-id="b2e7a-125">Уведомления без данных ресурса предоставляют достаточно сведений, чтобы выполнить вызов GET для получения ресурса.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-125">Notifications without resource data give you enough information to make GET calls to get the resource.</span></span> <span data-ttu-id="b2e7a-126">Для подписок на уведомления без данных ресурса не требуется сертификат шифрования (так как фактические данные ресурса не передаются).</span><span class="sxs-lookup"><span data-stu-id="b2e7a-126">Subscriptions for notifications without resource data don't require an encryption certificate (because actual resource data is not sent over).</span></span>

<span data-ttu-id="b2e7a-127">Полезные данные выглядят следующим образом.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-127">The payload looks like the following.</span></span> <span data-ttu-id="b2e7a-128">Это полезные данные для сообщения, отправленного в канале.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-128">This payload is for a message sent in a channel.</span></span>

```json
{
  "subscriptionId": "9f9d1ed0-c9cc-42e7-8d80-a7fc4b0cda3c",
  "changeType": "created",
  "tenantId": "<<--TenantForWhichNotificationWasSent-->>",  
  "clientState": "<<--SpecifiedClientState-->>",
  "subscriptionExpirationDateTime": "2021-02-02T11:26:41.0537895-08:00",
  "resource": "teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2')/messages('1612293113399')",
  "resourceData": {
    "id": "1612293113399",
    "@odata.type": "#Microsoft.Graph.chatMessage",
    "@odata.id": "teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2')/messages('1612293113399')"
  }
}
```
<span data-ttu-id="b2e7a-129">В примере выше показано уведомление, соответствующее ресурсу сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-129">Previous example above shows a notification that corresponds to a chat message resource.</span></span> <span data-ttu-id="b2e7a-130">Фактическое уведомление включает свойства **resource** и **resourceData**, представляющие ресурс, который вызвал уведомление.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-130">The actual notification includes the **resource** and **resourceData** properties, which represent the resource that has triggered the notification.</span></span> <span data-ttu-id="b2e7a-131">Свойства **resource** и **@odata.id** можно использовать для вызовов в Microsoft Graph, чтобы получить полезные данные ресурса.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-131">The **resource** and **@odata.id** properties can be used to make calls to Microsoft Graph to get the payload of the resource.</span></span>

> <span data-ttu-id="b2e7a-132">**Примечание**. Вызовы GET всегда возвращают текущее состояние ресурса.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-132">**Note** GET calls will always return the current state of the resource.</span></span> <span data-ttu-id="b2e7a-133">Если ресурс изменяется с момента отправки уведомления и до его получения, операция возвращает обновленный ресурс.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-133">If the resource is changed between when the notification is sent and when the resource is retrieved, the operation will return the updated resource.</span></span>

## <a name="see-also"></a><span data-ttu-id="b2e7a-134">См. также</span><span class="sxs-lookup"><span data-stu-id="b2e7a-134">See also</span></span>
- [<span data-ttu-id="b2e7a-135">Уведомления об изменениях в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b2e7a-135">Microsoft Graph change notifications</span></span>](webhooks.md)
- [<span data-ttu-id="b2e7a-136">Обзор API Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="b2e7a-136">Microsoft Teams API overview</span></span>](teams-concept-overview.md)
