---
title: Обновление подписки
description: Возобновление подписки путем увеличения срока действия.
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: e23995651f4ad08f75a435bc3a75323c64927c31
ms.sourcegitcommit: bbff139eea483faaa2d1dd08af39314f35ef48ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/08/2020
ms.locfileid: "46598131"
---
# <a name="update-subscription"></a><span data-ttu-id="c82d8-103">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="c82d8-103">Update subscription</span></span>

<span data-ttu-id="c82d8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c82d8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c82d8-105">Возобновление подписки путем увеличения срока действия.</span><span class="sxs-lookup"><span data-stu-id="c82d8-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="c82d8-106">Срок действия подписок истечет через период времени, который зависит от типа ресурса.</span><span class="sxs-lookup"><span data-stu-id="c82d8-106">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="c82d8-107">Чтобы избежать отсутствия уведомлений об изменениях, приложение должно правильно обновить свои подписки до истечения срока их действия.</span><span class="sxs-lookup"><span data-stu-id="c82d8-107">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="c82d8-108">В этой [статье приведены сведения](../resources/subscription.md) о максимальной длине подписки для каждого типа ресурсов.</span><span class="sxs-lookup"><span data-stu-id="c82d8-108">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="c82d8-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c82d8-109">Permissions</span></span>

<span data-ttu-id="c82d8-110">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="c82d8-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="c82d8-111">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c82d8-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c82d8-112">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="c82d8-112">Supported resource</span></span> | <span data-ttu-id="c82d8-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c82d8-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c82d8-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c82d8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c82d8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c82d8-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="c82d8-116">callRecord</span><span class="sxs-lookup"><span data-stu-id="c82d8-116">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="c82d8-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c82d8-117">Not supported</span></span> | <span data-ttu-id="c82d8-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c82d8-118">Not supported</span></span> | <span data-ttu-id="c82d8-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="c82d8-119">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="c82d8-120">[chatMessage](../resources/chatmessage.md) (/теамс/{ИД}/чаннелс/{ИД}/мессажес)</span><span class="sxs-lookup"><span data-stu-id="c82d8-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="c82d8-121">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c82d8-121">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> | <span data-ttu-id="c82d8-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c82d8-122">Not supported</span></span> | <span data-ttu-id="c82d8-123">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="c82d8-123">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="c82d8-124">[chatMessage](../resources/chatmessage.md) (/теамс/аллмессажес--все сообщения каналов в организации)</span><span class="sxs-lookup"><span data-stu-id="c82d8-124">[chatMessage](../resources/chatmessage.md) (/teams/allMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="c82d8-125">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c82d8-125">Not supported</span></span> | <span data-ttu-id="c82d8-126">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c82d8-126">Not supported</span></span> | <span data-ttu-id="c82d8-127">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="c82d8-127">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="c82d8-128">[chatMessage](../resources/chatmessage.md) (/ЧАТС/{ИД}/мессажес)</span><span class="sxs-lookup"><span data-stu-id="c82d8-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="c82d8-129">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c82d8-129">Chat.Read, Chat.ReadWrite</span></span> | <span data-ttu-id="c82d8-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c82d8-130">Not supported</span></span> | <span data-ttu-id="c82d8-131">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="c82d8-131">Chat.Read.All</span></span>  |
|<span data-ttu-id="c82d8-132">[chatMessage](../resources/chatmessage.md) (/ЧАТС/аллмессажес--все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="c82d8-132">[chatMessage](../resources/chatmessage.md) (/chats/allMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="c82d8-133">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c82d8-133">Not supported</span></span> | <span data-ttu-id="c82d8-134">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c82d8-134">Not supported</span></span> | <span data-ttu-id="c82d8-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="c82d8-135">Chat.Read.All</span></span>  |
|[<span data-ttu-id="c82d8-136">contact</span><span class="sxs-lookup"><span data-stu-id="c82d8-136">contact</span></span>](../resources/contact.md) | <span data-ttu-id="c82d8-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="c82d8-137">Contacts.Read</span></span> | <span data-ttu-id="c82d8-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="c82d8-138">Contacts.Read</span></span> | <span data-ttu-id="c82d8-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="c82d8-139">Contacts.Read</span></span> |
|<span data-ttu-id="c82d8-140">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="c82d8-140">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="c82d8-141">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c82d8-141">Not supported</span></span> | <span data-ttu-id="c82d8-142">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c82d8-142">Files.ReadWrite</span></span> | <span data-ttu-id="c82d8-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c82d8-143">Not supported</span></span> |
|<span data-ttu-id="c82d8-144">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="c82d8-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="c82d8-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c82d8-145">Files.ReadWrite.All</span></span> | <span data-ttu-id="c82d8-146">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c82d8-146">Not supported</span></span> | <span data-ttu-id="c82d8-147">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c82d8-147">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="c82d8-148">event</span><span class="sxs-lookup"><span data-stu-id="c82d8-148">event</span></span>](../resources/event.md) | <span data-ttu-id="c82d8-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c82d8-149">Calendars.Read</span></span> | <span data-ttu-id="c82d8-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c82d8-150">Calendars.Read</span></span> | <span data-ttu-id="c82d8-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="c82d8-151">Calendars.Read</span></span> |
|[<span data-ttu-id="c82d8-152">group</span><span class="sxs-lookup"><span data-stu-id="c82d8-152">group</span></span>](../resources/group.md) | <span data-ttu-id="c82d8-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c82d8-153">Group.Read.All</span></span> | <span data-ttu-id="c82d8-154">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c82d8-154">Not supported</span></span> | <span data-ttu-id="c82d8-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c82d8-155">Group.Read.All</span></span> |
|[<span data-ttu-id="c82d8-156">group conversation</span><span class="sxs-lookup"><span data-stu-id="c82d8-156">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="c82d8-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="c82d8-157">Group.Read.All</span></span> | <span data-ttu-id="c82d8-158">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c82d8-158">Not supported</span></span> | <span data-ttu-id="c82d8-159">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c82d8-159">Not supported</span></span> |
|[<span data-ttu-id="c82d8-160">list</span><span class="sxs-lookup"><span data-stu-id="c82d8-160">list</span></span>](../resources/list.md) | <span data-ttu-id="c82d8-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c82d8-161">Sites.ReadWrite.All</span></span> | <span data-ttu-id="c82d8-162">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c82d8-162">Not supported</span></span> | <span data-ttu-id="c82d8-163">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c82d8-163">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="c82d8-164">message</span><span class="sxs-lookup"><span data-stu-id="c82d8-164">message</span></span>](../resources/message.md) | <span data-ttu-id="c82d8-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c82d8-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="c82d8-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c82d8-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="c82d8-167">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c82d8-167">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="c82d8-168">presence</span><span class="sxs-lookup"><span data-stu-id="c82d8-168">presence</span></span>](../resources/presence.md) | <span data-ttu-id="c82d8-169">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="c82d8-169">Presence.Read.All</span></span> | <span data-ttu-id="c82d8-170">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c82d8-170">Not supported</span></span> | <span data-ttu-id="c82d8-171">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c82d8-171">Not supported</span></span> |
|[<span data-ttu-id="c82d8-172">security alert</span><span class="sxs-lookup"><span data-stu-id="c82d8-172">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="c82d8-173">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c82d8-173">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="c82d8-174">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="c82d8-174">Not supported</span></span> | <span data-ttu-id="c82d8-175">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c82d8-175">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="c82d8-176">user</span><span class="sxs-lookup"><span data-stu-id="c82d8-176">user</span></span>](../resources/user.md) | <span data-ttu-id="c82d8-177">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="c82d8-177">User.Read.All</span></span> | <span data-ttu-id="c82d8-178">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="c82d8-178">User.Read.All</span></span> | <span data-ttu-id="c82d8-179">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="c82d8-179">User.Read.All</span></span> |

### <a name="chatmessage"></a><span data-ttu-id="c82d8-180">chatMessage</span><span class="sxs-lookup"><span data-stu-id="c82d8-180">chatMessage</span></span>

<span data-ttu-id="c82d8-181">подписки **chatMessage** с делегированными разрешениями не поддерживают данные ресурсов (**инклудересаурцедата** должны быть `false` ) и не требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="c82d8-181">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="c82d8-182">подписки **chatMessage** с разрешениями приложений включают данные ресурсов и требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="c82d8-182">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="c82d8-183">Если [енкриптионцертификате](../resources/subscription.md) не указан, создание подписки завершится с ошибками.</span><span class="sxs-lookup"><span data-stu-id="c82d8-183">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="c82d8-184">Перед созданием подписки на **chatMessage** необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="c82d8-184">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="c82d8-185">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="c82d8-185">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="c82d8-186">**Примечание:** `/teams/allMessages` и `/chats/allMessages` в настоящее время находятся в предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="c82d8-186">**Note:** `/teams/allMessages` and `/chats/allMessages` are currently in preview.</span></span> <span data-ttu-id="c82d8-187">Во время предварительной версии вы можете использовать этот API без сборов в соответствии с [условиями использования API Майкрософт](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context).</span><span class="sxs-lookup"><span data-stu-id="c82d8-187">During the preview, you may use this API without fees, subject to the [Microsoft APIs Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use?context=graph/context).</span></span> <span data-ttu-id="c82d8-188">Однако пользователям приложений, использующих API, может потребоваться подписка на конкретные решения Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c82d8-188">However, users of apps that use the API might be required to have subscriptions to specific Microsoft 365 offerings.</span></span> <span data-ttu-id="c82d8-189">После общедоступной доступности Корпорация Майкрософт может потребовать от вас или ваших клиентов взимать дополнительные сборы на основе объема данных, доступ к которым осуществляется через API.</span><span class="sxs-lookup"><span data-stu-id="c82d8-189">Upon general availability, Microsoft may require you or your customers to pay additional fees based on the amount of data accessed through the API.</span></span>

### <a name="driveitem"></a><span data-ttu-id="c82d8-190">driveItem</span><span class="sxs-lookup"><span data-stu-id="c82d8-190">driveItem</span></span>

<span data-ttu-id="c82d8-191">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c82d8-191">Additional limitations apply for subscriptions on OneDrive  items.</span></span> <span data-ttu-id="c82d8-192">Ограничения применяются к созданию и управлению (получению, обновлению и удалению) подписок.</span><span class="sxs-lookup"><span data-stu-id="c82d8-192">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="c82d8-193">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="c82d8-193">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="c82d8-194">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="c82d8-194">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="c82d8-195">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="c82d8-195">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="c82d8-196">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="c82d8-196">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="c82d8-197">контакты, события и сообщения</span><span class="sxs-lookup"><span data-stu-id="c82d8-197">contact, event, and message</span></span>

<span data-ttu-id="c82d8-198">Дополнительные ограничения применяются для подписок на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="c82d8-198">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="c82d8-199">Ограничения применяются к созданию и управлению (получению, обновлению и удалению) подписок.</span><span class="sxs-lookup"><span data-stu-id="c82d8-199">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="c82d8-200">Делегированное разрешение поддерживает подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="c82d8-200">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="c82d8-201">Это означает, например, что нельзя использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="c82d8-201">That means, for example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="c82d8-202">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="c82d8-202">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="c82d8-203">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="c82d8-203">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="c82d8-204">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="c82d8-204">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

### <a name="presence"></a><span data-ttu-id="c82d8-205">presence</span><span class="sxs-lookup"><span data-stu-id="c82d8-205">presence</span></span>

<span data-ttu-id="c82d8-206">для подписок на **присутствие** требуется [Шифрование](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="c82d8-206">**presence** subscriptions require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="c82d8-207">Если [енкриптионцертификате](../resources/subscription.md) не указан, создание подписки завершится с ошибками.</span><span class="sxs-lookup"><span data-stu-id="c82d8-207">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span>

## <a name="http-request"></a><span data-ttu-id="c82d8-208">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c82d8-208">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c82d8-209">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c82d8-209">Request headers</span></span>

| <span data-ttu-id="c82d8-210">Имя</span><span class="sxs-lookup"><span data-stu-id="c82d8-210">Name</span></span>       | <span data-ttu-id="c82d8-211">Тип</span><span class="sxs-lookup"><span data-stu-id="c82d8-211">Type</span></span> | <span data-ttu-id="c82d8-212">Описание</span><span class="sxs-lookup"><span data-stu-id="c82d8-212">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c82d8-213">Authorization</span><span class="sxs-lookup"><span data-stu-id="c82d8-213">Authorization</span></span>  | <span data-ttu-id="c82d8-214">string</span><span class="sxs-lookup"><span data-stu-id="c82d8-214">string</span></span>  | <span data-ttu-id="c82d8-p110">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c82d8-p110">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c82d8-217">Отклик</span><span class="sxs-lookup"><span data-stu-id="c82d8-217">Response</span></span>

<span data-ttu-id="c82d8-218">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c82d8-218">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="c82d8-219">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="c82d8-219">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="c82d8-220">Пример</span><span class="sxs-lookup"><span data-stu-id="c82d8-220">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c82d8-221">Запрос</span><span class="sxs-lookup"><span data-stu-id="c82d8-221">Request</span></span>

<span data-ttu-id="c82d8-222">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c82d8-222">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c82d8-223">HTTP</span><span class="sxs-lookup"><span data-stu-id="c82d8-223">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c82d8-224">C#</span><span class="sxs-lookup"><span data-stu-id="c82d8-224">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c82d8-225">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c82d8-225">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c82d8-226">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c82d8-226">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c82d8-227">Отклик</span><span class="sxs-lookup"><span data-stu-id="c82d8-227">Response</span></span>

<span data-ttu-id="c82d8-228">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c82d8-228">Here is an example of the response.</span></span>
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
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2"
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
