---
title: Получение уведомлений об изменениях участников чата с помощью Microsoft Graph
description: Узнайте, как получать уведомления об изменениях участников чата с помощью API Microsoft Graph.
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: aa8fa5ddea9c8e0df8eb8bf81558840392bdd306
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/10/2021
ms.locfileid: "53367029"
---
# <a name="get-change-notifications-for-chat-membership-using-microsoft-graph"></a><span data-ttu-id="2c315-103">Получение уведомлений об изменениях участников чата с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2c315-103">Get change notifications for chat membership using Microsoft Graph</span></span>

<span data-ttu-id="2c315-104">Уведомления об изменениях позволяют подписаться на изменения (создание и удаление) участников чатов.</span><span class="sxs-lookup"><span data-stu-id="2c315-104">Change notifications enable you to subscribe to changes (create and delete) in chats membership.</span></span> <span data-ttu-id="2c315-105">Вы можете получать уведомления при добавлении или удалении участника из чата.</span><span class="sxs-lookup"><span data-stu-id="2c315-105">You can get notified whenever a member is added or removed from a chat.</span></span> <span data-ttu-id="2c315-106">Кроме того, вы можете получать данные ресурсов в уведомлениях и, следовательно, избегать вызова API, чтобы получить полезные данные.</span><span class="sxs-lookup"><span data-stu-id="2c315-106">You can also get the resource data in the notifications and therefore avoid calling the API to get the payload.</span></span>

## <a name="subscribe-to-changes-in-membership-of-any-chat-at-tenant-level"></a><span data-ttu-id="2c315-107">Подписка на изменения участников любого чата на уровне клиента</span><span class="sxs-lookup"><span data-stu-id="2c315-107">Subscribe to changes in membership of any chat at tenant level</span></span>

<span data-ttu-id="2c315-108">Чтобы получать уведомления об изменениях участников любого чата в клиенте, подпишитесь на `/chats/getAllMembers`.</span><span class="sxs-lookup"><span data-stu-id="2c315-108">To get change notifications for membership changes in any chat across the tenant, subscribe to `/chats/getAllMembers`.</span></span> <span data-ttu-id="2c315-109">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.</span><span class="sxs-lookup"><span data-stu-id="2c315-109">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

### <a name="permissions"></a><span data-ttu-id="2c315-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2c315-110">Permissions</span></span>

|<span data-ttu-id="2c315-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c315-111">Permission type</span></span>      | <span data-ttu-id="2c315-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c315-112">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="2c315-113">Поддерживаемые версии</span><span class="sxs-lookup"><span data-stu-id="2c315-113">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="2c315-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c315-114">Delegated (work or school account)</span></span> | <span data-ttu-id="2c315-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c315-115">Not supported.</span></span> | <span data-ttu-id="2c315-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c315-116">Not supported.</span></span> |
|<span data-ttu-id="2c315-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c315-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c315-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c315-118">Not supported.</span></span>    | <span data-ttu-id="2c315-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c315-119">Not supported.</span></span> |
|<span data-ttu-id="2c315-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2c315-120">Application</span></span> | <span data-ttu-id="2c315-121">ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c315-121">ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span>  | <span data-ttu-id="2c315-122">бета</span><span class="sxs-lookup"><span data-stu-id="2c315-122">beta</span></span>|

### <a name="example"></a><span data-ttu-id="2c315-123">Пример</span><span class="sxs-lookup"><span data-stu-id="2c315-123">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,deleted",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/getAllMembers",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-changes-in-membership-of-a-particular-chat"></a><span data-ttu-id="2c315-124">Подписка на изменения участников определенного чата</span><span class="sxs-lookup"><span data-stu-id="2c315-124">Subscribe to changes in membership of a particular chat</span></span>

<span data-ttu-id="2c315-125">Чтобы получать уведомления об изменениях участников определенного чата, подпишитесь на `/chats/{id}/members`.</span><span class="sxs-lookup"><span data-stu-id="2c315-125">To get change notifications for membership changes in a particular chat, subscribe to `/chats/{id}/members`.</span></span> <span data-ttu-id="2c315-126">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.</span><span class="sxs-lookup"><span data-stu-id="2c315-126">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

### <a name="permissions"></a><span data-ttu-id="2c315-127">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2c315-127">Permissions</span></span>

|<span data-ttu-id="2c315-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c315-128">Permission type</span></span>      | <span data-ttu-id="2c315-129">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c315-129">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="2c315-130">Поддерживаемые версии</span><span class="sxs-lookup"><span data-stu-id="2c315-130">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="2c315-131">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c315-131">Delegated (work or school account)</span></span> | <span data-ttu-id="2c315-132">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2c315-132">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="2c315-133">Бета</span><span class="sxs-lookup"><span data-stu-id="2c315-133">beta</span></span> |
|<span data-ttu-id="2c315-134">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c315-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c315-135">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c315-135">Not supported.</span></span>    | <span data-ttu-id="2c315-136">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c315-136">Not supported.</span></span> |
|<span data-ttu-id="2c315-137">Приложение</span><span class="sxs-lookup"><span data-stu-id="2c315-137">Application</span></span> | <span data-ttu-id="2c315-138">ChatMember.Read.Chat *, Chat.Manage.Chat*, ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c315-138">ChatMember.Read.Chat *, Chat.Manage.Chat*, ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span>  | <span data-ttu-id="2c315-139">Бета</span><span class="sxs-lookup"><span data-stu-id="2c315-139">beta</span></span> |

