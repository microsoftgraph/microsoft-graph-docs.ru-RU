---
title: Создание подписки
description: Подписывает приложение-слушатель для получения уведомлений об изменениях при изменении данных о Graph microsoft.
localization_priority: Normal
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 8f2e1524c63ceb77b092f0699f7bf1002a8420b0
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366926"
---
# <a name="create-subscription"></a><span data-ttu-id="4f38b-103">Создание подписки</span><span class="sxs-lookup"><span data-stu-id="4f38b-103">Create subscription</span></span>

<span data-ttu-id="4f38b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f38b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f38b-105">Создание подписки для приложения прослушивателя, позволяющей ему получать уведомления об изменениях определенного типа в указанном ресурсе в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4f38b-105">Subscribes a listener application to receive change notifications when the requested type of changes occur to the specified resource in Microsoft Graph.</span></span>

<span data-ttu-id="4f38b-106">Список ресурсов, поддерживающих подписку на уведомления об изменениях, см. в таблице раздела [Разрешения](#permissions).</span><span class="sxs-lookup"><span data-stu-id="4f38b-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f38b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4f38b-107">Permissions</span></span>

<span data-ttu-id="4f38b-108">Для создания подписки требуется разрешение на чтение на ресурс.</span><span class="sxs-lookup"><span data-stu-id="4f38b-108">Creating a subscription requires read permission to the resource.</span></span> <span data-ttu-id="4f38b-109">Например, чтобы получать уведомления об изменениях в сообщениях, вашему приложению необходимо разрешение Mail.Read.</span><span class="sxs-lookup"><span data-stu-id="4f38b-109">For example, to get change notifications on messages, your app needs the Mail.Read permission.</span></span> 

<span data-ttu-id="4f38b-110">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="4f38b-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="4f38b-111">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f38b-111">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4f38b-112">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="4f38b-112">Supported resource</span></span> | <span data-ttu-id="4f38b-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f38b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4f38b-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f38b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f38b-115">Application</span><span class="sxs-lookup"><span data-stu-id="4f38b-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="4f38b-116">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span><span class="sxs-lookup"><span data-stu-id="4f38b-116">[callRecord](../resources/callrecords-callrecord.md) (/communications/callRecords)</span></span> | <span data-ttu-id="4f38b-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-117">Not supported</span></span> | <span data-ttu-id="4f38b-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-118">Not supported</span></span> | <span data-ttu-id="4f38b-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-119">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="4f38b-120">[каналы](../resources/channel.md) (/teams/getAllChannels — все каналы в организации)</span><span class="sxs-lookup"><span data-stu-id="4f38b-120">[channels](../resources/channel.md) (/teams/getAllChannels – all channels in an organization)</span></span> | <span data-ttu-id="4f38b-121">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-121">Not supported</span></span>  | <span data-ttu-id="4f38b-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-122">Not supported</span></span> | <span data-ttu-id="4f38b-123">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-123">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span> |
|<span data-ttu-id="4f38b-124">[каналы](../resources/channel.md) (/teams/{id}/channels)</span><span class="sxs-lookup"><span data-stu-id="4f38b-124">[channels](../resources/channel.md) (/teams/{id}/channels)</span></span> | <span data-ttu-id="4f38b-125">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-125">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  | <span data-ttu-id="4f38b-126">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-126">Not supported</span></span> | <span data-ttu-id="4f38b-127">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-127">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  |
|<span data-ttu-id="4f38b-128">[чат](../resources/chat.md) (/чаты — все чаты в организации)</span><span class="sxs-lookup"><span data-stu-id="4f38b-128">[chat](../resources/chat.md) (/chats – all chats in an organization)</span></span> | <span data-ttu-id="4f38b-129">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-129">Not supported</span></span> | <span data-ttu-id="4f38b-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-130">Not supported</span></span> | <span data-ttu-id="4f38b-131">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-131">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="4f38b-132">[чат](../resources/chat.md) (/chats/{id})</span><span class="sxs-lookup"><span data-stu-id="4f38b-132">[chat](../resources/chat.md) (/chats/{id})</span></span> | <span data-ttu-id="4f38b-133">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f38b-133">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="4f38b-134">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-134">Not supported</span></span> | <span data-ttu-id="4f38b-135">ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat\*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-135">ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat\*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="4f38b-136">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="4f38b-136">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="4f38b-137">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-137">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="4f38b-138">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-138">Not supported</span></span> | <span data-ttu-id="4f38b-139">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-139">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="4f38b-140">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="4f38b-140">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="4f38b-141">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-141">Not supported</span></span> | <span data-ttu-id="4f38b-142">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-142">Not supported</span></span> | <span data-ttu-id="4f38b-143">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-143">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="4f38b-144">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="4f38b-144">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="4f38b-145">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f38b-145">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="4f38b-146">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-146">Not supported</span></span> | <span data-ttu-id="4f38b-147">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-147">Chat.Read.All</span></span>  |
|<span data-ttu-id="4f38b-148">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="4f38b-148">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="4f38b-149">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-149">Not supported</span></span> | <span data-ttu-id="4f38b-150">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-150">Not supported</span></span> | <span data-ttu-id="4f38b-151">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-151">Chat.Read.All</span></span>  |
|[<span data-ttu-id="4f38b-152">contact</span><span class="sxs-lookup"><span data-stu-id="4f38b-152">contact</span></span>](../resources/contact.md) | <span data-ttu-id="4f38b-153">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="4f38b-153">Contacts.Read</span></span> | <span data-ttu-id="4f38b-154">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="4f38b-154">Contacts.Read</span></span> | <span data-ttu-id="4f38b-155">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="4f38b-155">Contacts.Read</span></span> |
|<span data-ttu-id="4f38b-156">[conversationMember](../resources/conversationmember.md) (/chats/getAllMembers)</span><span class="sxs-lookup"><span data-stu-id="4f38b-156">[conversationMember](../resources/conversationmember.md) (/chats/getAllMembers)</span></span> | <span data-ttu-id="4f38b-157">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-157">Not supported</span></span> | <span data-ttu-id="4f38b-158">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-158">Not supported</span></span> | <span data-ttu-id="4f38b-159">ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-159">ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="4f38b-160">[conversationMember](../resources/conversationmember.md) (/chats/{id}/members)</span><span class="sxs-lookup"><span data-stu-id="4f38b-160">[conversationMember](../resources/conversationmember.md) (/chats/{id}/members)</span></span> | <span data-ttu-id="4f38b-161">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f38b-161">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="4f38b-162">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-162">Not supported</span></span> | <span data-ttu-id="4f38b-163">ChatMember.Read.Chat *, Chat.Manage.Chat*, ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-163">ChatMember.Read.Chat *, Chat.Manage.Chat*, ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="4f38b-164">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members)</span><span class="sxs-lookup"><span data-stu-id="4f38b-164">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members)</span></span> | <span data-ttu-id="4f38b-165">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-165">TeamMember.Read.All</span></span> | <span data-ttu-id="4f38b-166">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-166">Not supported</span></span> | <span data-ttu-id="4f38b-167">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-167">TeamMember.Read.All</span></span> |
|<span data-ttu-id="4f38b-168">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="4f38b-168">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="4f38b-169">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-169">Not supported</span></span> | <span data-ttu-id="4f38b-170">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f38b-170">Files.ReadWrite</span></span> | <span data-ttu-id="4f38b-171">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-171">Not supported</span></span> |
|<span data-ttu-id="4f38b-172">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="4f38b-172">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="4f38b-173">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-173">Files.ReadWrite.All</span></span> | <span data-ttu-id="4f38b-174">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-174">Not supported</span></span> | <span data-ttu-id="4f38b-175">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-175">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="4f38b-176">event</span><span class="sxs-lookup"><span data-stu-id="4f38b-176">event</span></span>](../resources/event.md) | <span data-ttu-id="4f38b-177">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4f38b-177">Calendars.Read</span></span> | <span data-ttu-id="4f38b-178">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4f38b-178">Calendars.Read</span></span> | <span data-ttu-id="4f38b-179">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4f38b-179">Calendars.Read</span></span> |
|[<span data-ttu-id="4f38b-180">group</span><span class="sxs-lookup"><span data-stu-id="4f38b-180">group</span></span>](../resources/group.md) | <span data-ttu-id="4f38b-181">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-181">Group.Read.All</span></span> | <span data-ttu-id="4f38b-182">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-182">Not supported</span></span> | <span data-ttu-id="4f38b-183">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-183">Group.Read.All</span></span> |
|[<span data-ttu-id="4f38b-184">group conversation</span><span class="sxs-lookup"><span data-stu-id="4f38b-184">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="4f38b-185">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-185">Group.Read.All</span></span> | <span data-ttu-id="4f38b-186">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-186">Not supported</span></span> | <span data-ttu-id="4f38b-187">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-187">Not supported</span></span> |
|[<span data-ttu-id="4f38b-188">list</span><span class="sxs-lookup"><span data-stu-id="4f38b-188">list</span></span>](../resources/list.md) | <span data-ttu-id="4f38b-189">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-189">Sites.ReadWrite.All</span></span> | <span data-ttu-id="4f38b-190">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-190">Not supported</span></span> | <span data-ttu-id="4f38b-191">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-191">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="4f38b-192">message</span><span class="sxs-lookup"><span data-stu-id="4f38b-192">message</span></span>](../resources/message.md) | <span data-ttu-id="4f38b-193">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4f38b-193">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="4f38b-194">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4f38b-194">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="4f38b-195">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="4f38b-195">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="4f38b-196">presence</span><span class="sxs-lookup"><span data-stu-id="4f38b-196">presence</span></span>](../resources/presence.md) | <span data-ttu-id="4f38b-197">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-197">Presence.Read.All</span></span> | <span data-ttu-id="4f38b-198">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-198">Not supported</span></span> | <span data-ttu-id="4f38b-199">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-199">Not supported</span></span> |
|[<span data-ttu-id="4f38b-200">printer</span><span class="sxs-lookup"><span data-stu-id="4f38b-200">printer</span></span>](../resources/printer.md) | <span data-ttu-id="4f38b-201">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-201">Not supported</span></span> | <span data-ttu-id="4f38b-202">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-202">Not supported</span></span> | <span data-ttu-id="4f38b-203">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-203">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="4f38b-204">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="4f38b-204">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="4f38b-205">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-205">Not supported</span></span> | <span data-ttu-id="4f38b-206">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-206">Not supported</span></span> | <span data-ttu-id="4f38b-207">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-207">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="4f38b-208">security alert</span><span class="sxs-lookup"><span data-stu-id="4f38b-208">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="4f38b-209">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-209">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="4f38b-210">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-210">Not supported</span></span> | <span data-ttu-id="4f38b-211">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-211">SecurityEvents.ReadWrite.All</span></span> |
|<span data-ttu-id="4f38b-212">[teams](../resources/team.md) (/teams — все команды в организации)</span><span class="sxs-lookup"><span data-stu-id="4f38b-212">[teams](../resources/team.md) (/teams – all teams in an organization)</span></span> | <span data-ttu-id="4f38b-213">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-213">Not supported</span></span> | <span data-ttu-id="4f38b-214">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-214">Not supported</span></span> | <span data-ttu-id="4f38b-215">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-215">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|<span data-ttu-id="4f38b-216">[teams](../resources/team.md) (/teams/{id})</span><span class="sxs-lookup"><span data-stu-id="4f38b-216">[teams](../resources/team.md) (/teams/{id})</span></span> | <span data-ttu-id="4f38b-217">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-217">Team.ReadBasic.All, TeamSettings.Read.All</span></span> | <span data-ttu-id="4f38b-218">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-218">Not supported</span></span> | <span data-ttu-id="4f38b-219">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-219">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|[<span data-ttu-id="4f38b-220">todoTask</span><span class="sxs-lookup"><span data-stu-id="4f38b-220">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="4f38b-221">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f38b-221">Tasks.ReadWrite</span></span> | <span data-ttu-id="4f38b-222">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f38b-222">Tasks.ReadWrite</span></span> | <span data-ttu-id="4f38b-223">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="4f38b-223">Not supported</span></span> |
|[<span data-ttu-id="4f38b-224">user</span><span class="sxs-lookup"><span data-stu-id="4f38b-224">user</span></span>](../resources/user.md) | <span data-ttu-id="4f38b-225">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-225">User.Read.All</span></span> | <span data-ttu-id="4f38b-226">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-226">User.Read.All</span></span> | <span data-ttu-id="4f38b-227">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f38b-227">User.Read.All</span></span> |

> <span data-ttu-id="4f38b-228">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="4f38b-228">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="4f38b-229">driveItem</span><span class="sxs-lookup"><span data-stu-id="4f38b-229">driveItem</span></span>

<span data-ttu-id="4f38b-230">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4f38b-230">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="4f38b-231">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="4f38b-231">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="4f38b-232">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="4f38b-232">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="4f38b-233">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="4f38b-233">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="4f38b-234">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="4f38b-234">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="4f38b-235">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="4f38b-235">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

<span data-ttu-id="4f38b-236">OneDrive для бизнеса и SharePoint поддерживают отправку уведомлений приложений о событиях безопасности, которые происходят в **driveItem**.</span><span class="sxs-lookup"><span data-stu-id="4f38b-236">OneDrive for Business and SharePoint support sending your application notifications of security events that occur on a **driveItem**.</span></span> <span data-ttu-id="4f38b-237">Чтобы подписаться на эти события, добавьте заголовок `prefer:includesecuritywebhooks` в запрос на создание подписки.</span><span class="sxs-lookup"><span data-stu-id="4f38b-237">To subscribe to these events, add the `prefer:includesecuritywebhooks` header to your request to create a subscription.</span></span> <span data-ttu-id="4f38b-238">После создания подписки вы будете получать уведомления об изменениях разрешений для элемента.</span><span class="sxs-lookup"><span data-stu-id="4f38b-238">After the subscription is created, you will receive notifications when the permissions on an item change.</span></span> <span data-ttu-id="4f38b-239">Этот заголовок можно использовать в SharePoint и OneDrive для бизнеса, но не в учетных записях потребителей в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4f38b-239">This header is applicable to SharePoint and OneDrive for Business but not consumer OneDrive accounts.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="4f38b-240">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="4f38b-240">contact, event, and message</span></span>

<span data-ttu-id="4f38b-241">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="4f38b-241">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="4f38b-242">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="4f38b-242">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="4f38b-243">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="4f38b-243">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="4f38b-244">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f38b-244">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="4f38b-245">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="4f38b-245">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="4f38b-246">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="4f38b-246">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="4f38b-247">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="4f38b-247">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="4f38b-248">presence</span><span class="sxs-lookup"><span data-stu-id="4f38b-248">presence</span></span>

<span data-ttu-id="4f38b-249">**Подписки** на присутствие требуют [шифрования.](/graph/webhooks-with-resource-data)</span><span class="sxs-lookup"><span data-stu-id="4f38b-249">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="4f38b-250">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="4f38b-250">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="4f38b-251">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f38b-251">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a><span data-ttu-id="4f38b-252">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f38b-252">Request headers</span></span>

| <span data-ttu-id="4f38b-253">Имя</span><span class="sxs-lookup"><span data-stu-id="4f38b-253">Name</span></span>       | <span data-ttu-id="4f38b-254">Тип</span><span class="sxs-lookup"><span data-stu-id="4f38b-254">Type</span></span> | <span data-ttu-id="4f38b-255">Описание</span><span class="sxs-lookup"><span data-stu-id="4f38b-255">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4f38b-256">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f38b-256">Authorization</span></span>  | <span data-ttu-id="4f38b-257">string</span><span class="sxs-lookup"><span data-stu-id="4f38b-257">string</span></span>  | <span data-ttu-id="4f38b-p109">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f38b-p109">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4f38b-260">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f38b-260">Response</span></span>

<span data-ttu-id="4f38b-261">В случае успешного использования этот метод возвращает код отклика и объект подписки `201 Created` в тексте [](../resources/subscription.md) ответа.</span><span class="sxs-lookup"><span data-stu-id="4f38b-261">If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="4f38b-262">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="4f38b-262">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="4f38b-263">Пример</span><span class="sxs-lookup"><span data-stu-id="4f38b-263">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f38b-264">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f38b-264">Request</span></span>

<span data-ttu-id="4f38b-265">Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f38b-265">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="4f38b-266">Поля `clientState` и `latestSupportedTlsVersion` необязательны.</span><span class="sxs-lookup"><span data-stu-id="4f38b-266">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

<span data-ttu-id="4f38b-267">Этот запрос создает подписку на уведомления об изменениях о новой почте, полученной в настоящее время подписанным пользователем.</span><span class="sxs-lookup"><span data-stu-id="4f38b-267">This request creates a subscription for change notifications about new mail received by the currently signed in user.</span></span>

# <a name="http"></a>[<span data-ttu-id="4f38b-268">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f38b-268">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4f38b-269">C#</span><span class="sxs-lookup"><span data-stu-id="4f38b-269">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subscription-from-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f38b-270">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f38b-270">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subscription-from-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f38b-271">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f38b-271">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subscription-from-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4f38b-272">Java</span><span class="sxs-lookup"><span data-stu-id="4f38b-272">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-subscription-from-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="4f38b-273">Предоставьте в тексте запроса описание объекта [subscription](../resources/subscription.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f38b-273">In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.</span></span>
<span data-ttu-id="4f38b-274">Поля `clientState` и `latestSupportedTlsVersion` необязательны.</span><span class="sxs-lookup"><span data-stu-id="4f38b-274">The `clientState` and `latestSupportedTlsVersion` fields are optional.</span></span>

#### <a name="resources-examples"></a><span data-ttu-id="4f38b-275">Примеры ресурсов</span><span class="sxs-lookup"><span data-stu-id="4f38b-275">Resources examples</span></span>

<span data-ttu-id="4f38b-276">Ниже приводится допустимые значения для свойства ресурса.</span><span class="sxs-lookup"><span data-stu-id="4f38b-276">The following are valid values for the resource property.</span></span>

| <span data-ttu-id="4f38b-277">Тип ресурса</span><span class="sxs-lookup"><span data-stu-id="4f38b-277">Resource type</span></span> | <span data-ttu-id="4f38b-278">Примеры</span><span class="sxs-lookup"><span data-stu-id="4f38b-278">Examples</span></span> |
|:------ |:----- |
|[<span data-ttu-id="4f38b-279">Записи звонков</span><span class="sxs-lookup"><span data-stu-id="4f38b-279">Call records</span></span>](../resources/callrecords-callrecord.md)|`communications/callRecords`|
|[<span data-ttu-id="4f38b-280">Каналы</span><span class="sxs-lookup"><span data-stu-id="4f38b-280">Channels</span></span>](../resources/channel.md)|<span data-ttu-id="4f38b-281">`/teams/getAllChannels`, `/teams/{id}/channels`</span><span class="sxs-lookup"><span data-stu-id="4f38b-281">`/teams/getAllChannels`, `/teams/{id}/channels`</span></span>|
|[<span data-ttu-id="4f38b-282">Чат</span><span class="sxs-lookup"><span data-stu-id="4f38b-282">Chat</span></span>](../resources/chat.md)|<span data-ttu-id="4f38b-283">`/chats`, `/chats/{id}`</span><span class="sxs-lookup"><span data-stu-id="4f38b-283">`/chats`, `/chats/{id}`</span></span>|
|[<span data-ttu-id="4f38b-284">Сообщение чата</span><span class="sxs-lookup"><span data-stu-id="4f38b-284">Chat message</span></span>](../resources/chatmessage.md) | <span data-ttu-id="4f38b-285">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="4f38b-285">`chats/{id}/messages`, `chats/getAllMessages`, `teams/{id}/channels/{id}/messages`, `teams/getAllMessages`</span></span> |
|[<span data-ttu-id="4f38b-286">Контакты</span><span class="sxs-lookup"><span data-stu-id="4f38b-286">Contacts</span></span>](../resources/contact.md)|`me/contacts`|
|[<span data-ttu-id="4f38b-287">ConversationMember</span><span class="sxs-lookup"><span data-stu-id="4f38b-287">ConversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="4f38b-288">`/chats/{id}/members`, `/chats/getAllMembers`, `/teams/{id}/members`</span><span class="sxs-lookup"><span data-stu-id="4f38b-288">`/chats/{id}/members`, `/chats/getAllMembers`, `/teams/{id}/members`</span></span>|
|[<span data-ttu-id="4f38b-289">Беседы</span><span class="sxs-lookup"><span data-stu-id="4f38b-289">Conversations</span></span>](../resources/conversation.md)|`groups('{id}')/conversations`|
|[<span data-ttu-id="4f38b-290">Диски</span><span class="sxs-lookup"><span data-stu-id="4f38b-290">Drives</span></span>](../resources/driveitem.md)|`me/drive/root`|
|[<span data-ttu-id="4f38b-291">События</span><span class="sxs-lookup"><span data-stu-id="4f38b-291">Events</span></span>](../resources/event.md)|`me/events`|
|[<span data-ttu-id="4f38b-292">Группы</span><span class="sxs-lookup"><span data-stu-id="4f38b-292">Groups</span></span>](../resources/group.md)|`groups`|
|[<span data-ttu-id="4f38b-293">Список</span><span class="sxs-lookup"><span data-stu-id="4f38b-293">List</span></span>](../resources/list.md)|`sites/{site-id}/lists/{list-id}`|
|[<span data-ttu-id="4f38b-294">Почта</span><span class="sxs-lookup"><span data-stu-id="4f38b-294">Mail</span></span>](../resources/message.md)|<span data-ttu-id="4f38b-295">`me/mailfolders('inbox')/messages`, `me/messages`</span><span class="sxs-lookup"><span data-stu-id="4f38b-295">`me/mailfolders('inbox')/messages`, `me/messages`</span></span>|
|[<span data-ttu-id="4f38b-296">Присутствие</span><span class="sxs-lookup"><span data-stu-id="4f38b-296">Presence</span></span>](../resources/presence.md)| <span data-ttu-id="4f38b-297">`/communications/presences/{id}` (один пользователь), `/communications/presences?$filter=id in ({id},{id}…)` (несколько пользователей)</span><span class="sxs-lookup"><span data-stu-id="4f38b-297">`/communications/presences/{id}` (single user), `/communications/presences?$filter=id in ({id},{id}…)` (multiple users)</span></span>|
|[<span data-ttu-id="4f38b-298">printer</span><span class="sxs-lookup"><span data-stu-id="4f38b-298">printer</span></span>](../resources/printer.md) |`print/printers/{id}/jobs`|
|[<span data-ttu-id="4f38b-299">PrintTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="4f38b-299">PrintTaskDefinition</span></span>](../resources/printtaskdefinition.md)|`print/taskDefinitions/{id}/tasks`|
|[<span data-ttu-id="4f38b-300">Teams</span><span class="sxs-lookup"><span data-stu-id="4f38b-300">Teams</span></span>](../resources/team.md)|<span data-ttu-id="4f38b-301">`/teams`, `/teams/{id}`</span><span class="sxs-lookup"><span data-stu-id="4f38b-301">`/teams`, `/teams/{id}`</span></span>|
|[<span data-ttu-id="4f38b-302">Пользователи</span><span class="sxs-lookup"><span data-stu-id="4f38b-302">Users</span></span>](../resources/user.md)|`users`|
|[<span data-ttu-id="4f38b-303">todoTask</span><span class="sxs-lookup"><span data-stu-id="4f38b-303">todoTask</span></span>](../resources/todotask.md) | `/me/todo/lists/{todoTaskListId}/tasks`
|[<span data-ttu-id="4f38b-304">Оповещение безопасности</span><span class="sxs-lookup"><span data-stu-id="4f38b-304">Security alert</span></span>](../resources/alert.md)|`security/alerts?$filter=status eq 'NewAlert'`|

> <span data-ttu-id="4f38b-305">**Примечание.** Любой путь, начинающийся с `me`, также можно использовать с `users/{id}` вместо `me`, чтобы указать определенного пользователя, а не текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f38b-305">**Note:** Any path starting with `me` can also be used with `users/{id}` instead of `me` to target a specific user instead of the current user.</span></span>

### <a name="response"></a><span data-ttu-id="4f38b-306">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f38b-306">Response</span></span>

<span data-ttu-id="4f38b-307">Ниже показан пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4f38b-307">The following example shows the response.</span></span> 

><span data-ttu-id="4f38b-308">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4f38b-308">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "changeType": "created",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2",
  "notificationContentType": "application/json"
}
```

### <a name="notification-endpoint-validation"></a><span data-ttu-id="4f38b-309">Проверка конечной точки уведомлений</span><span class="sxs-lookup"><span data-stu-id="4f38b-309">Notification endpoint validation</span></span>

<span data-ttu-id="4f38b-310">Конечная точка уведомления о подписке (указанная в свойстве **notificationUrl)** должна быть способна отвечать на запрос проверки, как описано в настройках уведомлений об изменениях в пользовательских [данных.](/graph/webhooks#notification-endpoint-validation)</span><span class="sxs-lookup"><span data-stu-id="4f38b-310">The subscription notification endpoint (specified in the **notificationUrl** property) must be capable of responding to a validation request as described in [Set up notifications for changes in user data](/graph/webhooks#notification-endpoint-validation).</span></span> <span data-ttu-id="4f38b-311">Если проверка завершилась сбоем, запрос на создание подписки возвращает ошибку 400 (неверный запрос).</span><span class="sxs-lookup"><span data-stu-id="4f38b-311">If validation fails, the request to create the subscription returns a 400 Bad Request error.</span></span>

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


