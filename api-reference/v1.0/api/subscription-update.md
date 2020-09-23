---
title: Обновление подписки
description: Возобновление подписки путем увеличения срока действия.
localization_priority: Normal
author: davidmu1
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 7b50b6b32bf3d5927d13d0f5ad146949a858dd1e
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193565"
---
# <a name="update-subscription"></a><span data-ttu-id="85ca9-103">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="85ca9-103">Update subscription</span></span>

<span data-ttu-id="85ca9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85ca9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="85ca9-105">Возобновление подписки путем увеличения срока действия.</span><span class="sxs-lookup"><span data-stu-id="85ca9-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="85ca9-106">Срок действия подписок истечет через период времени, который зависит от типа ресурса.</span><span class="sxs-lookup"><span data-stu-id="85ca9-106">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="85ca9-107">Чтобы избежать отсутствия уведомлений об изменениях, приложение должно правильно обновить свои подписки до истечения срока их действия.</span><span class="sxs-lookup"><span data-stu-id="85ca9-107">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="85ca9-108">В этой [статье приведены сведения](../resources/subscription.md) о максимальной длине подписки для каждого типа ресурсов.</span><span class="sxs-lookup"><span data-stu-id="85ca9-108">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="85ca9-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="85ca9-109">Permissions</span></span>

