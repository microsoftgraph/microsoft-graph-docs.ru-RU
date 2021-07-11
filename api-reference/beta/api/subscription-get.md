---
title: Получение подписки
description: Получение свойств и связей подписки.
localization_priority: Normal
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 7a87d2c594756e4ee9b71e112e459a4c02deb793
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366949"
---
# <a name="get-subscription"></a><span data-ttu-id="2b14e-103">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="2b14e-103">Get subscription</span></span>

<span data-ttu-id="2b14e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b14e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b14e-105">Получение свойств и связей подписки.</span><span class="sxs-lookup"><span data-stu-id="2b14e-105">Retrieve the properties and relationships of a subscription.</span></span>

<span data-ttu-id="2b14e-106">Список ресурсов, поддерживающих подписку на уведомления об изменениях, см. в таблице раздела [Разрешения](#permissions).</span><span class="sxs-lookup"><span data-stu-id="2b14e-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b14e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2b14e-107">Permissions</span></span>

<span data-ttu-id="2b14e-108">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="2b14e-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="2b14e-109">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b14e-109">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2b14e-110">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="2b14e-110">Supported resource</span></span> | <span data-ttu-id="2b14e-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b14e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2b14e-112">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b14e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b14e-113">Приложение</span><span class="sxs-lookup"><span data-stu-id="2b14e-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="2b14e-114">callRecord</span><span class="sxs-lookup"><span data-stu-id="2b14e-114">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="2b14e-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-115">Not supported</span></span> | <span data-ttu-id="2b14e-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-116">Not supported</span></span> | <span data-ttu-id="2b14e-117">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-117">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="2b14e-118">[каналы](../resources/channel.md) (/teams/getAllChannels — все каналы в организации)</span><span class="sxs-lookup"><span data-stu-id="2b14e-118">[channels](../resources/channel.md) (/teams/getAllChannels – all channels in an organization)</span></span> | <span data-ttu-id="2b14e-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-119">Not supported</span></span>  | <span data-ttu-id="2b14e-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-120">Not supported</span></span> | <span data-ttu-id="2b14e-121">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-121">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span> |
|<span data-ttu-id="2b14e-122">[каналы](../resources/channel.md) (/teams/{id}/channels)</span><span class="sxs-lookup"><span data-stu-id="2b14e-122">[channels](../resources/channel.md) (/teams/{id}/channels)</span></span> | <span data-ttu-id="2b14e-123">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-123">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  | <span data-ttu-id="2b14e-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-124">Not supported</span></span> | <span data-ttu-id="2b14e-125">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-125">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  |
|<span data-ttu-id="2b14e-126">[чат](../resources/chat.md) (/чаты — все чаты в организации)</span><span class="sxs-lookup"><span data-stu-id="2b14e-126">[chat](../resources/chat.md) (/chats – all chats in an organization)</span></span> | <span data-ttu-id="2b14e-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-127">Not supported</span></span> | <span data-ttu-id="2b14e-128">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-128">Not supported</span></span> | <span data-ttu-id="2b14e-129">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-129">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="2b14e-130">[чат](../resources/chat.md) (/chats/{id})</span><span class="sxs-lookup"><span data-stu-id="2b14e-130">[chat](../resources/chat.md) (/chats/{id})</span></span> | <span data-ttu-id="2b14e-131">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b14e-131">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="2b14e-132">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-132">Not supported</span></span> | <span data-ttu-id="2b14e-133">ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat\*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-133">ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat\*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="2b14e-134">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="2b14e-134">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="2b14e-135">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-135">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="2b14e-136">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-136">Not supported</span></span> | <span data-ttu-id="2b14e-137">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-137">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="2b14e-138">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="2b14e-138">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="2b14e-139">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-139">Not supported</span></span> | <span data-ttu-id="2b14e-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-140">Not supported</span></span> | <span data-ttu-id="2b14e-141">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-141">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="2b14e-142">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="2b14e-142">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="2b14e-143">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b14e-143">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="2b14e-144">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-144">Not supported</span></span> | <span data-ttu-id="2b14e-145">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-145">Chat.Read.All</span></span>  |
|<span data-ttu-id="2b14e-146">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="2b14e-146">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="2b14e-147">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-147">Not supported</span></span> | <span data-ttu-id="2b14e-148">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-148">Not supported</span></span> | <span data-ttu-id="2b14e-149">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-149">Chat.Read.All</span></span>  |
|[<span data-ttu-id="2b14e-150">contact</span><span class="sxs-lookup"><span data-stu-id="2b14e-150">contact</span></span>](../resources/contact.md) | <span data-ttu-id="2b14e-151">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2b14e-151">Contacts.Read</span></span> | <span data-ttu-id="2b14e-152">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2b14e-152">Contacts.Read</span></span> | <span data-ttu-id="2b14e-153">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2b14e-153">Contacts.Read</span></span> |
|<span data-ttu-id="2b14e-154">[conversationMember](../resources/conversationmember.md) (/chats/getAllMembers)</span><span class="sxs-lookup"><span data-stu-id="2b14e-154">[conversationMember](../resources/conversationmember.md) (/chats/getAllMembers)</span></span> | <span data-ttu-id="2b14e-155">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-155">Not supported</span></span> | <span data-ttu-id="2b14e-156">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-156">Not supported</span></span> | <span data-ttu-id="2b14e-157">ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-157">ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="2b14e-158">[conversationMember](../resources/conversationmember.md) (/chats/{id}/members)</span><span class="sxs-lookup"><span data-stu-id="2b14e-158">[conversationMember](../resources/conversationmember.md) (/chats/{id}/members)</span></span> | <span data-ttu-id="2b14e-159">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b14e-159">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="2b14e-160">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-160">Not supported</span></span> | <span data-ttu-id="2b14e-161">ChatMember.Read.Chat *, Chat.Manage.Chat*, ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-161">ChatMember.Read.Chat *, Chat.Manage.Chat*, ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |
|<span data-ttu-id="2b14e-162">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members)</span><span class="sxs-lookup"><span data-stu-id="2b14e-162">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members)</span></span> | <span data-ttu-id="2b14e-163">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-163">TeamMember.Read.All</span></span> | <span data-ttu-id="2b14e-164">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-164">Not supported</span></span> | <span data-ttu-id="2b14e-165">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-165">TeamMember.Read.All</span></span> |
|<span data-ttu-id="2b14e-166">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="2b14e-166">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="2b14e-167">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-167">Not supported</span></span> | <span data-ttu-id="2b14e-168">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b14e-168">Files.ReadWrite</span></span> | <span data-ttu-id="2b14e-169">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-169">Not supported</span></span> |
|<span data-ttu-id="2b14e-170">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="2b14e-170">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="2b14e-171">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-171">Files.ReadWrite.All</span></span> | <span data-ttu-id="2b14e-172">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-172">Not supported</span></span> | <span data-ttu-id="2b14e-173">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-173">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="2b14e-174">event</span><span class="sxs-lookup"><span data-stu-id="2b14e-174">event</span></span>](../resources/event.md) | <span data-ttu-id="2b14e-175">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2b14e-175">Calendars.Read</span></span> | <span data-ttu-id="2b14e-176">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2b14e-176">Calendars.Read</span></span> | <span data-ttu-id="2b14e-177">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="2b14e-177">Calendars.Read</span></span> |
|[<span data-ttu-id="2b14e-178">group</span><span class="sxs-lookup"><span data-stu-id="2b14e-178">group</span></span>](../resources/group.md) | <span data-ttu-id="2b14e-179">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-179">Group.Read.All</span></span> | <span data-ttu-id="2b14e-180">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-180">Not supported</span></span> | <span data-ttu-id="2b14e-181">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-181">Group.Read.All</span></span> |
|[<span data-ttu-id="2b14e-182">group conversation</span><span class="sxs-lookup"><span data-stu-id="2b14e-182">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="2b14e-183">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-183">Group.Read.All</span></span> | <span data-ttu-id="2b14e-184">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-184">Not supported</span></span> | <span data-ttu-id="2b14e-185">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-185">Not supported</span></span> |
|[<span data-ttu-id="2b14e-186">list</span><span class="sxs-lookup"><span data-stu-id="2b14e-186">list</span></span>](../resources/list.md) | <span data-ttu-id="2b14e-187">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-187">Sites.ReadWrite.All</span></span> | <span data-ttu-id="2b14e-188">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-188">Not supported</span></span> | <span data-ttu-id="2b14e-189">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-189">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="2b14e-190">message</span><span class="sxs-lookup"><span data-stu-id="2b14e-190">message</span></span>](../resources/message.md) | <span data-ttu-id="2b14e-191">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2b14e-191">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="2b14e-192">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2b14e-192">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="2b14e-193">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="2b14e-193">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="2b14e-194">presence</span><span class="sxs-lookup"><span data-stu-id="2b14e-194">presence</span></span>](../resources/presence.md) | <span data-ttu-id="2b14e-195">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-195">Presence.Read.All</span></span> | <span data-ttu-id="2b14e-196">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-196">Not supported</span></span> | <span data-ttu-id="2b14e-197">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-197">Not supported</span></span> |
|[<span data-ttu-id="2b14e-198">printer</span><span class="sxs-lookup"><span data-stu-id="2b14e-198">printer</span></span>](../resources/printer.md) | <span data-ttu-id="2b14e-199">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-199">Not supported</span></span> | <span data-ttu-id="2b14e-200">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-200">Not supported</span></span> | <span data-ttu-id="2b14e-201">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-201">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="2b14e-202">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="2b14e-202">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="2b14e-203">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-203">Not supported</span></span> | <span data-ttu-id="2b14e-204">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-204">Not supported</span></span> | <span data-ttu-id="2b14e-205">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-205">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="2b14e-206">security alert</span><span class="sxs-lookup"><span data-stu-id="2b14e-206">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="2b14e-207">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-207">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="2b14e-208">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-208">Not supported</span></span> | <span data-ttu-id="2b14e-209">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-209">SecurityEvents.ReadWrite.All</span></span> |
|<span data-ttu-id="2b14e-210">[teams](../resources/team.md) (/teams — все команды в организации)</span><span class="sxs-lookup"><span data-stu-id="2b14e-210">[teams](../resources/team.md) (/teams – all teams in an organization)</span></span> | <span data-ttu-id="2b14e-211">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-211">Not supported</span></span> | <span data-ttu-id="2b14e-212">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-212">Not supported</span></span> | <span data-ttu-id="2b14e-213">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-213">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|<span data-ttu-id="2b14e-214">[teams](../resources/team.md) (/teams/{id})</span><span class="sxs-lookup"><span data-stu-id="2b14e-214">[teams](../resources/team.md) (/teams/{id})</span></span> | <span data-ttu-id="2b14e-215">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-215">Team.ReadBasic.All, TeamSettings.Read.All</span></span> | <span data-ttu-id="2b14e-216">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-216">Not supported</span></span> | <span data-ttu-id="2b14e-217">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-217">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|[<span data-ttu-id="2b14e-218">todoTask</span><span class="sxs-lookup"><span data-stu-id="2b14e-218">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="2b14e-219">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b14e-219">Tasks.ReadWrite</span></span> | <span data-ttu-id="2b14e-220">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b14e-220">Tasks.ReadWrite</span></span> | <span data-ttu-id="2b14e-221">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2b14e-221">Not supported</span></span> |
|[<span data-ttu-id="2b14e-222">user</span><span class="sxs-lookup"><span data-stu-id="2b14e-222">user</span></span>](../resources/user.md) | <span data-ttu-id="2b14e-223">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-223">User.Read.All</span></span> | <span data-ttu-id="2b14e-224">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-224">User.Read.All</span></span> | <span data-ttu-id="2b14e-225">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b14e-225">User.Read.All</span></span> |

> <span data-ttu-id="2b14e-226">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="2b14e-226">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="2b14e-227">driveItem</span><span class="sxs-lookup"><span data-stu-id="2b14e-227">driveItem</span></span>

<span data-ttu-id="2b14e-228">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="2b14e-228">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="2b14e-229">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="2b14e-229">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="2b14e-230">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="2b14e-230">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="2b14e-231">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="2b14e-231">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="2b14e-232">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="2b14e-232">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="2b14e-233">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="2b14e-233">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="2b14e-234">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="2b14e-234">contact, event, and message</span></span>

<span data-ttu-id="2b14e-235">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="2b14e-235">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="2b14e-236">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="2b14e-236">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="2b14e-237">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="2b14e-237">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="2b14e-238">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="2b14e-238">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="2b14e-239">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="2b14e-239">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="2b14e-240">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="2b14e-240">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="2b14e-241">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="2b14e-241">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="2b14e-242">presence</span><span class="sxs-lookup"><span data-stu-id="2b14e-242">presence</span></span>

<span data-ttu-id="2b14e-243">**Подписки** на присутствие требуют [шифрования.](/graph/webhooks-with-resource-data)</span><span class="sxs-lookup"><span data-stu-id="2b14e-243">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="2b14e-244">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="2b14e-244">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="2b14e-245">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b14e-245">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2b14e-246">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="2b14e-246">Optional query parameters</span></span>

<span data-ttu-id="2b14e-247">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2b14e-247">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2b14e-248">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b14e-248">Request headers</span></span>

| <span data-ttu-id="2b14e-249">Имя</span><span class="sxs-lookup"><span data-stu-id="2b14e-249">Name</span></span>       | <span data-ttu-id="2b14e-250">Тип</span><span class="sxs-lookup"><span data-stu-id="2b14e-250">Type</span></span> | <span data-ttu-id="2b14e-251">Описание</span><span class="sxs-lookup"><span data-stu-id="2b14e-251">Description</span></span>|
|:-----------|:-----|:-----------|
| <span data-ttu-id="2b14e-252">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b14e-252">Authorization</span></span>  | <span data-ttu-id="2b14e-253">string</span><span class="sxs-lookup"><span data-stu-id="2b14e-253">string</span></span>  | <span data-ttu-id="2b14e-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b14e-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b14e-256">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b14e-256">Request body</span></span>

<span data-ttu-id="2b14e-257">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2b14e-257">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b14e-258">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b14e-258">Response</span></span>

<span data-ttu-id="2b14e-259">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2b14e-259">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b14e-260">Пример</span><span class="sxs-lookup"><span data-stu-id="2b14e-260">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2b14e-261">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b14e-261">Request</span></span>

<span data-ttu-id="2b14e-262">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b14e-262">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2b14e-263">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b14e-263">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="2b14e-264">C#</span><span class="sxs-lookup"><span data-stu-id="2b14e-264">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b14e-265">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b14e-265">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b14e-266">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b14e-266">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2b14e-267">Java</span><span class="sxs-lookup"><span data-stu-id="2b14e-267">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2b14e-268">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b14e-268">Response</span></span>

<span data-ttu-id="2b14e-269">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2b14e-269">Here is an example of the response.</span></span>
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
  "applicationId" : "string",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "lifecycleNotificationUrl":"https://webhook.azurewebsites.net/api/send/lifecycleNotifications",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
  "creatorId": "string",
  "latestSupportedTlsVersion": "v1_2",
  "encryptionCertificate": "",
  "encryptionCertificateId": "",
  "includeResourceData": false,
  "notificationContentType": "application/json"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


