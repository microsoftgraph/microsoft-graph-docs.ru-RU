---
title: Получение уведомлений об изменениях команд и каналов с помощью Microsoft Graph
description: Узнайте, как получать уведомления об изменениях (создание, обновление и удаление) команд и каналов с помощью API Microsoft Graph.
author: anandab
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 4d04333818fa57664664675feb4683465c4b63c6
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941562"
---
# <a name="get-change-notifications-for-teams-and-channels-using-microsoft-graph"></a><span data-ttu-id="9524d-103">Получение уведомлений об изменениях команд и каналов с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9524d-103">Get change notifications for teams and channels using Microsoft Graph</span></span>

<span data-ttu-id="9524d-104">Уведомления об изменениях позволяют подписаться на изменения (создание, обновление и удаление) команд и каналов.</span><span class="sxs-lookup"><span data-stu-id="9524d-104">Change notifications enable you to subscribe to changes (create, update, and delete) to teams and channels.</span></span> <span data-ttu-id="9524d-105">Вы можете получать уведомления при создании, обновлении и удалении команды или канала.</span><span class="sxs-lookup"><span data-stu-id="9524d-105">You can get notified whenever a team or channel is created, updated, or deleted.</span></span> <span data-ttu-id="9524d-106">Кроме того, вы можете получать данные ресурсов в уведомлениях и, следовательно, избегать вызова API, чтобы получить полезные данные.</span><span class="sxs-lookup"><span data-stu-id="9524d-106">You can also get the resource data in the notifications and therefore avoid calling the API to get the payload.</span></span>

## <a name="subscribe-to-changes-in-any-team-at-tenant-level"></a><span data-ttu-id="9524d-107">Подписка на изменения в любой команде на уровне клиента</span><span class="sxs-lookup"><span data-stu-id="9524d-107">Subscribe to changes in any team at tenant level</span></span>

<span data-ttu-id="9524d-108">Чтобы получать уведомления обо всех изменениях (создание, обновление и удаление), связанных с любой командой в клиенте, подпишитесь на `/teams`.</span><span class="sxs-lookup"><span data-stu-id="9524d-108">To get change notifications for all changes (create, update, and delete) related to any team in a tenant, subscribe to `/teams`.</span></span> <span data-ttu-id="9524d-109">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.</span><span class="sxs-lookup"><span data-stu-id="9524d-109">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

### <a name="permissions"></a><span data-ttu-id="9524d-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9524d-110">Permissions</span></span>

|<span data-ttu-id="9524d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9524d-111">Permission type</span></span>      | <span data-ttu-id="9524d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9524d-112">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="9524d-113">Поддерживаемые версии</span><span class="sxs-lookup"><span data-stu-id="9524d-113">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="9524d-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9524d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="9524d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9524d-115">Not supported.</span></span> | <span data-ttu-id="9524d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9524d-116">Not supported.</span></span> |
|<span data-ttu-id="9524d-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9524d-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9524d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9524d-118">Not supported.</span></span>    | <span data-ttu-id="9524d-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9524d-119">Not supported.</span></span> |
|<span data-ttu-id="9524d-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="9524d-120">Application</span></span> | <span data-ttu-id="9524d-121">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="9524d-121">Team.ReadBasic.All, TeamSettings.Read.All</span></span>   | <span data-ttu-id="9524d-122">бета</span><span class="sxs-lookup"><span data-stu-id="9524d-122">beta</span></span>|

### <a name="example"></a><span data-ttu-id="9524d-123">Пример</span><span class="sxs-lookup"><span data-stu-id="9524d-123">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-changes-in-a-particular-team"></a><span data-ttu-id="9524d-124">Подписка на изменения в определенной команде</span><span class="sxs-lookup"><span data-stu-id="9524d-124">Subscribe to changes in a particular team</span></span>


<span data-ttu-id="9524d-125">Чтобы получать уведомления обо всех изменениях, связанных с определенной командой в клиенте, подпишитесь на `/teams/{id}`.</span><span class="sxs-lookup"><span data-stu-id="9524d-125">To get change notifications for all changes related to a particular team in a tenant, subscribe to `/teams/{id}`.</span></span> <span data-ttu-id="9524d-126">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.</span><span class="sxs-lookup"><span data-stu-id="9524d-126">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