<span data-ttu-id="85ca9-110">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="85ca9-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="85ca9-111">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85ca9-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="85ca9-112">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="85ca9-112">Supported resource</span></span> | <span data-ttu-id="85ca9-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85ca9-113">Delegated (work or school account)</span></span> | <span data-ttu-id="85ca9-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85ca9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85ca9-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="85ca9-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="85ca9-116">callRecord</span><span class="sxs-lookup"><span data-stu-id="85ca9-116">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="85ca9-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="85ca9-117">Not supported</span></span> | <span data-ttu-id="85ca9-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="85ca9-118">Not supported</span></span> | <span data-ttu-id="85ca9-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="85ca9-119">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="85ca9-120">[chatMessage](../resources/chatmessage.md) (/теамс/{ИД}/чаннелс/{ИД}/мессажес)</span><span class="sxs-lookup"><span data-stu-id="85ca9-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="85ca9-121">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="85ca9-121">Not supported</span></span> | <span data-ttu-id="85ca9-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="85ca9-122">Not supported</span></span> | <span data-ttu-id="85ca9-123">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="85ca9-123">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="85ca9-124">[chatMessage](../resources/chatmessage.md) (/теамс/жеталлмессажес--все сообщения каналов в организации)</span><span class="sxs-lookup"><span data-stu-id="85ca9-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="85ca9-125">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="85ca9-125">Not supported</span></span> | <span data-ttu-id="85ca9-126">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="85ca9-126">Not supported</span></span> | <span data-ttu-id="85ca9-127">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="85ca9-127">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="85ca9-128">[chatMessage](../resources/chatmessage.md) (/ЧАТС/{ИД}/мессажес)</span><span class="sxs-lookup"><span data-stu-id="85ca9-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="85ca9-129">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="85ca9-129">Not supported</span></span> | <span data-ttu-id="85ca9-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="85ca9-130">Not supported</span></span> | <span data-ttu-id="85ca9-131">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="85ca9-131">Chat.Read.All</span></span>  |
|<span data-ttu-id="85ca9-132">[chatMessage](../resources/chatmessage.md) (/ЧАТС/жеталлмессажес--все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="85ca9-132">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="85ca9-133">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="85ca9-133">Not supported</span></span> | <span data-ttu-id="85ca9-134">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="85ca9-134">Not supported</span></span> | <span data-ttu-id="85ca9-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="85ca9-135">Chat.Read.All</span></span>  |
|[<span data-ttu-id="85ca9-136">contact</span><span class="sxs-lookup"><span data-stu-id="85ca9-136">contact</span></span>](../resources/contact.md) | <span data-ttu-id="85ca9-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="85ca9-137">Contacts.Read</span></span> | <span data-ttu-id="85ca9-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="85ca9-138">Contacts.Read</span></span> | <span data-ttu-id="85ca9-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="85ca9-139">Contacts.Read</span></span> |
|<span data-ttu-id="85ca9-140">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="85ca9-140">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="85ca9-141">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="85ca9-141">Not supported</span></span> | <span data-ttu-id="85ca9-142">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85ca9-142">Files.ReadWrite</span></span> | <span data-ttu-id="85ca9-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="85ca9-143">Not supported</span></span> |
|<span data-ttu-id="85ca9-144">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="85ca9-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="85ca9-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85ca9-145">Files.ReadWrite.All</span></span> | <span data-ttu-id="85ca9-146">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="85ca9-146">Not supported</span></span> | <span data-ttu-id="85ca9-147">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85ca9-147">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="85ca9-148">event</span><span class="sxs-lookup"><span data-stu-id="85ca9-148">event</span></span>](../resources/event.md) | <span data-ttu-id="85ca9-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="85ca9-149">Calendars.Read</span></span> | <span data-ttu-id="85ca9-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="85ca9-150">Calendars.Read</span></span> | <span data-ttu-id="85ca9-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="85ca9-151">Calendars.Read</span></span> |
|[<span data-ttu-id="85ca9-152">group</span><span class="sxs-lookup"><span data-stu-id="85ca9-152">group</span></span>](../resources/group.md) | <span data-ttu-id="85ca9-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="85ca9-153">Group.Read.All</span></span> | <span data-ttu-id="85ca9-154">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="85ca9-154">Not supported</span></span> | <span data-ttu-id="85ca9-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="85ca9-155">Group.Read.All</span></span> |
|[<span data-ttu-id="85ca9-156">group conversation</span><span class="sxs-lookup"><span data-stu-id="85ca9-156">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="85ca9-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="85ca9-157">Group.Read.All</span></span> | <span data-ttu-id="85ca9-158">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="85ca9-158">Not supported</span></span> | <span data-ttu-id="85ca9-159">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="85ca9-159">Not supported</span></span> |
|[<span data-ttu-id="85ca9-160">list</span><span class="sxs-lookup"><span data-stu-id="85ca9-160">list</span></span>](../resources/list.md) | <span data-ttu-id="85ca9-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85ca9-161">Sites.ReadWrite.All</span></span> | <span data-ttu-id="85ca9-162">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="85ca9-162">Not supported</span></span> | <span data-ttu-id="85ca9-163">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85ca9-163">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="85ca9-164">message</span><span class="sxs-lookup"><span data-stu-id="85ca9-164">message</span></span>](../resources/message.md) | <span data-ttu-id="85ca9-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="85ca9-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="85ca9-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="85ca9-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="85ca9-167">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="85ca9-167">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="85ca9-168">security alert</span><span class="sxs-lookup"><span data-stu-id="85ca9-168">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="85ca9-169">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85ca9-169">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="85ca9-170">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="85ca9-170">Not supported</span></span> | <span data-ttu-id="85ca9-171">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85ca9-171">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="85ca9-172">user</span><span class="sxs-lookup"><span data-stu-id="85ca9-172">user</span></span>](../resources/user.md) | <span data-ttu-id="85ca9-173">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="85ca9-173">User.Read.All</span></span> | <span data-ttu-id="85ca9-174">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="85ca9-174">User.Read.All</span></span> | <span data-ttu-id="85ca9-175">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="85ca9-175">User.Read.All</span></span> |

### <a name="chatmessage"></a><span data-ttu-id="85ca9-176">chatMessage</span><span class="sxs-lookup"><span data-stu-id="85ca9-176">chatMessage</span></span>

<span data-ttu-id="85ca9-177">подписки **chatMessage** с разрешениями приложений включают данные ресурсов и требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="85ca9-177">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="85ca9-178">Если [енкриптионцертификате](../resources/subscription.md) не указан, создание подписки завершится с ошибками.</span><span class="sxs-lookup"><span data-stu-id="85ca9-178">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="85ca9-179">Перед созданием подписки на **chatMessage** необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="85ca9-179">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="85ca9-180">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="85ca9-180">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="85ca9-181">**Примечание:** `/teams/getAllMessages` и `/chats/getAllMessages` доступны пользователям, у которых есть  
 [необходимые лицензии](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="85ca9-181">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the 
[required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

### <a name="driveitem"></a><span data-ttu-id="85ca9-182">driveItem</span><span class="sxs-lookup"><span data-stu-id="85ca9-182">driveItem</span></span>

<span data-ttu-id="85ca9-183">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="85ca9-183">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="85ca9-184">Ограничения применяются к созданию и управлению (получению, обновлению и удалению) подписок.</span><span class="sxs-lookup"><span data-stu-id="85ca9-184">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="85ca9-185">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="85ca9-185">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="85ca9-186">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="85ca9-186">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="85ca9-187">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="85ca9-187">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="85ca9-188">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="85ca9-188">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="85ca9-189">контакты, события и сообщения</span><span class="sxs-lookup"><span data-stu-id="85ca9-189">contact, event, and message</span></span>

<span data-ttu-id="85ca9-190">Дополнительные ограничения применяются для подписок на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="85ca9-190">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="85ca9-191">Ограничения применяются к созданию и управлению (получению, обновлению и удалению) подписок.</span><span class="sxs-lookup"><span data-stu-id="85ca9-191">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="85ca9-192">Делегированное разрешение поддерживает подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="85ca9-192">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="85ca9-193">Например, нельзя использовать делегированные календари разрешений. Read для подписки на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="85ca9-193">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="85ca9-194">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="85ca9-194">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="85ca9-195">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="85ca9-195">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="85ca9-196">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="85ca9-196">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="85ca9-197">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85ca9-197">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="85ca9-198">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85ca9-198">Request headers</span></span>

| <span data-ttu-id="85ca9-199">Имя</span><span class="sxs-lookup"><span data-stu-id="85ca9-199">Name</span></span>       | <span data-ttu-id="85ca9-200">Тип</span><span class="sxs-lookup"><span data-stu-id="85ca9-200">Type</span></span> | <span data-ttu-id="85ca9-201">Описание</span><span class="sxs-lookup"><span data-stu-id="85ca9-201">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="85ca9-202">Authorization</span><span class="sxs-lookup"><span data-stu-id="85ca9-202">Authorization</span></span>  | <span data-ttu-id="85ca9-203">string</span><span class="sxs-lookup"><span data-stu-id="85ca9-203">string</span></span>  | <span data-ttu-id="85ca9-p108">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85ca9-p108">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="85ca9-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="85ca9-206">Response</span></span>

<span data-ttu-id="85ca9-207">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="85ca9-207">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="85ca9-208">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="85ca9-208">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="85ca9-209">Пример</span><span class="sxs-lookup"><span data-stu-id="85ca9-209">Example</span></span>

##### <a name="request"></a><span data-ttu-id="85ca9-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="85ca9-210">Request</span></span>

<span data-ttu-id="85ca9-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85ca9-211">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="85ca9-212">HTTP</span><span class="sxs-lookup"><span data-stu-id="85ca9-212">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```
# <a name="c"></a>[<span data-ttu-id="85ca9-213">C#</span><span class="sxs-lookup"><span data-stu-id="85ca9-213">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="85ca9-214">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85ca9-214">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="85ca9-215">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85ca9-215">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="85ca9-216">Java</span><span class="sxs-lookup"><span data-stu-id="85ca9-216">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="85ca9-217">Отклик</span><span class="sxs-lookup"><span data-stu-id="85ca9-217">Response</span></span>

<span data-ttu-id="85ca9-218">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="85ca9-218">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
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
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2",
  "encryptionCertificate": "",
  "encryptionCertificateId": "",
  "includeResourceData": false
}
```

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

