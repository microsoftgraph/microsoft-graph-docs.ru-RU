---
title: Обновление подписки
description: Возобновление подписки путем увеличения срока действия.
localization_priority: Normal
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 96680ebb1cedf85f7272bc09b8ab1c55a04c7591
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366928"
---
# <a name="update-subscription"></a><span data-ttu-id="1b41a-103">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="1b41a-103">Update subscription</span></span>

<span data-ttu-id="1b41a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b41a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b41a-105">Возобновление подписки путем увеличения срока действия.</span><span class="sxs-lookup"><span data-stu-id="1b41a-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="1b41a-106">В таблице в разделе [Разрешения](#permissions) перечислены ресурсы, поддерживаюющие подписку на изменение уведомлений.</span><span class="sxs-lookup"><span data-stu-id="1b41a-106">The table in the [Permissions](#permissions) section lists the resources that support subscribing to change notifications.</span></span>

<span data-ttu-id="1b41a-107">Срок действия подписки истекает по истечении времени, которое зависит от типа ресурса.</span><span class="sxs-lookup"><span data-stu-id="1b41a-107">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="1b41a-108">Чтобы избежать пропуска уведомлений об изменениях, приложение должно продлить подписки заблаговременно до истечения срока их действия.</span><span class="sxs-lookup"><span data-stu-id="1b41a-108">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="1b41a-109">См. [подписку](../resources/subscription.md) на максимальную длину подписки для каждого типа ресурсов.</span><span class="sxs-lookup"><span data-stu-id="1b41a-109">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b41a-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1b41a-110">Permissions</span></span>

