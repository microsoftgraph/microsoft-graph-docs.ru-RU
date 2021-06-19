---
title: Получение уведомлений об изменениях команд и каналов с помощью Microsoft Graph
description: Узнайте, как получать уведомления об изменениях (создание, обновление и удаление) команд и каналов с помощью API Microsoft Graph.
author: anandab
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 44f07661309da100ef65cf691ccfe30261467d52
ms.sourcegitcommit: 39a8c6eccc07ead237dac17387cd269733a86abd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53025021"
---
# <a name="get-change-notifications-for-teams-and-channels-using-microsoft-graph"></a><span data-ttu-id="2003b-103">Получение уведомлений об изменениях команд и каналов с помощью Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2003b-103">Get change notifications for teams and channels using Microsoft Graph</span></span>

<span data-ttu-id="2003b-104">Уведомления об изменениях позволяют подписаться на изменения (создание, обновление и удаление) команд и каналов.</span><span class="sxs-lookup"><span data-stu-id="2003b-104">Change notifications enable you to subscribe to changes (create, update, and delete) to teams and channels.</span></span> <span data-ttu-id="2003b-105">Вы можете получать уведомления при создании, обновлении и удалении команды или канала.</span><span class="sxs-lookup"><span data-stu-id="2003b-105">You can get notified whenever a team or channel is created, updated, or deleted.</span></span> <span data-ttu-id="2003b-106">Кроме того, вы можете получать данные ресурсов в уведомлениях и, следовательно, избегать вызова API, чтобы получить полезные данные.</span><span class="sxs-lookup"><span data-stu-id="2003b-106">You can also get the resource data in the notifications and therefore avoid calling the API to get the payload.</span></span>

## <a name="subscribe-to-changes-in-any-team-at-tenant-level"></a><span data-ttu-id="2003b-107">Подписка на изменения в любой команде на уровне клиента</span><span class="sxs-lookup"><span data-stu-id="2003b-107">Subscribe to changes in any team at tenant level</span></span>

<span data-ttu-id="2003b-108">Чтобы получать уведомления обо всех изменениях (создание, обновление и удаление), связанных с любой командой в клиенте, подпишитесь на `/teams`.</span><span class="sxs-lookup"><span data-stu-id="2003b-108">To get change notifications for all changes (create, update, and delete) related to any team in a tenant, subscribe to `/teams`.</span></span> <span data-ttu-id="2003b-109">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.</span><span class="sxs-lookup"><span data-stu-id="2003b-109">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

### <a name="permissions"></a><span data-ttu-id="2003b-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2003b-110">Permissions</span></span>

|<span data-ttu-id="2003b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2003b-111">Permission type</span></span>      | <span data-ttu-id="2003b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2003b-112">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="2003b-113">Поддерживаемые версии</span><span class="sxs-lookup"><span data-stu-id="2003b-113">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="2003b-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2003b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="2003b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2003b-115">Not supported.</span></span> | <span data-ttu-id="2003b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2003b-116">Not supported.</span></span> |
|<span data-ttu-id="2003b-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2003b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2003b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2003b-118">Not supported.</span></span>    | <span data-ttu-id="2003b-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2003b-119">Not supported.</span></span> |
|<span data-ttu-id="2003b-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="2003b-120">Application</span></span> | <span data-ttu-id="2003b-121">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2003b-121">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All</span></span>   | <span data-ttu-id="2003b-122">бета</span><span class="sxs-lookup"><span data-stu-id="2003b-122">beta</span></span>|

### <a name="example"></a><span data-ttu-id="2003b-123">Пример</span><span class="sxs-lookup"><span data-stu-id="2003b-123">Example</span></span>

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

## <a name="subscribe-to-changes-in-a-particular-team"></a><span data-ttu-id="2003b-124">Подписка на изменения в определенной команде</span><span class="sxs-lookup"><span data-stu-id="2003b-124">Subscribe to changes in a particular team</span></span>


<span data-ttu-id="2003b-125">Чтобы получать уведомления обо всех изменениях, связанных с определенной командой в клиенте, подпишитесь на `/teams/{team-id}`.</span><span class="sxs-lookup"><span data-stu-id="2003b-125">To get change notifications for all changes related to a particular team in a tenant, subscribe to `/teams/{team-id}`.</span></span> <span data-ttu-id="2003b-126">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.</span><span class="sxs-lookup"><span data-stu-id="2003b-126">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

### <a name="permissions"></a><span data-ttu-id="2003b-127">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2003b-127">Permissions</span></span>