> <span data-ttu-id="2c315-140">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="2c315-140">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="example"></a><span data-ttu-id="2c315-141">Пример</span><span class="sxs-lookup"><span data-stu-id="2c315-141">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,deleted",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{id}/members",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```



### <a name="notifications-with-resource-data"></a><span data-ttu-id="2c315-142">Уведомления с данными ресурсов</span><span class="sxs-lookup"><span data-stu-id="2c315-142">Notifications with resource data</span></span>

<span data-ttu-id="2c315-143">Для уведомлений с данными ресурсов полезные данные выглядят следующим образом.</span><span class="sxs-lookup"><span data-stu-id="2c315-143">For notifications with resource data, the payload looks like the following.</span></span> <span data-ttu-id="2c315-144">Эти полезные данные относятся к изменению участников в чате.</span><span class="sxs-lookup"><span data-stu-id="2c315-144">This payload is for a membership change in a chat.</span></span>

```json
{
    "value": [{
        "subscriptionId": "c0125ef2-7a87-4e94-aa71-b995510f369b",
        "changeType": "Created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-06-03T11:04:58.5537601+00:00",
        "resource": "chats('19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces')/members('MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOToxMjczYTAxNi0yMDFkLTRmOTUtODA4My0xYjdmOTliM2VkZWJfOTc2ZjRiMzEtZmQwMS00ZTBiLTkxNzgtMjljYzQwYzE0NDM4QHVucS5nYmwuc3BhY2VzIyMyZmM2MDY2My0xOWEyLTRhYTQtODUyYy1mN2JhNGU5MGFkYTI=')",
        "resourceData": {
            "id": "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOToxMjczYTAxNi0yMDFkLTRmOTUtODA4My0xYjdmOTliM2VkZWJfOTc2ZjRiMzEtZmQwMS00ZTBiLTkxNzgtMjljYzQwYzE0NDM4QHVucS5nYmwuc3BhY2VzIyMyZmM2MDY2My0xOWEyLTRhYTQtODUyYy1mN2JhNGU5MGFkYTI=",
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "@odata.id": "chats('19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces')/members('MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOToxMjczYTAxNi0yMDFkLTRmOTUtODA4My0xYjdmOTliM2VkZWJfOTc2ZjRiMzEtZmQwMS00ZTBiLTkxNzgtMjljYzQwYzE0NDM4QHVucS5nYmwuc3BhY2VzIyMyZmM2MDY2My0xOWEyLTRhYTQtODUyYy1mN2JhNGU5MGFkYTI=')"
        },
        "EncryptedContent": {
            "data": "<<--EncryptedContent-->>",
            "dataKey": "<<--EnryptedDataKeyUsedForEncryptingContent-->>",
            "encryptionCertificateId": "<<--IdOfTheCertificateUsedForEncryptingDataKey-->>",
            "encryptionCertificateThumbprint": "<<--ThumbprintOfTheCertificateUsedForEncryptingDataKey-->>"
        },
        "tenantId": "<<--TenantForWhichNotificationWasSent-->>"
    }],
    "validationTokens": ["<<--ValidationTokens-->>"]
}
```

<span data-ttu-id="2c315-145">Дополнительные сведения о проверке маркеров и расшифровке полезных данных см. в статье [Настройка уведомлений об изменениях, включающих данные ресурсов](webhooks-with-resource-data.md).</span><span class="sxs-lookup"><span data-stu-id="2c315-145">For details about how to validate tokens and decrypt the payload, see [Set up change notifications that include resource data](webhooks-with-resource-data.md).</span></span>

<span data-ttu-id="2c315-146">Расшифрованные полезные данные уведомления выглядят следующим образом.</span><span class="sxs-lookup"><span data-stu-id="2c315-146">The decrypted notification payload looks like the following.</span></span> <span data-ttu-id="2c315-147">Полезные данные соответствуют схеме [aaduserconversationmember](/graph/api/resources/aaduserconversationmember?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="2c315-147">The payload conforms to the [aaduserconversationmember](/graph/api/resources/aaduserconversationmember?preserve-view=true) schema.</span></span> <span data-ttu-id="2c315-148">Полезные данные похожи на результаты, возвращаемые операциями GET.</span><span class="sxs-lookup"><span data-stu-id="2c315-148">The payload is similar to that returned by GET operations.</span></span>

```json
{
    "userId": "2fc60663-19a2-4aa4-852c-f7ba4e90ada2",
    "email": null,
    "tenantId": "2432b57b-0abd-43db-aa7b-16eadd115d34",
    "id": "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOToxMjczYTAxNi0yMDFkLTRmOTUtODA4My0xYjdmOTliM2VkZWJfOTc2ZjRiMzEtZmQwMS00ZTBiLTkxNzgtMjljYzQwYzE0NDM4QHVucS5nYmwuc3BhY2VzIyMyZmM2MDY2My0xOWEyLTRhYTQtODUyYy1mN2JhNGU5MGFkYTI=",
    "roles": [
    "Owner"
    ],
    "displayName": null,
    "visibleHistoryStartDateTime": "1970-01-01T00:00:00Z",
    "user": null
}
```

### <a name="notifications-without-resource-data"></a><span data-ttu-id="2c315-149">Уведомления без данных о ресурсах</span><span class="sxs-lookup"><span data-stu-id="2c315-149">Notifications without resource data</span></span>

<span data-ttu-id="2c315-150">Следующие полезные данные описывают сведения, отправляемые в запросе на уведомления без данных ресурса.</span><span class="sxs-lookup"><span data-stu-id="2c315-150">The following payload describes the information sent in the request for notifications without resource data.</span></span> <span data-ttu-id="2c315-151">Эти конкретные полезные данные означают, что пользователь добавлен в чат.</span><span class="sxs-lookup"><span data-stu-id="2c315-151">This particular payload signifies that a user has been added to a chat.</span></span>

```json
{
    "subscriptionId": "cae901f1-ad1d-41b1-95b7-37029ed327bf",
    "changeType": "Created",
    "tenantId": "<<--TenantForWhichNotificationWasSent-->>",
    "clientState": "<<--SpecifiedClientState-->>",
    "subscriptionExpirationDateTime": "2021-06-03T10:58:54.7656077+00:00",
    "resource": "chats('19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces')/members('MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOToxMjczYTAxNi0yMDFkLTRmOTUtODA4My0xYjdmOTliM2VkZWJfOTc2ZjRiMzEtZmQwMS00ZTBiLTkxNzgtMjljYzQwYzE0NDM4QHVucS5nYmwuc3BhY2VzIyMyZmM2MDY2My0xOWEyLTRhYTQtODUyYy1mN2JhNGU5MGFkYTI=')",
    "resourceData": {
        "id": "MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOToxMjczYTAxNi0yMDFkLTRmOTUtODA4My0xYjdmOTliM2VkZWJfOTc2ZjRiMzEtZmQwMS00ZTBiLTkxNzgtMjljYzQwYzE0NDM4QHVucS5nYmwuc3BhY2VzIyMyZmM2MDY2My0xOWEyLTRhYTQtODUyYy1mN2JhNGU5MGFkYTI=",
        "@odata.type": "#microsoft.graph.aadUserConversationMember",
        "@odata.id": "chats('19:1273a016-201d-4f95-8083-1b7f99b3edeb_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces')/members('MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOToxMjczYTAxNi0yMDFkLTRmOTUtODA4My0xYjdmOTliM2VkZWJfOTc2ZjRiMzEtZmQwMS00ZTBiLTkxNzgtMjljYzQwYzE0NDM4QHVucS5nYmwuc3BhY2VzIyMyZmM2MDY2My0xOWEyLTRhYTQtODUyYy1mN2JhNGU5MGFkYTI=')"
    }
}
```

<span data-ttu-id="2c315-152">Свойства **resource** и **@odata.id** можно использовать для вызовов в Microsoft Graph, чтобы получить полезные данные сведений об участнике чата.</span><span class="sxs-lookup"><span data-stu-id="2c315-152">The **resource** and **@odata.id** properties can be used to make calls to Microsoft Graph to get the payload for the chat member details.</span></span> <span data-ttu-id="2c315-153">Вызовы GET всегда возвращают текущее состояние сведений об участнике чата.</span><span class="sxs-lookup"><span data-stu-id="2c315-153">GET calls will always return the current state of the chat member details.</span></span> <span data-ttu-id="2c315-154">Если сведения об участнике чата изменились после отправки уведомления и до получения сведений об участнике чата, операция возвращает обновленные сведения об участнике чата.</span><span class="sxs-lookup"><span data-stu-id="2c315-154">If the chat member details has changed between when the notification is sent and when the chat member details were retrieved, the operation will return the updated chat member details.</span></span>

## <a name="see-also"></a><span data-ttu-id="2c315-155">См. также</span><span class="sxs-lookup"><span data-stu-id="2c315-155">See also</span></span>
- [<span data-ttu-id="2c315-156">Уведомления об изменениях в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2c315-156">Microsoft Graph change notifications</span></span>](webhooks.md)
- [<span data-ttu-id="2c315-157">Обзор API Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="2c315-157">Microsoft Teams API overview</span></span>](teams-concept-overview.md)