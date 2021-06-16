---
title: Обновление подписки
description: Возобновление подписки путем увеличения срока действия.
localization_priority: Normal
author: Jumaodhiss
doc_type: apiPageType
ms.prod: change-notifications
ms.openlocfilehash: 592631033cc411e034433d8fe33648b513da403f
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941515"
---
# <a name="update-subscription"></a><span data-ttu-id="6c549-103">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="6c549-103">Update subscription</span></span>

<span data-ttu-id="6c549-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c549-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c549-105">Возобновление подписки путем увеличения срока действия.</span><span class="sxs-lookup"><span data-stu-id="6c549-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="6c549-106">В таблице в разделе [Разрешения](#permissions) перечислены ресурсы, поддерживаюющие подписку на изменение уведомлений.</span><span class="sxs-lookup"><span data-stu-id="6c549-106">The table in the [Permissions](#permissions) section lists the resources that support subscribing to change notifications.</span></span>

<span data-ttu-id="6c549-107">Срок действия подписки истекает по истечении времени, которое зависит от типа ресурса.</span><span class="sxs-lookup"><span data-stu-id="6c549-107">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="6c549-108">Чтобы избежать пропуска уведомлений об изменениях, приложение должно продлить подписки заблаговременно до истечения срока их действия.</span><span class="sxs-lookup"><span data-stu-id="6c549-108">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="6c549-109">См. [подписку](../resources/subscription.md) на максимальную длину подписки для каждого типа ресурсов.</span><span class="sxs-lookup"><span data-stu-id="6c549-109">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c549-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6c549-110">Permissions</span></span>