|<span data-ttu-id="2003b-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2003b-128">Permission type</span></span>      | <span data-ttu-id="2003b-129">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2003b-129">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="2003b-130">Поддерживаемые версии</span><span class="sxs-lookup"><span data-stu-id="2003b-130">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="2003b-131">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2003b-131">Delegated (work or school account)</span></span> | <span data-ttu-id="2003b-132">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2003b-132">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All</span></span> | <span data-ttu-id="2003b-133">Бета</span><span class="sxs-lookup"><span data-stu-id="2003b-133">beta</span></span> |
|<span data-ttu-id="2003b-134">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2003b-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2003b-135">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2003b-135">Not supported.</span></span>    | <span data-ttu-id="2003b-136">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2003b-136">Not supported.</span></span> |
|<span data-ttu-id="2003b-137">Приложение</span><span class="sxs-lookup"><span data-stu-id="2003b-137">Application</span></span> | <span data-ttu-id="2003b-138">TeamSettings.Read.Group *, TeamSettings.ReadWrite.Group*, Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2003b-138">TeamSettings.Read.Group *, TeamSettings.ReadWrite.Group*, Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All</span></span>    | <span data-ttu-id="2003b-139">Бета</span><span class="sxs-lookup"><span data-stu-id="2003b-139">beta</span></span> |

><span data-ttu-id="2003b-140">**Примечание.** Разрешения, помеченные звездочкой (\*), поддерживаются в рамках [согласия для конкретных ресурсов](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).</span><span class="sxs-lookup"><span data-stu-id="2003b-140">**Note:** Permissions marked with \* are supported as part of [resource-specific consent](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).</span></span>

### <a name="example"></a><span data-ttu-id="2003b-141">Пример</span><span class="sxs-lookup"><span data-stu-id="2003b-141">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{team-id}",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```


## <a name="subscribe-to-changes-in-any-channel-at-tenant-level"></a><span data-ttu-id="2003b-142">Подписка на изменения в любом канале на уровне клиента</span><span class="sxs-lookup"><span data-stu-id="2003b-142">Subscribe to changes in any channel at tenant level</span></span>

<span data-ttu-id="2003b-143">Чтобы получать уведомления обо всех изменениях (создание, обновление и удаление), связанных с любым каналом в клиенте, подпишитесь на `/teams/getAllChannels`.</span><span class="sxs-lookup"><span data-stu-id="2003b-143">To get change notifications for all changes (create, update, and delete) related to any channel in a tenant, subscribe to `/teams/getAllChannels`.</span></span> <span data-ttu-id="2003b-144">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.</span><span class="sxs-lookup"><span data-stu-id="2003b-144">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

><span data-ttu-id="2003b-145">**Примечание.** Закрытые каналы не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="2003b-145">**Note:** Private channels aren't supported.</span></span>

### <a name="permissions"></a><span data-ttu-id="2003b-146">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2003b-146">Permissions</span></span>

|<span data-ttu-id="2003b-147">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2003b-147">Permission type</span></span>      | <span data-ttu-id="2003b-148">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2003b-148">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="2003b-149">Поддерживаемые версии</span><span class="sxs-lookup"><span data-stu-id="2003b-149">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="2003b-150">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2003b-150">Delegated (work or school account)</span></span> | <span data-ttu-id="2003b-151">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2003b-151">Not supported.</span></span> | <span data-ttu-id="2003b-152">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2003b-152">Not supported.</span></span> |
|<span data-ttu-id="2003b-153">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2003b-153">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2003b-154">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2003b-154">Not supported.</span></span>    | <span data-ttu-id="2003b-155">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2003b-155">Not supported.</span></span> |
|<span data-ttu-id="2003b-156">Приложение</span><span class="sxs-lookup"><span data-stu-id="2003b-156">Application</span></span> | <span data-ttu-id="2003b-157">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2003b-157">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All</span></span> | <span data-ttu-id="2003b-158">бета</span><span class="sxs-lookup"><span data-stu-id="2003b-158">beta</span></span> |

### <a name="example"></a><span data-ttu-id="2003b-159">Пример</span><span class="sxs-lookup"><span data-stu-id="2003b-159">Example</span></span>

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

## <a name="subscribe-to-changes-in-any-channel-of-a-particular-team"></a><span data-ttu-id="2003b-160">Подписка на изменения в любом канале определенной команды</span><span class="sxs-lookup"><span data-stu-id="2003b-160">Subscribe to changes in any channel of a particular team</span></span>


