---
title: Получение уведомлений об изменениях чатов с помощью Microsoft Graph
description: Узнайте, как получать уведомления об изменениях (создание и обновление) чатов с помощью API Microsoft Graph.
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 246a0236b705f98835a4c8131a04e28d3d8c846c
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/10/2021
ms.locfileid: "53367035"
---
# <a name="get-change-notifications-for-chats-using-microsoft-graph"></a><span data-ttu-id="74c71-103">Получение уведомлений об изменениях чатов с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="74c71-103">Get change notifications for chats using Microsoft Graph</span></span>

<span data-ttu-id="74c71-104">Уведомления об изменениях позволяют подписаться на изменения (создание и обновление) чатов.</span><span class="sxs-lookup"><span data-stu-id="74c71-104">Change notifications enable you to subscribe to changes (create and update) to chats.</span></span> <span data-ttu-id="74c71-105">Вы можете получать уведомления при создании или обновлении чата.</span><span class="sxs-lookup"><span data-stu-id="74c71-105">You can get notified whenever a chat is created or updated.</span></span> <span data-ttu-id="74c71-106">Кроме того, вы можете получать данные ресурсов в уведомлениях и, следовательно, избегать вызова API, чтобы получить полезные данные.</span><span class="sxs-lookup"><span data-stu-id="74c71-106">You can also get the resource data in the notifications and therefore avoid calling the API to get the payload.</span></span>

## <a name="subscribe-to-changes-in-any-chat-at-tenant-level"></a><span data-ttu-id="74c71-107">Подписка на изменения в любом чате на уровне клиента</span><span class="sxs-lookup"><span data-stu-id="74c71-107">Subscribe to changes in any chat at tenant level</span></span>

<span data-ttu-id="74c71-108">Чтобы получать уведомления обо всех изменениях (создание и обновление), связанных с любым чатом в клиенте, подпишитесь на `/chats`.</span><span class="sxs-lookup"><span data-stu-id="74c71-108">To get change notifications for all changes (create and update) related to any chat in a tenant, subscribe to `/chats`.</span></span> <span data-ttu-id="74c71-109">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.</span><span class="sxs-lookup"><span data-stu-id="74c71-109">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

### <a name="permissions"></a><span data-ttu-id="74c71-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="74c71-110">Permissions</span></span>

|<span data-ttu-id="74c71-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74c71-111">Permission type</span></span>      | <span data-ttu-id="74c71-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="74c71-112">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="74c71-113">Поддерживаемые версии</span><span class="sxs-lookup"><span data-stu-id="74c71-113">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="74c71-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74c71-114">Delegated (work or school account)</span></span> | <span data-ttu-id="74c71-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74c71-115">Not supported.</span></span> | <span data-ttu-id="74c71-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74c71-116">Not supported.</span></span> |
|<span data-ttu-id="74c71-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74c71-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74c71-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74c71-118">Not supported.</span></span>    | <span data-ttu-id="74c71-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74c71-119">Not supported.</span></span> |
|<span data-ttu-id="74c71-120">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="74c71-120">Application</span></span> | <span data-ttu-id="74c71-121">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74c71-121">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span>   | <span data-ttu-id="74c71-122">бета</span><span class="sxs-lookup"><span data-stu-id="74c71-122">beta</span></span>|

### <a name="example"></a><span data-ttu-id="74c71-123">Пример</span><span class="sxs-lookup"><span data-stu-id="74c71-123">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-changes-in-a-particular-chat"></a><span data-ttu-id="74c71-124">Подписка на изменения в определенном чате</span><span class="sxs-lookup"><span data-stu-id="74c71-124">Subscribe to changes in a particular chat</span></span>


<span data-ttu-id="74c71-125">Чтобы получать уведомления обо всех изменениях, связанных с определенным чатом, подпишитесь на `/chats/{id}`.</span><span class="sxs-lookup"><span data-stu-id="74c71-125">To get change notifications for all changes related to a particular chat, subscribe to `/chats/{id}`.</span></span> <span data-ttu-id="74c71-126">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.</span><span class="sxs-lookup"><span data-stu-id="74c71-126">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

### <a name="permissions"></a><span data-ttu-id="74c71-127">Разрешения</span><span class="sxs-lookup"><span data-stu-id="74c71-127">Permissions</span></span>