<span data-ttu-id="6c549-111">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="6c549-111">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="6c549-112">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c549-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6c549-113">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="6c549-113">Supported resource</span></span> | <span data-ttu-id="6c549-114">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c549-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6c549-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c549-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c549-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="6c549-116">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="6c549-117">callRecord</span><span class="sxs-lookup"><span data-stu-id="6c549-117">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="6c549-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6c549-118">Not supported</span></span> | <span data-ttu-id="6c549-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6c549-119">Not supported</span></span> | <span data-ttu-id="6c549-120">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c549-120">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="6c549-121">[каналы](../resources/channel.md) (/teams/getAllChannels — все каналы в организации)</span><span class="sxs-lookup"><span data-stu-id="6c549-121">[channels](../resources/channel.md) (/teams/getAllChannels – all channels in an organization)</span></span> | <span data-ttu-id="6c549-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6c549-122">Not supported</span></span>  | <span data-ttu-id="6c549-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6c549-123">Not supported</span></span> | <span data-ttu-id="6c549-124">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c549-124">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span> |
|<span data-ttu-id="6c549-125">[каналы](../resources/channel.md) (/teams/{id}/channels)</span><span class="sxs-lookup"><span data-stu-id="6c549-125">[channels](../resources/channel.md) (/teams/{id}/channels)</span></span> | <span data-ttu-id="6c549-126">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c549-126">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  | <span data-ttu-id="6c549-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6c549-127">Not supported</span></span> | <span data-ttu-id="6c549-128">Channel.ReadBasic.All, ChannelSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c549-128">Channel.ReadBasic.All, ChannelSettings.Read.All</span></span>  |
|<span data-ttu-id="6c549-129">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="6c549-129">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="6c549-130">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c549-130">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="6c549-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6c549-131">Not supported</span></span> | <span data-ttu-id="6c549-132">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c549-132">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="6c549-133">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="6c549-133">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="6c549-134">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6c549-134">Not supported</span></span> | <span data-ttu-id="6c549-135">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6c549-135">Not supported</span></span> | <span data-ttu-id="6c549-136">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c549-136">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="6c549-137">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="6c549-137">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="6c549-138">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c549-138">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="6c549-139">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6c549-139">Not supported</span></span> | <span data-ttu-id="6c549-140">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c549-140">Chat.Read.All</span></span>  |
|<span data-ttu-id="6c549-141">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="6c549-141">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="6c549-142">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6c549-142">Not supported</span></span> | <span data-ttu-id="6c549-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6c549-143">Not supported</span></span> | <span data-ttu-id="6c549-144">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c549-144">Chat.Read.All</span></span>  |
|[<span data-ttu-id="6c549-145">contact</span><span class="sxs-lookup"><span data-stu-id="6c549-145">contact</span></span>](../resources/contact.md) | <span data-ttu-id="6c549-146">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6c549-146">Contacts.Read</span></span> | <span data-ttu-id="6c549-147">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6c549-147">Contacts.Read</span></span> | <span data-ttu-id="6c549-148">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="6c549-148">Contacts.Read</span></span> |
|<span data-ttu-id="6c549-149">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members)</span><span class="sxs-lookup"><span data-stu-id="6c549-149">[conversationMember](../resources/conversationmember.md) (/teams/{id}/members)</span></span> | <span data-ttu-id="6c549-150">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c549-150">TeamMember.Read.All</span></span> | <span data-ttu-id="6c549-151">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6c549-151">Not supported</span></span> | <span data-ttu-id="6c549-152">TeamMember.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c549-152">TeamMember.Read.All</span></span> |
|<span data-ttu-id="6c549-153">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="6c549-153">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="6c549-154">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6c549-154">Not supported</span></span> | <span data-ttu-id="6c549-155">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c549-155">Files.ReadWrite</span></span> | <span data-ttu-id="6c549-156">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6c549-156">Not supported</span></span> |
|<span data-ttu-id="6c549-157">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="6c549-157">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="6c549-158">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c549-158">Files.ReadWrite.All</span></span> | <span data-ttu-id="6c549-159">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6c549-159">Not supported</span></span> | <span data-ttu-id="6c549-160">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c549-160">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="6c549-161">event</span><span class="sxs-lookup"><span data-stu-id="6c549-161">event</span></span>](../resources/event.md) | <span data-ttu-id="6c549-162">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6c549-162">Calendars.Read</span></span> | <span data-ttu-id="6c549-163">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6c549-163">Calendars.Read</span></span> | <span data-ttu-id="6c549-164">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6c549-164">Calendars.Read</span></span> |
|[<span data-ttu-id="6c549-165">group</span><span class="sxs-lookup"><span data-stu-id="6c549-165">group</span></span>](../resources/group.md) | <span data-ttu-id="6c549-166">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c549-166">Group.Read.All</span></span> | <span data-ttu-id="6c549-167">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6c549-167">Not supported</span></span> | <span data-ttu-id="6c549-168">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c549-168">Group.Read.All</span></span> |
|[<span data-ttu-id="6c549-169">group conversation</span><span class="sxs-lookup"><span data-stu-id="6c549-169">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="6c549-170">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c549-170">Group.Read.All</span></span> | <span data-ttu-id="6c549-171">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6c549-171">Not supported</span></span> | <span data-ttu-id="6c549-172">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6c549-172">Not supported</span></span> |
|[<span data-ttu-id="6c549-173">list</span><span class="sxs-lookup"><span data-stu-id="6c549-173">list</span></span>](../resources/list.md) | <span data-ttu-id="6c549-174">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c549-174">Sites.ReadWrite.All</span></span> | <span data-ttu-id="6c549-175">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6c549-175">Not supported</span></span> | <span data-ttu-id="6c549-176">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c549-176">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="6c549-177">message</span><span class="sxs-lookup"><span data-stu-id="6c549-177">message</span></span>](../resources/message.md) | <span data-ttu-id="6c549-178">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6c549-178">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="6c549-179">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6c549-179">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="6c549-180">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6c549-180">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="6c549-181">presence</span><span class="sxs-lookup"><span data-stu-id="6c549-181">presence</span></span>](../resources/presence.md) | <span data-ttu-id="6c549-182">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c549-182">Presence.Read.All</span></span> | <span data-ttu-id="6c549-183">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6c549-183">Not supported</span></span> | <span data-ttu-id="6c549-184">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6c549-184">Not supported</span></span> |
|[<span data-ttu-id="6c549-185">printer</span><span class="sxs-lookup"><span data-stu-id="6c549-185">printer</span></span>](../resources/printer.md) | <span data-ttu-id="6c549-186">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6c549-186">Not supported</span></span> | <span data-ttu-id="6c549-187">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6c549-187">Not supported</span></span> | <span data-ttu-id="6c549-188">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c549-188">Printer.Read.All, Printer.ReadWrite.All</span></span> |
|[<span data-ttu-id="6c549-189">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="6c549-189">printTaskDefinition</span></span>](../resources/printtaskdefinition.md) | <span data-ttu-id="6c549-190">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6c549-190">Not supported</span></span> | <span data-ttu-id="6c549-191">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6c549-191">Not supported</span></span> | <span data-ttu-id="6c549-192">PrintTaskDefinition.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c549-192">PrintTaskDefinition.ReadWrite.All</span></span> |
|[<span data-ttu-id="6c549-193">security alert</span><span class="sxs-lookup"><span data-stu-id="6c549-193">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="6c549-194">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c549-194">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="6c549-195">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6c549-195">Not supported</span></span> | <span data-ttu-id="6c549-196">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c549-196">SecurityEvents.ReadWrite.All</span></span> |
|<span data-ttu-id="6c549-197">[teams](../resources/team.md) (/teams — все команды в организации)</span><span class="sxs-lookup"><span data-stu-id="6c549-197">[teams](../resources/team.md) (/teams – all teams in an organization)</span></span> | <span data-ttu-id="6c549-198">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6c549-198">Not supported</span></span> | <span data-ttu-id="6c549-199">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6c549-199">Not supported</span></span> | <span data-ttu-id="6c549-200">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c549-200">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|<span data-ttu-id="6c549-201">[teams](../resources/team.md) (/teams/{id})</span><span class="sxs-lookup"><span data-stu-id="6c549-201">[teams](../resources/team.md) (/teams/{id})</span></span> | <span data-ttu-id="6c549-202">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c549-202">Team.ReadBasic.All, TeamSettings.Read.All</span></span> | <span data-ttu-id="6c549-203">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6c549-203">Not supported</span></span> | <span data-ttu-id="6c549-204">Team.ReadBasic.All, TeamSettings.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c549-204">Team.ReadBasic.All, TeamSettings.Read.All</span></span> |
|[<span data-ttu-id="6c549-205">todoTask</span><span class="sxs-lookup"><span data-stu-id="6c549-205">todoTask</span></span>](../resources/todotask.md) | <span data-ttu-id="6c549-206">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c549-206">Tasks.ReadWrite</span></span> | <span data-ttu-id="6c549-207">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6c549-207">Tasks.ReadWrite</span></span> | <span data-ttu-id="6c549-208">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="6c549-208">Not supported</span></span> |
|[<span data-ttu-id="6c549-209">user</span><span class="sxs-lookup"><span data-stu-id="6c549-209">user</span></span>](../resources/user.md) | <span data-ttu-id="6c549-210">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c549-210">User.Read.All</span></span> | <span data-ttu-id="6c549-211">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c549-211">User.Read.All</span></span> | <span data-ttu-id="6c549-212">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c549-212">User.Read.All</span></span> |

> <span data-ttu-id="6c549-213">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="6c549-213">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="6c549-214">driveItem</span><span class="sxs-lookup"><span data-stu-id="6c549-214">driveItem</span></span>

<span data-ttu-id="6c549-215">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="6c549-215">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="6c549-216">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="6c549-216">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="6c549-217">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="6c549-217">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="6c549-218">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="6c549-218">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="6c549-219">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="6c549-219">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="6c549-220">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="6c549-220">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="6c549-221">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="6c549-221">contact, event, and message</span></span>

<span data-ttu-id="6c549-222">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="6c549-222">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="6c549-223">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="6c549-223">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="6c549-224">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="6c549-224">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="6c549-225">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="6c549-225">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="6c549-226">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="6c549-226">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="6c549-227">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="6c549-227">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="6c549-228">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="6c549-228">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="6c549-229">presence</span><span class="sxs-lookup"><span data-stu-id="6c549-229">presence</span></span>

<span data-ttu-id="6c549-230">**Подписки** на присутствие требуют [шифрования.](/graph/webhooks-with-resource-data)</span><span class="sxs-lookup"><span data-stu-id="6c549-230">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="6c549-231">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="6c549-231">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="6c549-232">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c549-232">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6c549-233">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c549-233">Request headers</span></span>

| <span data-ttu-id="6c549-234">Имя</span><span class="sxs-lookup"><span data-stu-id="6c549-234">Name</span></span>       | <span data-ttu-id="6c549-235">Тип</span><span class="sxs-lookup"><span data-stu-id="6c549-235">Type</span></span> | <span data-ttu-id="6c549-236">Описание</span><span class="sxs-lookup"><span data-stu-id="6c549-236">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6c549-237">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c549-237">Authorization</span></span>  | <span data-ttu-id="6c549-238">string</span><span class="sxs-lookup"><span data-stu-id="6c549-238">string</span></span>  | <span data-ttu-id="6c549-p108">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c549-p108">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6c549-241">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c549-241">Response</span></span>

<span data-ttu-id="6c549-242">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6c549-242">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="6c549-243">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="6c549-243">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="6c549-244">Пример</span><span class="sxs-lookup"><span data-stu-id="6c549-244">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6c549-245">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c549-245">Request</span></span>

<span data-ttu-id="6c549-246">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c549-246">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6c549-247">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c549-247">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6c549-248">C#</span><span class="sxs-lookup"><span data-stu-id="6c549-248">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6c549-249">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c549-249">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6c549-250">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c549-250">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6c549-251">Java</span><span class="sxs-lookup"><span data-stu-id="6c549-251">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6c549-252">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c549-252">Response</span></span>

<span data-ttu-id="6c549-253">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6c549-253">Here is an example of the response.</span></span>
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