### <a name="permissions"></a><span data-ttu-id="9524d-127">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9524d-127">Permissions</span></span>

|<span data-ttu-id="9524d-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9524d-128">Permission type</span></span>      | <span data-ttu-id="9524d-129">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9524d-129">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="9524d-130">Поддерживаемые версии</span><span class="sxs-lookup"><span data-stu-id="9524d-130">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="9524d-131">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9524d-131">Delegated (work or school account)</span></span> | <span data-ttu-id="9524d-132">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="9524d-132">Team.ReadBasic.All, TeamSettings.Read.All</span></span> | <span data-ttu-id="9524d-133">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9524d-133">Not supported.</span></span> |
|<span data-ttu-id="9524d-134">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9524d-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9524d-135">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9524d-135">Not supported.</span></span>    | <span data-ttu-id="9524d-136">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9524d-136">Not supported.</span></span> |
|<span data-ttu-id="9524d-137">Приложение</span><span class="sxs-lookup"><span data-stu-id="9524d-137">Application</span></span> | <span data-ttu-id="9524d-138">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="9524d-138">Team.ReadBasic.All, TeamSettings.Read.All</span></span>    | <span data-ttu-id="9524d-139">бета</span><span class="sxs-lookup"><span data-stu-id="9524d-139">beta</span></span> |

### <a name="example"></a><span data-ttu-id="9524d-140">Пример</span><span class="sxs-lookup"><span data-stu-id="9524d-140">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```


## <a name="subscribe-to-changes-in-any-channel-at-tenant-level"></a><span data-ttu-id="9524d-141">Подписка на изменения в любом канале на уровне клиента</span><span class="sxs-lookup"><span data-stu-id="9524d-141">Subscribe to changes in any channel at tenant level</span></span>

<span data-ttu-id="9524d-142">Чтобы получать уведомления обо всех изменениях (создание, обновление и удаление), связанных с любым каналом в клиенте, подпишитесь на `/teams/getAllChannels`.</span><span class="sxs-lookup"><span data-stu-id="9524d-142">To get change notifications for all changes (create, update, and delete) related to any channel in a tenant, subscribe to `/teams/getAllChannels`.</span></span> <span data-ttu-id="9524d-143">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.</span><span class="sxs-lookup"><span data-stu-id="9524d-143">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

><span data-ttu-id="9524d-144">**Примечание.** Закрытые каналы не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="9524d-144">**Note:** Private channels aren't supported.</span></span>

### <a name="permissions"></a><span data-ttu-id="9524d-145">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9524d-145">Permissions</span></span>

|<span data-ttu-id="9524d-146">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9524d-146">Permission type</span></span>      | <span data-ttu-id="9524d-147">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9524d-147">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="9524d-148">Поддерживаемые версии</span><span class="sxs-lookup"><span data-stu-id="9524d-148">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="9524d-149">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9524d-149">Delegated (work or school account)</span></span> | <span data-ttu-id="9524d-150">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9524d-150">Not supported.</span></span> | <span data-ttu-id="9524d-151">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9524d-151">Not supported.</span></span> |
|<span data-ttu-id="9524d-152">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9524d-152">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9524d-153">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9524d-153">Not supported.</span></span>    | <span data-ttu-id="9524d-154">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9524d-154">Not supported.</span></span> |
|<span data-ttu-id="9524d-155">Приложение</span><span class="sxs-lookup"><span data-stu-id="9524d-155">Application</span></span> | <span data-ttu-id="9524d-156">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="9524d-156">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span> | <span data-ttu-id="9524d-157">бета</span><span class="sxs-lookup"><span data-stu-id="9524d-157">beta</span></span> |

### <a name="example"></a><span data-ttu-id="9524d-158">Пример</span><span class="sxs-lookup"><span data-stu-id="9524d-158">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/getAllChannels",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-changes-in-any-channel-of-a-particular-team"></a><span data-ttu-id="9524d-159">Подписка на изменения в любом канале определенной команды</span><span class="sxs-lookup"><span data-stu-id="9524d-159">Subscribe to changes in any channel of a particular team</span></span>