<span data-ttu-id="2003b-161">Чтобы получать уведомления обо всех изменениях, связанных с любым каналом в определенной команде, подпишитесь на `/teams/{team-id}/channels`.</span><span class="sxs-lookup"><span data-stu-id="2003b-161">To get change notifications for all changes related to any channel in a particular team, subscribe to `/teams/{team-id}/channels`.</span></span> <span data-ttu-id="2003b-162">Этот ресурс поддерживает [включение данных ресурса](webhooks-with-resource-data.md) в уведомление.</span><span class="sxs-lookup"><span data-stu-id="2003b-162">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

### <a name="permissions"></a><span data-ttu-id="2003b-163">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2003b-163">Permissions</span></span>

|<span data-ttu-id="2003b-164">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2003b-164">Permission type</span></span>      | <span data-ttu-id="2003b-165">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2003b-165">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="2003b-166">Поддерживаемые версии</span><span class="sxs-lookup"><span data-stu-id="2003b-166">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="2003b-167">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2003b-167">Delegated (work or school account)</span></span> | <span data-ttu-id="2003b-168">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2003b-168">Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All</span></span> | <span data-ttu-id="2003b-169">Бета</span><span class="sxs-lookup"><span data-stu-id="2003b-169">beta</span></span> |
|<span data-ttu-id="2003b-170">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2003b-170">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2003b-171">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2003b-171">Not supported.</span></span>    | <span data-ttu-id="2003b-172">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2003b-172">Not supported.</span></span> |
|<span data-ttu-id="2003b-173">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2003b-173">Application</span></span> | <span data-ttu-id="2003b-174">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2003b-174">ChannelSettings.Read.Group *, ChannelSettings.ReadWrite.Group*, Channel.ReadBasic.All, ChannelSettings.Read.All, ChannelSettings.ReadWrite.All</span></span>   | <span data-ttu-id="2003b-175">Бета</span><span class="sxs-lookup"><span data-stu-id="2003b-175">beta</span></span> |

><span data-ttu-id="2003b-176">**Примечание.** Разрешения, помеченные звездочкой (\*), поддерживаются в рамках [согласия для конкретных ресурсов](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).</span><span class="sxs-lookup"><span data-stu-id="2003b-176">**Note:** Permissions marked with \* are supported as part of [resource-specific consent](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).</span></span>

### <a name="example"></a><span data-ttu-id="2003b-177">Пример</span><span class="sxs-lookup"><span data-stu-id="2003b-177">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{team-id}/channels",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```


### <a name="notifications-with-resource-data"></a><span data-ttu-id="2003b-178">Уведомления с данными ресурсов</span><span class="sxs-lookup"><span data-stu-id="2003b-178">Notifications with resource data</span></span>

<span data-ttu-id="2003b-179">Для уведомлений с данными ресурсов полезные данные выглядят следующим образом.</span><span class="sxs-lookup"><span data-stu-id="2003b-179">For notifications with resource data, the payload looks like the following.</span></span> <span data-ttu-id="2003b-180">Эти полезные данные относятся к изменению свойства в команде.</span><span class="sxs-lookup"><span data-stu-id="2003b-180">This payload is for a property change in a team.</span></span>

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