|<span data-ttu-id="74c71-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74c71-128">Permission type</span></span>      | <span data-ttu-id="74c71-129">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="74c71-129">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="74c71-130">Поддерживаемые версии</span><span class="sxs-lookup"><span data-stu-id="74c71-130">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="74c71-131">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74c71-131">Delegated (work or school account)</span></span> | <span data-ttu-id="74c71-132">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="74c71-132">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="74c71-133">Бета</span><span class="sxs-lookup"><span data-stu-id="74c71-133">beta</span></span> |
|<span data-ttu-id="74c71-134">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74c71-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74c71-135">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74c71-135">Not supported.</span></span>    | <span data-ttu-id="74c71-136">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74c71-136">Not supported.</span></span> |
|<span data-ttu-id="74c71-137">Приложение</span><span class="sxs-lookup"><span data-stu-id="74c71-137">Application</span></span> | <span data-ttu-id="74c71-138">ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat\*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74c71-138">ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat\*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> | <span data-ttu-id="74c71-139">Бета</span><span class="sxs-lookup"><span data-stu-id="74c71-139">beta</span></span> |

> <span data-ttu-id="74c71-140">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="74c71-140">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="example"></a><span data-ttu-id="74c71-141">Пример</span><span class="sxs-lookup"><span data-stu-id="74c71-141">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{id}",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```


### <a name="notifications-with-resource-data"></a><span data-ttu-id="74c71-142">Уведомления с данными ресурсов</span><span class="sxs-lookup"><span data-stu-id="74c71-142">Notifications with resource data</span></span>

<span data-ttu-id="74c71-143">Для уведомлений с данными ресурсов полезные данные выглядят следующим образом.</span><span class="sxs-lookup"><span data-stu-id="74c71-143">For notifications with resource data, the payload looks like the following.</span></span> <span data-ttu-id="74c71-144">Эти полезные данные относятся к изменению свойства в чате.</span><span class="sxs-lookup"><span data-stu-id="74c71-144">This payload is for a property change in a chat.</span></span>

```json
{
    "value": [{
        "subscriptionId": "352887e3-9be0-4b6f-a4e6-dec118d857db",
        "changeType": "Created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-06-03T09:50:37.719033+00:00",
        "resource": "chats('19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces')",
        "resourceData": {
            "id": "19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces",
            "@odata.type": "#microsoft.graph.chat",
            "@odata.id": "chats('19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces')"
        },
        "EncryptedContent": {
            "data": "<<--EncryptedContent-->>",
            "dataKey": "<<--EnryptedDataKeyUsedForEncryptingContent-->>",
            "encryptionCertificateId": "<<--IdOfTheCertificateUsedForEncryptingDataKey-->>",
            "encryptionCertificateThumbprint": "<<--ThumbprintOfTheCertificateUsedForEncryptingDataKey-->>"
        }
            "tenantId": "<<--TenantForWhichNotificationWasSent-->>"
        }],
    "validationTokens": ["<<--ValidationTokens-->>"]
}
```

<span data-ttu-id="74c71-145">Дополнительные сведения о проверке маркеров и расшифровке полезных данных см. в статье [Настройка уведомлений об изменениях, включающих данные ресурсов](webhooks-with-resource-data.md).</span><span class="sxs-lookup"><span data-stu-id="74c71-145">For details about how to validate tokens and decrypt the payload, see [Set up change notifications that include resource data](webhooks-with-resource-data.md).</span></span>