<span data-ttu-id="9524d-160">Чтобы получать уведомления обо всех изменениях, связанных с любым каналом в определенной команде, подпишитесь на `/teams/{id}/channels`.</span><span class="sxs-lookup"><span data-stu-id="9524d-160">To get change notifications for all changes related to any channel in a particular team, subscribe to `/teams/{id}/channels`.</span></span> <span data-ttu-id="9524d-161">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.</span><span class="sxs-lookup"><span data-stu-id="9524d-161">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

### <a name="permissions"></a><span data-ttu-id="9524d-162">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9524d-162">Permissions</span></span>

|<span data-ttu-id="9524d-163">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9524d-163">Permission type</span></span>      | <span data-ttu-id="9524d-164">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9524d-164">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="9524d-165">Поддерживаемые версии</span><span class="sxs-lookup"><span data-stu-id="9524d-165">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="9524d-166">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9524d-166">Delegated (work or school account)</span></span> | <span data-ttu-id="9524d-167">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="9524d-167">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span> | <span data-ttu-id="9524d-168">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9524d-168">Not supported.</span></span> |
|<span data-ttu-id="9524d-169">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9524d-169">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9524d-170">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9524d-170">Not supported.</span></span>    | <span data-ttu-id="9524d-171">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9524d-171">Not supported.</span></span> |
|<span data-ttu-id="9524d-172">Приложение</span><span class="sxs-lookup"><span data-stu-id="9524d-172">Application</span></span> | <span data-ttu-id="9524d-173">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="9524d-173">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>   | <span data-ttu-id="9524d-174">бета</span><span class="sxs-lookup"><span data-stu-id="9524d-174">beta</span></span> |

### <a name="example"></a><span data-ttu-id="9524d-175">Пример</span><span class="sxs-lookup"><span data-stu-id="9524d-175">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}/channels",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```


### <a name="notifications-with-resource-data"></a><span data-ttu-id="9524d-176">Уведомления с данными ресурсов</span><span class="sxs-lookup"><span data-stu-id="9524d-176">Notifications with resource data</span></span>

<span data-ttu-id="9524d-177">Для уведомлений с данными ресурсов полезные данные выглядят следующим образом.</span><span class="sxs-lookup"><span data-stu-id="9524d-177">For notifications with resource data, the payload looks like the following.</span></span> <span data-ttu-id="9524d-178">Эти полезные данные относятся к изменению свойства в команде.</span><span class="sxs-lookup"><span data-stu-id="9524d-178">This payload is for a property change in a team.</span></span>