<span data-ttu-id="2003b-181">Расшифрованные полезные данные уведомления выглядят следующим образом.</span><span class="sxs-lookup"><span data-stu-id="2003b-181">The decrypted notification payload looks like the following.</span></span> <span data-ttu-id="2003b-182">Полезные данные соответствуют схеме [teams](/graph/api/resources/team?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="2003b-182">The payload conforms to the [teams](/graph/api/resources/team?preserve-view=true) schema.</span></span> <span data-ttu-id="2003b-183">Полезные данные похожи на результаты, возвращаемые операциями GET.</span><span class="sxs-lookup"><span data-stu-id="2003b-183">The payload is similar to that returned by GET operations.</span></span>

><span data-ttu-id="2003b-184">**Примечание.** [discoverySettings](/graph/api/resources/teamdiscoverysettings?preserve-view=true) и [classSettings](/graph/api/resources/teamclasssettings?preserve-view=true) не предоставляются в полезных данных.</span><span class="sxs-lookup"><span data-stu-id="2003b-184">**Note:** [discoverySettings](/graph/api/resources/teamdiscoverysettings?preserve-view=true) and [classSettings](/graph/api/resources/teamclasssettings?preserve-view=true) aren't exposed in payload data.</span></span>

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


<span data-ttu-id="2003b-185">Для уведомлений с данными ресурсов полезные данные выглядят следующим образом.</span><span class="sxs-lookup"><span data-stu-id="2003b-185">For notifications with resource data, the payload looks like the following.</span></span> <span data-ttu-id="2003b-186">Эти полезные данные относятся к изменению свойства в канале.</span><span class="sxs-lookup"><span data-stu-id="2003b-186">This payload is for a property change in a channel.</span></span>

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
  

<span data-ttu-id="2003b-187">Расшифрованные полезные данные уведомления выглядят следующим образом.</span><span class="sxs-lookup"><span data-stu-id="2003b-187">The decrypted notification payload looks like the following.</span></span> <span data-ttu-id="2003b-188">Полезные данные соответствуют схеме [channel](/graph/api/resources/channel?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="2003b-188">The payload conforms to the [channel](/graph/api/resources/channel?preserve-view=true) schema.</span></span> <span data-ttu-id="2003b-189">Полезные данные похожи на результаты, возвращаемые операциями GET.</span><span class="sxs-lookup"><span data-stu-id="2003b-189">The payload is similar to that returned by GET operations.</span></span>

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


### <a name="notifications-without-resource-data"></a><span data-ttu-id="2003b-190">Уведомления без данных о ресурсах</span><span class="sxs-lookup"><span data-stu-id="2003b-190">Notifications without resource data</span></span>

<span data-ttu-id="2003b-191">Уведомления без данных о ресурсах предоставляют достаточно сведений, чтобы выполнить вызов GET для получения содержимого сообщения.</span><span class="sxs-lookup"><span data-stu-id="2003b-191">Notifications without resource data give you enough information to make GET calls to get the message content.</span></span> <span data-ttu-id="2003b-192">Для подписок на уведомления без данных ресурса не требуется сертификат шифрования (так как фактические данные ресурса не передаются).</span><span class="sxs-lookup"><span data-stu-id="2003b-192">Subscriptions for notifications without resource data don't require an encryption certificate (because actual resource data is not sent over).</span></span>

<span data-ttu-id="2003b-193">Для уведомлений без данных ресурса полезные данные выглядят следующим образом.</span><span class="sxs-lookup"><span data-stu-id="2003b-193">For notifications without resource data, the payload looks like the following.</span></span> <span data-ttu-id="2003b-194">Эти полезные данные относятся к изменению свойства в команде.</span><span class="sxs-lookup"><span data-stu-id="2003b-194">This payload is for a property change in a team.</span></span>

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

<span data-ttu-id="2003b-195">Свойства **resource** и **@odata.id** можно использовать для вызовов в Microsoft Graph, чтобы получить полезные данные для сообщения.</span><span class="sxs-lookup"><span data-stu-id="2003b-195">The **resource** and **@odata.id** properties can be used to make calls to Microsoft Graph to get the payload for the message.</span></span> <span data-ttu-id="2003b-196">Вызовы GET всегда возвращают текущее состояние сообщения.</span><span class="sxs-lookup"><span data-stu-id="2003b-196">GET calls will always return the current state of the message.</span></span> <span data-ttu-id="2003b-197">Если сообщение изменяется с момента отправки уведомления и до получения сообщения, операция возвращает обновленное сообщение.</span><span class="sxs-lookup"><span data-stu-id="2003b-197">If the message is changed between when the notification is sent and when the message is retrieved, the operation will return the updated message.</span></span>


><span data-ttu-id="2003b-198">**Примечание.** Адрес электронной почты канала не возвращается в полезных данных.</span><span class="sxs-lookup"><span data-stu-id="2003b-198">**Note:** Channel email address isn't returned in the payload.</span></span>

<span data-ttu-id="2003b-199">Для уведомлений без данных ресурса полезные данные выглядят следующим образом.</span><span class="sxs-lookup"><span data-stu-id="2003b-199">For notifications without resource data, the payload looks like the following.</span></span> <span data-ttu-id="2003b-200">Эти полезные данные относятся к изменению свойства в команде.</span><span class="sxs-lookup"><span data-stu-id="2003b-200">This payload is for a property change in a team.</span></span>

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


## <a name="see-also"></a><span data-ttu-id="2003b-201">См. также</span><span class="sxs-lookup"><span data-stu-id="2003b-201">See also</span></span>
- [<span data-ttu-id="2003b-202">Уведомления об изменениях в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2003b-202">Microsoft Graph change notifications</span></span>](webhooks.md)
- [<span data-ttu-id="2003b-203">Обзор API Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="2003b-203">Microsoft Teams API overview</span></span>](teams-concept-overview.md)
