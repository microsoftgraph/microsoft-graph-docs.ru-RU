---
title: Удаление подписки
description: Удаление подписки.
localization_priority: Normal
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: d2692e1af87fd7449829ab646d14dd6c3d5a067a
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941489"
---
# <a name="delete-subscription"></a><span data-ttu-id="8bb6a-103">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="8bb6a-103">Delete subscription</span></span>

<span data-ttu-id="8bb6a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bb6a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bb6a-105">Удаление подписки.</span><span class="sxs-lookup"><span data-stu-id="8bb6a-105">Delete a subscription.</span></span>

<span data-ttu-id="8bb6a-106">Список ресурсов, поддерживающих подписку на уведомления об изменениях, см. в таблице раздела [Разрешения](#permissions).</span><span class="sxs-lookup"><span data-stu-id="8bb6a-106">See the table in the [Permissions](#permissions) section for the list of resources that support subscribing to change notifications.</span></span>

## <a name="permissions"></a><span data-ttu-id="8bb6a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8bb6a-107">Permissions</span></span>

<span data-ttu-id="8bb6a-108">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="8bb6a-108">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="8bb6a-109">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bb6a-109">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8bb6a-110">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="8bb6a-110">Supported resource</span></span> | <span data-ttu-id="8bb6a-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8bb6a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8bb6a-112">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8bb6a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bb6a-113">Приложение</span><span class="sxs-lookup"><span data-stu-id="8bb6a-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="8bb6a-114">callRecord</span><span class="sxs-lookup"><span data-stu-id="8bb6a-114">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="8bb6a-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8bb6a-115">Not supported</span></span> | <span data-ttu-id="8bb6a-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8bb6a-116">Not supported</span></span> | <span data-ttu-id="8bb6a-117">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb6a-117">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="8bb6a-118">[каналы](../resources/channel.md) (/teams/getAllChannels — все каналы в организации)</span><span class="sxs-lookup"><span data-stu-id="8bb6a-118">[channels](../resources/channel.md) (/teams/getAllChannels – all channels in an organization)</span></span> | <span data-ttu-id="8bb6a-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8bb6a-119">Not supported</span></span>  | <span data-ttu-id="8bb6a-120">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8bb6a-120">Not supported</span></span> | <span data-ttu-id="8bb6a-121">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb6a-121">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span> |
|<span data-ttu-id="8bb6a-122">[каналы](../resources/channel.md) (/teams/{id}/channels)</span><span class="sxs-lookup"><span data-stu-id="8bb6a-122">[channels](../resources/channel.md) (/teams/{id}/channels)</span></span> | <span data-ttu-id="8bb6a-123">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb6a-123">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  | <span data-ttu-id="8bb6a-124">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8bb6a-124">Not supported</span></span> | <span data-ttu-id="8bb6a-125">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb6a-125">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  |
|<span data-ttu-id="8bb6a-126">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="8bb6a-126">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="8bb6a-127">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bb6a-127">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="8bb6a-128">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8bb6a-128">Not supported</span></span> | <span data-ttu-id="8bb6a-129">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb6a-129">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="8bb6a-130">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="8bb6a-130">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="8bb6a-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8bb6a-131">Not supported</span></span> | <span data-ttu-id="8bb6a-132">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8bb6a-132">Not supported</span></span> | <span data-ttu-id="8bb6a-133">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb6a-133">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="8bb6a-134">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="8bb6a-134">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="8bb6a-135">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8bb6a-135">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="8bb6a-136">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8bb6a-136">Not supported</span></span> | <span data-ttu-id="8bb6a-137">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb6a-137">Chat.Read.All</span></span>  |
|<span data-ttu-id="8bb6a-138">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="8bb6a-138">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="8bb6a-139">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8bb6a-139">Not supported</span></span> | <span data-ttu-id="8bb6a-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8bb6a-140">Not supported</span></span> | <span data-ttu-id="8bb6a-141">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb6a-141">Chat.Read.All</span></span>  |
|[<span data-ttu-id="8bb6a-142">contact</span><span class="sxs-lookup"><span data-stu-id="8bb6a-142">contact</span></span>](../resources/contact.md) | <span data-ttu-id="8bb6a-143">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8bb6a-143">Contacts.Read</span></span> | <span data-ttu-id="8bb6a-144">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8bb6a-144">Contacts.Read</span></span> | <span data-ttu-id="8bb6a-145">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8bb6a-145">Contacts.Read</span></span> |
|<span data-ttu-id="8bb6a-146">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members)</span><span class="sxs-lookup"><span data-stu-id="8bb6a-146">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members)</span></span> | <span data-ttu-id="8bb6a-147">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb6a-147">TeamMember.Read.All</span></span> | <span data-ttu-id="8bb6a-148">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8bb6a-148">Not supported</span></span> | <span data-ttu-id="8bb6a-149">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb6a-149">TeamMember.Read.All</span></span> |
|<span data-ttu-id="8bb6a-150">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="8bb6a-150">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="8bb6a-151">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8bb6a-151">Not supported</span></span> | <span data-ttu-id="8bb6a-152">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8bb6a-152">Files.ReadWrite</span></span> | <span data-ttu-id="8bb6a-153">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8bb6a-153">Not supported</span></span> |
|<span data-ttu-id="8bb6a-154">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="8bb6a-154">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="8bb6a-155">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bb6a-155">Files.ReadWrite.All</span></span> | <span data-ttu-id="8bb6a-156">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8bb6a-156">Not supported</span></span> | <span data-ttu-id="8bb6a-157">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bb6a-157">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="8bb6a-158">event</span><span class="sxs-lookup"><span data-stu-id="8bb6a-158">event</span></span>](../resources/event.md) | <span data-ttu-id="8bb6a-159">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8bb6a-159">Calendars.Read</span></span> | <span data-ttu-id="8bb6a-160">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8bb6a-160">Calendars.Read</span></span> | <span data-ttu-id="8bb6a-161">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8bb6a-161">Calendars.Read</span></span> |
|[<span data-ttu-id="8bb6a-162">group</span><span class="sxs-lookup"><span data-stu-id="8bb6a-162">group</span></span>](../resources/group.md) | <span data-ttu-id="8bb6a-163">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb6a-163">Group.Read.All</span></span> | <span data-ttu-id="8bb6a-164">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8bb6a-164">Not supported</span></span> | <span data-ttu-id="8bb6a-165">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb6a-165">Group.Read.All</span></span> |
|[<span data-ttu-id="8bb6a-166">group conversation</span><span class="sxs-lookup"><span data-stu-id="8bb6a-166">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="8bb6a-167">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb6a-167">Group.Read.All</span></span> | <span data-ttu-id="8bb6a-168">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8bb6a-168">Not supported</span></span> | <span data-ttu-id="8bb6a-169">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8bb6a-169">Not supported</span></span> |
|[<span data-ttu-id="8bb6a-170">list</span><span class="sxs-lookup"><span data-stu-id="8bb6a-170">list</span></span>](../resources/list.md) | <span data-ttu-id="8bb6a-171">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bb6a-171">Sites.ReadWrite.All</span></span> | <span data-ttu-id="8bb6a-172">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8bb6a-172">Not supported</span></span> | <span data-ttu-id="8bb6a-173">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bb6a-173">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="8bb6a-174">message</span><span class="sxs-lookup"><span data-stu-id="8bb6a-174">message</span></span>](../resources/message.md) | <span data-ttu-id="8bb6a-175">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8bb6a-175">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="8bb6a-176">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8bb6a-176">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="8bb6a-177">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8bb6a-177">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="8bb6a-178">presence</span><span class="sxs-lookup"><span data-stu-id="8bb6a-178">presence</span></span>](../resources/presence.md) | <span data-ttu-id="8bb6a-179">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb6a-179">Presence.Read.All</span></span> | <span data-ttu-id="8bb6a-180">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8bb6a-180">Not supported</span></span> | <span data-ttu-id="8bb6a-181">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8bb6a-181">Not supported</span></span> |
|[<span data-ttu-id="8bb6a-182">printer</span><span class="sxs-lookup"><span data-stu-id="8bb6a-182">printer</span></span>](../resources/printer.md) | <span data-ttu-id="8bb6a-183">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8bb6a-183">Not supported</span></span> | <span data-ttu-id="8bb6a-184">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8bb6a-184">Not supported</span></span> | <span data-ttu-id="8bb6a-185">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bb6a-185">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="8bb6a-186">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="8bb6a-186">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="8bb6a-187">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8bb6a-187">Not supported</span></span> | <span data-ttu-id="8bb6a-188">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8bb6a-188">Not supported</span></span> | <span data-ttu-id="8bb6a-189">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bb6a-189">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="8bb6a-190">security alert</span><span class="sxs-lookup"><span data-stu-id="8bb6a-190">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="8bb6a-191">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bb6a-191">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="8bb6a-192">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8bb6a-192">Not supported</span></span> | <span data-ttu-id="8bb6a-193">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bb6a-193">SecurityEvents.ReadWrite.All</span></span> |
|<span data-ttu-id="8bb6a-194">[teams](../resources/team.md) (/teams — все команды в организации)</span><span class="sxs-lookup"><span data-stu-id="8bb6a-194">[teams](../resources/team.md) (/teams – all teams in an organization)</span></span> | <span data-ttu-id="8bb6a-195">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8bb6a-195">Not supported</span></span> | <span data-ttu-id="8bb6a-196">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8bb6a-196">Not supported</span></span> | <span data-ttu-id="8bb6a-197">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb6a-197">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|<span data-ttu-id="8bb6a-198">[teams](../resources/team.md) (/teams/{id})</span><span class="sxs-lookup"><span data-stu-id="8bb6a-198">[teams](../resources/team.md) (/teams/{id})</span></span> | <span data-ttu-id="8bb6a-199">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb6a-199">Team.ReadBasic.All, TeamSettings.Read.All</span></span> | <span data-ttu-id="8bb6a-200">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8bb6a-200">Not supported</span></span> | <span data-ttu-id="8bb6a-201">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb6a-201">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|[<span data-ttu-id="8bb6a-202">todoTask</span><span class="sxs-lookup"><span data-stu-id="8bb6a-202">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="8bb6a-203">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8bb6a-203">Tasks.ReadWrite</span></span> | <span data-ttu-id="8bb6a-204">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8bb6a-204">Tasks.ReadWrite</span></span> | <span data-ttu-id="8bb6a-205">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="8bb6a-205">Not supported</span></span> |
|[<span data-ttu-id="8bb6a-206">user</span><span class="sxs-lookup"><span data-stu-id="8bb6a-206">user</span></span>](../resources/user.md) | <span data-ttu-id="8bb6a-207">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb6a-207">User.Read.All</span></span> | <span data-ttu-id="8bb6a-208">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb6a-208">User.Read.All</span></span> | <span data-ttu-id="8bb6a-209">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="8bb6a-209">User.Read.All</span></span> |

> <span data-ttu-id="8bb6a-210">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="8bb6a-210">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="8bb6a-211">driveItem</span><span class="sxs-lookup"><span data-stu-id="8bb6a-211">driveItem</span></span>

<span data-ttu-id="8bb6a-212">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="8bb6a-212">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="8bb6a-213">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="8bb6a-213">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="8bb6a-214">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="8bb6a-214">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="8bb6a-215">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="8bb6a-215">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="8bb6a-216">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="8bb6a-216">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="8bb6a-217">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="8bb6a-217">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="8bb6a-218">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="8bb6a-218">contact, event, and message</span></span>

<span data-ttu-id="8bb6a-219">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="8bb6a-219">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="8bb6a-220">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="8bb6a-220">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="8bb6a-221">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="8bb6a-221">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="8bb6a-222">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="8bb6a-222">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="8bb6a-223">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="8bb6a-223">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="8bb6a-224">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="8bb6a-224">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="8bb6a-225">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="8bb6a-225">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="8bb6a-226">presence</span><span class="sxs-lookup"><span data-stu-id="8bb6a-226">presence</span></span>

<span data-ttu-id="8bb6a-227">**Подписки** на присутствие требуют [шифрования.](/graph/webhooks-with-resource-data)</span><span class="sxs-lookup"><span data-stu-id="8bb6a-227">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="8bb6a-228">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="8bb6a-228">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="8bb6a-229">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8bb6a-229">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{subscription-id}
```

## <a name="request-headers"></a><span data-ttu-id="8bb6a-230">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8bb6a-230">Request headers</span></span>

| <span data-ttu-id="8bb6a-231">Имя</span><span class="sxs-lookup"><span data-stu-id="8bb6a-231">Name</span></span>       | <span data-ttu-id="8bb6a-232">Тип</span><span class="sxs-lookup"><span data-stu-id="8bb6a-232">Type</span></span> | <span data-ttu-id="8bb6a-233">Описание</span><span class="sxs-lookup"><span data-stu-id="8bb6a-233">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8bb6a-234">Authorization</span><span class="sxs-lookup"><span data-stu-id="8bb6a-234">Authorization</span></span>  | <span data-ttu-id="8bb6a-235">string</span><span class="sxs-lookup"><span data-stu-id="8bb6a-235">string</span></span>  | <span data-ttu-id="8bb6a-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8bb6a-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8bb6a-238">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8bb6a-238">Request body</span></span>

<span data-ttu-id="8bb6a-239">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8bb6a-239">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8bb6a-240">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bb6a-240">Response</span></span>

<span data-ttu-id="8bb6a-241">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8bb6a-241">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="8bb6a-242">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="8bb6a-242">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="8bb6a-243">Пример</span><span class="sxs-lookup"><span data-stu-id="8bb6a-243">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8bb6a-244">Запрос</span><span class="sxs-lookup"><span data-stu-id="8bb6a-244">Request</span></span>

<span data-ttu-id="8bb6a-245">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8bb6a-245">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8bb6a-246">HTTP</span><span class="sxs-lookup"><span data-stu-id="8bb6a-246">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/beta/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07
```
# <a name="c"></a>[<span data-ttu-id="8bb6a-247">C#</span><span class="sxs-lookup"><span data-stu-id="8bb6a-247">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8bb6a-248">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8bb6a-248">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8bb6a-249">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8bb6a-249">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8bb6a-250">Java</span><span class="sxs-lookup"><span data-stu-id="8bb6a-250">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8bb6a-251">Отклик</span><span class="sxs-lookup"><span data-stu-id="8bb6a-251">Response</span></span>

<span data-ttu-id="8bb6a-252">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8bb6a-252">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