<span data-ttu-id="74c71-146">Расшифрованные полезные данные уведомления выглядят следующим образом.</span><span class="sxs-lookup"><span data-stu-id="74c71-146">The decrypted notification payload looks like the following.</span></span> <span data-ttu-id="74c71-147">Полезные данные соответствуют схеме [chats](/graph/api/resources/chat?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="74c71-147">The payload conforms to the [chats](/graph/api/resources/chat?preserve-view=true) schema.</span></span> <span data-ttu-id="74c71-148">Полезные данные похожи на результаты, возвращаемые операциями GET.</span><span class="sxs-lookup"><span data-stu-id="74c71-148">The payload is similar to that returned by GET operations.</span></span>

```json
{
  "id": "19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces",
  "topic": null,
  "createdDateTime": "2021-06-03T14:25:04+05:30",
  "lastUpdatedDateTime": "2021-06-03T14:25:04.387Z",
  "chatType": "oneOnOne",
  "members": [
    {
      "userId": "976f4b31-fd01-4e0b-9178-29cc40c14438",
      "email": null,
      "tenantId": "2432b57b-0abd-43db-aa7b-16eadd115d34",
      "id": "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOToxMjczYTAxNi0yMDFkLTRmOTUtODA4My0xYjdmOTliM2VkZWJfOTc2ZjRiMzEtZmQwMS00ZTBiLTkxNzgtMjljYzQwYzE0NDM4QHVucS5nYmwuc3BhY2VzIyM5NzZmNGIzMS1mZDAxLTRlMGItOTE3OC0yOWNjNDBjMTQ0Mzg=",
      "roles": [],
      "displayName": null,
      "visibleHistoryStartDateTime": "1970-01-01T00:00:00Z",
      "user": null
    },
    {
      "userId": "ee723d3d-22d0-4394-9c32-5764d68f4672",
      "email": null,
      "tenantId": "2432b57b-0abd-43db-aa7b-16eadd115d34",
      "id": "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOToxMjczYTAxNi0yMDFkLTRmOTUtODA4My0xYjdmOTliM2VkZWJfOTc2ZjRiMzEtZmQwMS00ZTBiLTkxNzgtMjljYzQwYzE0NDM4QHVucS5nYmwuc3BhY2VzIyNlZTcyM2QzZC0yMmQwLTQzOTQtOWMzMi01NzY0ZDY4ZjQ2NzI=",
      "roles": [],
      "displayName": null,
      "visibleHistoryStartDateTime": "1970-01-01T00:00:00Z",
      "user": null
    }
  ],
  "messages": [],
  "installedApps": [],
  "tabs": [],
  "permissionGrants": [],
  "operations": []
}
```

### <a name="notifications-without-resource-data"></a><span data-ttu-id="74c71-149">Уведомления без данных о ресурсах</span><span class="sxs-lookup"><span data-stu-id="74c71-149">Notifications without resource data</span></span>

<span data-ttu-id="74c71-150">Следующие полезные данные описывают сведения, отправляемые в запросе на уведомления без данных ресурса.</span><span class="sxs-lookup"><span data-stu-id="74c71-150">The following payload describes the information sent in the request for notifications without resource data.</span></span> <span data-ttu-id="74c71-151">Эти конкретные полезные данные означают, что создан новый чат.</span><span class="sxs-lookup"><span data-stu-id="74c71-151">This particular payload signifies that a new chat has been created.</span></span>

```json
{
    "subscriptionId": "8d85051d-779d-45bc-be92-e433f0a5d8ac",
    "changeType": "Created",
    "tenantId": "<<--TenantForWhichNotificationWasSent-->>",
    "clientState": "<<--SpecifiedClientState-->>",
    "subscriptionExpirationDateTime": "2021-06-03T10:26:09.8959595+00:00",
    "resource": "chats('19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces')",
    "resourceData": {
        "id": "19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces",
        "@odata.type": "#microsoft.graph.chat",
        "@odata.id": "chats('19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces')"
    }
}
```

<span data-ttu-id="74c71-152">Свойства **resource** и **@odata.id** можно использовать для вызовов в Microsoft Graph, чтобы получить полезные данные сведений о чате.</span><span class="sxs-lookup"><span data-stu-id="74c71-152">The **resource** and **@odata.id** properties can be used to make calls to Microsoft Graph to get the payload for the chat details.</span></span> <span data-ttu-id="74c71-153">Вызовы GET всегда возвращают текущее состояние сведений о чате.</span><span class="sxs-lookup"><span data-stu-id="74c71-153">GET calls will always return the current state of the chat details.</span></span> <span data-ttu-id="74c71-154">Если сведения о чате обновились после отправки уведомления и до получения сведений о чате, операция возвращает обновленные сведения о чате.</span><span class="sxs-lookup"><span data-stu-id="74c71-154">If the chat details were updated between when the notification is sent and when the chat details were retrieved, the operation will return the updated chat details.</span></span>

## <a name="see-also"></a><span data-ttu-id="74c71-155">См. также</span><span class="sxs-lookup"><span data-stu-id="74c71-155">See also</span></span>
- [<span data-ttu-id="74c71-156">Уведомления об изменениях в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="74c71-156">Microsoft Graph change notifications</span></span>](webhooks.md)
- [<span data-ttu-id="74c71-157">Обзор API Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="74c71-157">Microsoft Teams API overview</span></span>](teams-concept-overview.md)