<span data-ttu-id="1b41a-111">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="1b41a-111">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="1b41a-112">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b41a-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1b41a-113">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="1b41a-113">Supported resource</span></span> | <span data-ttu-id="1b41a-114">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b41a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="1b41a-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b41a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b41a-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="1b41a-116">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="1b41a-117">callRecord</span><span class="sxs-lookup"><span data-stu-id="1b41a-117">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="1b41a-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-118">Not supported</span></span> | <span data-ttu-id="1b41a-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-119">Not supported</span></span> | <span data-ttu-id="1b41a-120">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-120">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="1b41a-121">[каналы](../resources/channel.md) (/teams/getAllChannels — все каналы в организации)</span><span class="sxs-lookup"><span data-stu-id="1b41a-121">[channels](../resources/channel.md) (/teams/getAllChannels – all channels in an organization)</span></span> | <span data-ttu-id="1b41a-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-122">Not supported</span></span>  | <span data-ttu-id="1b41a-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-123">Not supported</span></span> | <span data-ttu-id="1b41a-124">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-124">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span> |
|<span data-ttu-id="1b41a-125">[каналы](../resources/channel.md) (/teams/{id}/channels)</span><span class="sxs-lookup"><span data-stu-id="1b41a-125">[channels](../resources/channel.md) (/teams/{id}/channels)</span></span> | <span data-ttu-id="1b41a-126">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-126">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  | <span data-ttu-id="1b41a-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-127">Not supported</span></span> | <span data-ttu-id="1b41a-128">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-128">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  |
|<span data-ttu-id="1b41a-129">[чат](../resources/chat.md) (/чаты — все чаты в организации)</span><span class="sxs-lookup"><span data-stu-id="1b41a-129">[chat](../resources/chat.md) (/chats – all chats in an organization)</span></span> | <span data-ttu-id="1b41a-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-130">Not supported</span></span> | <span data-ttu-id="1b41a-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-131">Not supported</span></span> | <span data-ttu-id="1b41a-132">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-132">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="1b41a-133">[чат](../resources/chat.md) (/chats/{id})</span><span class="sxs-lookup"><span data-stu-id="1b41a-133">[chat](../resources/chat.md) (/chats/{id})</span></span> | <span data-ttu-id="1b41a-134">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b41a-134">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="1b41a-135">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-135">Not supported</span></span> | <span data-ttu-id="1b41a-136">ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat\*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-136">ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat\*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="1b41a-137">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="1b41a-137">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="1b41a-138">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-138">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="1b41a-139">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-139">Not supported</span></span> | <span data-ttu-id="1b41a-140">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-140">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="1b41a-141">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="1b41a-141">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="1b41a-142">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-142">Not supported</span></span> | <span data-ttu-id="1b41a-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-143">Not supported</span></span> | <span data-ttu-id="1b41a-144">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-144">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="1b41a-145">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="1b41a-145">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="1b41a-146">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b41a-146">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="1b41a-147">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-147">Not supported</span></span> | <span data-ttu-id="1b41a-148">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-148">Chat.Read.All</span></span>  |
|<span data-ttu-id="1b41a-149">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="1b41a-149">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="1b41a-150">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-150">Not supported</span></span> | <span data-ttu-id="1b41a-151">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-151">Not supported</span></span> | <span data-ttu-id="1b41a-152">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-152">Chat.Read.All</span></span>  |
|[<span data-ttu-id="1b41a-153">contact</span><span class="sxs-lookup"><span data-stu-id="1b41a-153">contact</span></span>](../resources/contact.md) | <span data-ttu-id="1b41a-154">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1b41a-154">Contacts.Read</span></span> | <span data-ttu-id="1b41a-155">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1b41a-155">Contacts.Read</span></span> | <span data-ttu-id="1b41a-156">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1b41a-156">Contacts.Read</span></span> |
|<span data-ttu-id="1b41a-157">[conversationMember](../resources/conversationmember.md) (/chats/getAllMembers)</span><span class="sxs-lookup"><span data-stu-id="1b41a-157">[conversationMember](../resources/conversationmember.md) (/chats/getAllMembers)</span></span> | <span data-ttu-id="1b41a-158">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-158">Not supported</span></span> | <span data-ttu-id="1b41a-159">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-159">Not supported</span></span> | <span data-ttu-id="1b41a-160">ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-160">ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="1b41a-161">[conversationMember](../resources/conversationmember.md) (/chats/{id}/members)</span><span class="sxs-lookup"><span data-stu-id="1b41a-161">[conversationMember](../resources/conversationmember.md) (/chats/{id}/members)</span></span> | <span data-ttu-id="1b41a-162">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b41a-162">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="1b41a-163">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-163">Not supported</span></span> | <span data-ttu-id="1b41a-164">ChatMember.Read.Chat *, Chat.Manage.Chat*, ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-164">ChatMember.Read.Chat *, Chat.Manage.Chat*, ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="1b41a-165">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members)</span><span class="sxs-lookup"><span data-stu-id="1b41a-165">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members)</span></span> | <span data-ttu-id="1b41a-166">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-166">TeamMember.Read.All</span></span> | <span data-ttu-id="1b41a-167">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-167">Not supported</span></span> | <span data-ttu-id="1b41a-168">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-168">TeamMember.Read.All</span></span> |
|<span data-ttu-id="1b41a-169">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="1b41a-169">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="1b41a-170">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-170">Not supported</span></span> | <span data-ttu-id="1b41a-171">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b41a-171">Files.ReadWrite</span></span> | <span data-ttu-id="1b41a-172">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-172">Not supported</span></span> |
|<span data-ttu-id="1b41a-173">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="1b41a-173">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="1b41a-174">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-174">Files.ReadWrite.All</span></span> | <span data-ttu-id="1b41a-175">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-175">Not supported</span></span> | <span data-ttu-id="1b41a-176">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-176">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="1b41a-177">event</span><span class="sxs-lookup"><span data-stu-id="1b41a-177">event</span></span>](../resources/event.md) | <span data-ttu-id="1b41a-178">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1b41a-178">Calendars.Read</span></span> | <span data-ttu-id="1b41a-179">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1b41a-179">Calendars.Read</span></span> | <span data-ttu-id="1b41a-180">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1b41a-180">Calendars.Read</span></span> |
|[<span data-ttu-id="1b41a-181">group</span><span class="sxs-lookup"><span data-stu-id="1b41a-181">group</span></span>](../resources/group.md) | <span data-ttu-id="1b41a-182">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-182">Group.Read.All</span></span> | <span data-ttu-id="1b41a-183">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-183">Not supported</span></span> | <span data-ttu-id="1b41a-184">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-184">Group.Read.All</span></span> |
|[<span data-ttu-id="1b41a-185">group conversation</span><span class="sxs-lookup"><span data-stu-id="1b41a-185">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="1b41a-186">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-186">Group.Read.All</span></span> | <span data-ttu-id="1b41a-187">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-187">Not supported</span></span> | <span data-ttu-id="1b41a-188">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-188">Not supported</span></span> |
|[<span data-ttu-id="1b41a-189">list</span><span class="sxs-lookup"><span data-stu-id="1b41a-189">list</span></span>](../resources/list.md) | <span data-ttu-id="1b41a-190">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-190">Sites.ReadWrite.All</span></span> | <span data-ttu-id="1b41a-191">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-191">Not supported</span></span> | <span data-ttu-id="1b41a-192">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-192">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="1b41a-193">message</span><span class="sxs-lookup"><span data-stu-id="1b41a-193">message</span></span>](../resources/message.md) | <span data-ttu-id="1b41a-194">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1b41a-194">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="1b41a-195">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1b41a-195">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="1b41a-196">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1b41a-196">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="1b41a-197">presence</span><span class="sxs-lookup"><span data-stu-id="1b41a-197">presence</span></span>](../resources/presence.md) | <span data-ttu-id="1b41a-198">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-198">Presence.Read.All</span></span> | <span data-ttu-id="1b41a-199">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-199">Not supported</span></span> | <span data-ttu-id="1b41a-200">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-200">Not supported</span></span> |
|[<span data-ttu-id="1b41a-201">printer</span><span class="sxs-lookup"><span data-stu-id="1b41a-201">printer</span></span>](../resources/printer.md) | <span data-ttu-id="1b41a-202">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-202">Not supported</span></span> | <span data-ttu-id="1b41a-203">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-203">Not supported</span></span> | <span data-ttu-id="1b41a-204">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-204">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="1b41a-205">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="1b41a-205">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="1b41a-206">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-206">Not supported</span></span> | <span data-ttu-id="1b41a-207">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-207">Not supported</span></span> | <span data-ttu-id="1b41a-208">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-208">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="1b41a-209">security alert</span><span class="sxs-lookup"><span data-stu-id="1b41a-209">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="1b41a-210">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-210">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="1b41a-211">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-211">Not supported</span></span> | <span data-ttu-id="1b41a-212">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-212">SecurityEvents.ReadWrite.All</span></span> |
|<span data-ttu-id="1b41a-213">[teams](../resources/team.md) (/teams — все команды в организации)</span><span class="sxs-lookup"><span data-stu-id="1b41a-213">[teams](../resources/team.md) (/teams – all teams in an organization)</span></span> | <span data-ttu-id="1b41a-214">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-214">Not supported</span></span> | <span data-ttu-id="1b41a-215">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-215">Not supported</span></span> | <span data-ttu-id="1b41a-216">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-216">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|<span data-ttu-id="1b41a-217">[teams](../resources/team.md) (/teams/{id})</span><span class="sxs-lookup"><span data-stu-id="1b41a-217">[teams](../resources/team.md) (/teams/{id})</span></span> | <span data-ttu-id="1b41a-218">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-218">Team.ReadBasic.All, TeamSettings.Read.All</span></span> | <span data-ttu-id="1b41a-219">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-219">Not supported</span></span> | <span data-ttu-id="1b41a-220">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-220">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|[<span data-ttu-id="1b41a-221">todoTask</span><span class="sxs-lookup"><span data-stu-id="1b41a-221">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="1b41a-222">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b41a-222">Tasks.ReadWrite</span></span> | <span data-ttu-id="1b41a-223">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b41a-223">Tasks.ReadWrite</span></span> | <span data-ttu-id="1b41a-224">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1b41a-224">Not supported</span></span> |
|[<span data-ttu-id="1b41a-225">user</span><span class="sxs-lookup"><span data-stu-id="1b41a-225">user</span></span>](../resources/user.md) | <span data-ttu-id="1b41a-226">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-226">User.Read.All</span></span> | <span data-ttu-id="1b41a-227">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-227">User.Read.All</span></span> | <span data-ttu-id="1b41a-228">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b41a-228">User.Read.All</span></span> |

> <span data-ttu-id="1b41a-229">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="1b41a-229">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="1b41a-230">driveItem</span><span class="sxs-lookup"><span data-stu-id="1b41a-230">driveItem</span></span>

<span data-ttu-id="1b41a-231">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="1b41a-231">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="1b41a-232">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="1b41a-232">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="1b41a-233">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="1b41a-233">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="1b41a-234">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="1b41a-234">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="1b41a-235">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="1b41a-235">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="1b41a-236">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="1b41a-236">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="1b41a-237">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="1b41a-237">contact, event, and message</span></span>

<span data-ttu-id="1b41a-238">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="1b41a-238">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="1b41a-239">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="1b41a-239">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="1b41a-240">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="1b41a-240">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="1b41a-241">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="1b41a-241">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="1b41a-242">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="1b41a-242">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="1b41a-243">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="1b41a-243">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="1b41a-244">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="1b41a-244">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="1b41a-245">presence</span><span class="sxs-lookup"><span data-stu-id="1b41a-245">presence</span></span>

<span data-ttu-id="1b41a-246">**Подписки** на присутствие требуют [шифрования.](/graph/webhooks-with-resource-data)</span><span class="sxs-lookup"><span data-stu-id="1b41a-246">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="1b41a-247">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="1b41a-247">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="1b41a-248">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b41a-248">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1b41a-249">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b41a-249">Request headers</span></span>

| <span data-ttu-id="1b41a-250">Имя</span><span class="sxs-lookup"><span data-stu-id="1b41a-250">Name</span></span>       | <span data-ttu-id="1b41a-251">Тип</span><span class="sxs-lookup"><span data-stu-id="1b41a-251">Type</span></span> | <span data-ttu-id="1b41a-252">Описание</span><span class="sxs-lookup"><span data-stu-id="1b41a-252">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1b41a-253">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b41a-253">Authorization</span></span>  | <span data-ttu-id="1b41a-254">string</span><span class="sxs-lookup"><span data-stu-id="1b41a-254">string</span></span>  | <span data-ttu-id="1b41a-p108">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b41a-p108">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="1b41a-257">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b41a-257">Response</span></span>

<span data-ttu-id="1b41a-258">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1b41a-258">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="1b41a-259">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="1b41a-259">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="1b41a-260">Пример</span><span class="sxs-lookup"><span data-stu-id="1b41a-260">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1b41a-261">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b41a-261">Request</span></span>

<span data-ttu-id="1b41a-262">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b41a-262">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1b41a-263">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b41a-263">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/beta/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```
# <a name="c"></a>[<span data-ttu-id="1b41a-264">C#</span><span class="sxs-lookup"><span data-stu-id="1b41a-264">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b41a-265">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b41a-265">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b41a-266">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b41a-266">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1b41a-267">Java</span><span class="sxs-lookup"><span data-stu-id="1b41a-267">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1b41a-268">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b41a-268">Response</span></span>

<span data-ttu-id="1b41a-269">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1b41a-269">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "lifecycleNotificationUrl":"https://webhook.azurewebsites.net/api/send/lifecycleNotifications",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2",
  "encryptionCertificate": "",
  "encryptionCertificateId": "",
  "includeResourceData": false,
  "notificationContentType": "application/json"
}
```

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