```json
{
    "value": [{
        "subscriptionId": "10493aa0-4d29-4df5-bc0c-ef742cc6cd7f",
        "changeType": "created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-02-02T10:30:34.9097561-08:00",
        "resource": "teams('fb82c19a-0f6d-41ed-90f0-cbb29a476ede')",
        "resourceData": {
            "id": "1612289765949",
            "@odata.type": "#Microsoft.Graph.Team",
            "@odata.id": "teams('fb82c19a-0f6d-41ed-90f0-cbb29a476ede')"
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



<span data-ttu-id="9524d-179">Расшифрованные полезные данные уведомления выглядят следующим образом.</span><span class="sxs-lookup"><span data-stu-id="9524d-179">The decrypted notification payload looks like the following.</span></span> <span data-ttu-id="9524d-180">Полезные данные соответствуют схеме [teams](/graph/api/resources/team?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="9524d-180">The payload conforms to the [teams](/graph/api/resources/team?preserve-view=true) schema.</span></span> <span data-ttu-id="9524d-181">Полезные данные похожи на результаты, возвращаемые операциями GET.</span><span class="sxs-lookup"><span data-stu-id="9524d-181">The payload is similar to that returned by GET operations.</span></span>

><span data-ttu-id="9524d-182">**Примечание.** [discoverySettings](/graph/api/resources/teamdiscoverysettings?preserve-view=true) и [classSettings](/graph/api/resources/teamclasssettings?preserve-view=true) не предоставляются в полезных данных.</span><span class="sxs-lookup"><span data-stu-id="9524d-182">**Note:** [discoverySettings](/graph/api/resources/teamdiscoverysettings?preserve-view=true) and [classSettings](/graph/api/resources/teamclasssettings?preserve-view=true) aren't exposed in payload data.</span></span>

```json
{
  "id": "4c533ad3-e1dd-4277-a672-92ab64ed225c",
  "createdDateTime": "2021-03-18T10:31:14.597Z",
  "displayName": "Sample name",
  "description": "Sample description",
  "internalId": "19:2077546f765a42c1ba71236f4df70aa2@thread.tacv2",
  "specialization": "none",
  "visibility": "public",
  "webUrl": "https://teams.microsoft.com/l/team/19:2077546f724a42c1ba71236f4df79aa2%40thread.tacv2/conversations?groupId=4c533ad3-e1dd-4277-a672-92ab64ed225c&tenantId=0f2e8f59-862a-483b-9ca8-82a10665e17d",
  "isArchived": false,
  "isMembershipLimitedToOwners": false,
  "memberSettings": {
    "allowCreateUpdateChannels": true,
    "allowCreatePrivateChannels": true,
    "allowDeleteChannels": true,
    "allowAddRemoveApps": true,
    "allowCreateUpdateRemoveTabs": true,
    "allowCreateUpdateRemoveConnectors": true
  },
  "guestSettings": {
    "allowCreateUpdateChannels": false,
    "allowDeleteChannels": false
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true,
    "allowOwnerDeleteMessages": true,
    "allowTeamMentions": true,
    "allowChannelMentions": true
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "moderate",
    "allowStickersAndMemes": true,
    "allowCustomMemes": true
  }
}
```


<span data-ttu-id="9524d-183">Для уведомлений с данными ресурсов полезные данные выглядят следующим образом.</span><span class="sxs-lookup"><span data-stu-id="9524d-183">For notifications with resource data, the payload looks like the following.</span></span> <span data-ttu-id="9524d-184">Эти полезные данные относятся к изменению свойства в канале.</span><span class="sxs-lookup"><span data-stu-id="9524d-184">This payload is for a property change in a channel.</span></span>

```json
{
    "value": [{
        "subscriptionId": "10493aa0-4d29-4df5-bc0c-ef742cc6cd7f",
        "changeType": "created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-02-02T10:30:34.9097561-08:00",
        "resource": "teams('fb82c19a-0f6d-41ed-90f0-cbb29a476ede')/channels('19:01f39f5ac52f45fb9a7ce01cedd57b1f@thread.tacv2')",
        "resourceData": {
            "id": "19:01f39f5ac52f45fb9a7ce01cedd57b1f@thread.tacv2",
            "@odata.type": "#Microsoft.Graph.Channel",
            "@odata.id": "teams('fb82c19a-0f6d-41ed-90f0-cbb29a476ede')/channels('19:01f39f5ac52f45fb9a7ce01cedd57b1f@thread.tacv2')"
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
  

<span data-ttu-id="9524d-185">Расшифрованные полезные данные уведомления выглядят следующим образом.</span><span class="sxs-lookup"><span data-stu-id="9524d-185">The decrypted notification payload looks like the following.</span></span> <span data-ttu-id="9524d-186">Полезные данные соответствуют схеме [channel](/graph/api/resources/channel?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="9524d-186">The payload conforms to the [channel](/graph/api/resources/channel?preserve-view=true) schema.</span></span> <span data-ttu-id="9524d-187">Полезные данные похожи на результаты, возвращаемые операциями GET.</span><span class="sxs-lookup"><span data-stu-id="9524d-187">The payload is similar to that returned by GET operations.</span></span>

```json
{
  "id": "19:a3f841d969cd4ae0a7cbe847fc10b371@thread.tacv2",
  "createdDateTime": "2020-02-14T01:10:03.592Z",
  "displayName": "General",
  "description": "Sample Channel description",
  "isFavoriteByDefault": true,
  "email": "",
  "webUrl": "https://teams.microsoft.com/l/channel/19%3Aa3f841d969cd4ae0a7cbe847fc10b371%40thread.tacv2/General?groupId=7ed9bdab-9c7d-4c10-a25d-3f4ff0e34577&tenantId=0f2d8f49-862a-493b-9ca8-82a10637e17d",
  "membershipType": "standard",
  "moderationSettings": null
}
```


### <a name="notifications-without-resource-data"></a><span data-ttu-id="9524d-188">Уведомления без данных о ресурсах</span><span class="sxs-lookup"><span data-stu-id="9524d-188">Notifications without resource data</span></span>

<span data-ttu-id="9524d-189">Уведомления без данных о ресурсах предоставляют достаточно сведений, чтобы выполнить вызов GET для получения содержимого сообщения.</span><span class="sxs-lookup"><span data-stu-id="9524d-189">Notifications without resource data give you enough information to make GET calls to get the message content.</span></span> <span data-ttu-id="9524d-190">Для подписок на уведомления без данных ресурса не требуется сертификат шифрования (так как фактические данные ресурса не передаются).</span><span class="sxs-lookup"><span data-stu-id="9524d-190">Subscriptions for notifications without resource data don't require an encryption certificate (because actual resource data is not sent over).</span></span>

<span data-ttu-id="9524d-191">Для уведомлений без данных ресурса полезные данные выглядят следующим образом.</span><span class="sxs-lookup"><span data-stu-id="9524d-191">For notifications without resource data, the payload looks like the following.</span></span> <span data-ttu-id="9524d-192">Эти полезные данные относятся к изменению свойства в команде.</span><span class="sxs-lookup"><span data-stu-id="9524d-192">This payload is for a property change in a team.</span></span>

```json
{
  "subscriptionId": "9f9d1ed0-c9cc-42e7-8d80-a7fc4b0cda3c",
  "changeType": "created",
  "tenantId": "<<--TenantForWhichNotificationWasSent-->>",
  "clientState": "<<--SpecifiedClientState-->>",
  "subscriptionExpirationDateTime": "2021-02-02T11:26:41.0537895-08:00",
  "resource": "teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')",
  "resourceData": {
    "id": "1612293113399",
    "@odata.type": "#Microsoft.Graph.Teams",
    "@odata.id": "teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')"
  }
}
```

<span data-ttu-id="9524d-193">Свойства **resource** и **@odata.id** можно использовать для вызовов в Microsoft Graph, чтобы получить полезные данные для сообщения.</span><span class="sxs-lookup"><span data-stu-id="9524d-193">The **resource** and **@odata.id** properties can be used to make calls to Microsoft Graph to get the payload for the message.</span></span> <span data-ttu-id="9524d-194">Вызовы GET всегда возвращают текущее состояние сообщения.</span><span class="sxs-lookup"><span data-stu-id="9524d-194">GET calls will always return the current state of the message.</span></span> <span data-ttu-id="9524d-195">Если сообщение изменяется с момента отправки уведомления и до получения сообщения, операция возвращает обновленное сообщение.</span><span class="sxs-lookup"><span data-stu-id="9524d-195">If the message is changed between when the notification is sent and when the message is retrieved, the operation will return the updated message.</span></span>


><span data-ttu-id="9524d-196">**Примечание.** Адрес электронной почты канала не возвращается в полезных данных.</span><span class="sxs-lookup"><span data-stu-id="9524d-196">**Note:** Channel email address isn't returned in the payload.</span></span>

<span data-ttu-id="9524d-197">Для уведомлений без данных ресурса полезные данные выглядят следующим образом.</span><span class="sxs-lookup"><span data-stu-id="9524d-197">For notifications without resource data, the payload looks like the following.</span></span> <span data-ttu-id="9524d-198">Эти полезные данные относятся к изменению свойства в команде.</span><span class="sxs-lookup"><span data-stu-id="9524d-198">This payload is for a property change in a team.</span></span>

```json
{
  "id": "19:a3f841d969cd4ae0a7cbe847fc10b371@thread.tacv2",
  "createdDateTime": "2020-02-14T01:10:03.592Z",
  "displayName": "General",
  "description": "Sample Channel description",
  "isFavoriteByDefault": true,
  "email": "",
  "webUrl": "https://teams.microsoft.com/l/channel/19%3Aa3f841d969cd4ae0a7cbe847fc10b371%40thread.tacv2/General?groupId=7ed9bdab-9c7d-4c10-a25d-3f4ff0e34577&tenantId=0f2d8f49-862a-493b-9ca8-82a10637e17d",
  "membershipType": "standard",
  "moderationSettings": null
}
```


## <a name="see-also"></a><span data-ttu-id="9524d-199">См. также</span><span class="sxs-lookup"><span data-stu-id="9524d-199">See also</span></span>
- [<span data-ttu-id="9524d-200">Уведомления об изменениях в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9524d-200">Microsoft Graph change notifications</span></span>](webhooks.md)
- [<span data-ttu-id="9524d-201">Обзор API Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="9524d-201">Microsoft Teams API overview</span></span>](teams-concept-overview.md)
