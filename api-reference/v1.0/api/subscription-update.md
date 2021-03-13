---
title: Обновление подписки
description: Возобновление подписки путем увеличения срока действия.
localization_priority: Normal
author: davidmu1
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: e63f810e6e11d18d2e03fb702a629cee74d768fe
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50759505"
---
# <a name="update-subscription"></a><span data-ttu-id="a3c85-103">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="a3c85-103">Update subscription</span></span>

<span data-ttu-id="a3c85-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3c85-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a3c85-105">Возобновление подписки путем увеличения срока действия.</span><span class="sxs-lookup"><span data-stu-id="a3c85-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="a3c85-106">В таблице в разделе [Разрешения](#permissions) перечислены ресурсы, поддерживаюющие подписку на изменение уведомлений.</span><span class="sxs-lookup"><span data-stu-id="a3c85-106">The table in the [Permissions](#permissions) section lists the resources that support subscribing to change notifications.</span></span>

<span data-ttu-id="a3c85-107">Срок действия подписки истекает по истечении времени, которое зависит от типа ресурса.</span><span class="sxs-lookup"><span data-stu-id="a3c85-107">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="a3c85-108">Чтобы избежать пропуска уведомлений об изменениях, приложение должно продлить подписки заблаговременно до истечения срока их действия.</span><span class="sxs-lookup"><span data-stu-id="a3c85-108">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="a3c85-109">См. [подписку](../resources/subscription.md) на максимальную длину подписки для каждого типа ресурсов.</span><span class="sxs-lookup"><span data-stu-id="a3c85-109">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3c85-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a3c85-110">Permissions</span></span>

<span data-ttu-id="a3c85-111">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a3c85-111">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="a3c85-112">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3c85-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a3c85-113">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="a3c85-113">Supported resource</span></span> | <span data-ttu-id="a3c85-114">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3c85-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a3c85-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3c85-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3c85-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="a3c85-116">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="a3c85-117">callRecord</span><span class="sxs-lookup"><span data-stu-id="a3c85-117">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="a3c85-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a3c85-118">Not supported</span></span> | <span data-ttu-id="a3c85-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a3c85-119">Not supported</span></span> | <span data-ttu-id="a3c85-120">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3c85-120">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="a3c85-121">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="a3c85-121">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="a3c85-122">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3c85-122">ChannelMessage.Read.All</span></span> | <span data-ttu-id="a3c85-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a3c85-123">Not supported</span></span> |  <span data-ttu-id="a3c85-124">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3c85-124">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="a3c85-125">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="a3c85-125">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="a3c85-126">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a3c85-126">Not supported</span></span> | <span data-ttu-id="a3c85-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a3c85-127">Not supported</span></span> | <span data-ttu-id="a3c85-128">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3c85-128">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="a3c85-129">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="a3c85-129">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="a3c85-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a3c85-130">Not supported</span></span> | <span data-ttu-id="a3c85-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a3c85-131">Not supported</span></span> | <span data-ttu-id="a3c85-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3c85-132">Chat.Read.All</span></span>  |
|<span data-ttu-id="a3c85-133">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="a3c85-133">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="a3c85-134">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a3c85-134">Not supported</span></span> | <span data-ttu-id="a3c85-135">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a3c85-135">Not supported</span></span> | <span data-ttu-id="a3c85-136">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3c85-136">Chat.Read.All</span></span>  |
|[<span data-ttu-id="a3c85-137">contact</span><span class="sxs-lookup"><span data-stu-id="a3c85-137">contact</span></span>](../resources/contact.md) | <span data-ttu-id="a3c85-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a3c85-138">Contacts.Read</span></span> | <span data-ttu-id="a3c85-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a3c85-139">Contacts.Read</span></span> | <span data-ttu-id="a3c85-140">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="a3c85-140">Contacts.Read</span></span> |
|<span data-ttu-id="a3c85-141">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="a3c85-141">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="a3c85-142">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a3c85-142">Not supported</span></span> | <span data-ttu-id="a3c85-143">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a3c85-143">Files.ReadWrite</span></span> | <span data-ttu-id="a3c85-144">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a3c85-144">Not supported</span></span> |
|<span data-ttu-id="a3c85-145">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="a3c85-145">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="a3c85-146">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3c85-146">Files.ReadWrite.All</span></span> | <span data-ttu-id="a3c85-147">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a3c85-147">Not supported</span></span> | <span data-ttu-id="a3c85-148">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3c85-148">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="a3c85-149">event</span><span class="sxs-lookup"><span data-stu-id="a3c85-149">event</span></span>](../resources/event.md) | <span data-ttu-id="a3c85-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a3c85-150">Calendars.Read</span></span> | <span data-ttu-id="a3c85-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a3c85-151">Calendars.Read</span></span> | <span data-ttu-id="a3c85-152">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a3c85-152">Calendars.Read</span></span> |
|[<span data-ttu-id="a3c85-153">group</span><span class="sxs-lookup"><span data-stu-id="a3c85-153">group</span></span>](../resources/group.md) | <span data-ttu-id="a3c85-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3c85-154">Group.Read.All</span></span> | <span data-ttu-id="a3c85-155">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a3c85-155">Not supported</span></span> | <span data-ttu-id="a3c85-156">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3c85-156">Group.Read.All</span></span> |
|[<span data-ttu-id="a3c85-157">group conversation</span><span class="sxs-lookup"><span data-stu-id="a3c85-157">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="a3c85-158">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3c85-158">Group.Read.All</span></span> | <span data-ttu-id="a3c85-159">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a3c85-159">Not supported</span></span> | <span data-ttu-id="a3c85-160">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a3c85-160">Not supported</span></span> |
|[<span data-ttu-id="a3c85-161">list</span><span class="sxs-lookup"><span data-stu-id="a3c85-161">list</span></span>](../resources/list.md) | <span data-ttu-id="a3c85-162">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3c85-162">Sites.ReadWrite.All</span></span> | <span data-ttu-id="a3c85-163">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a3c85-163">Not supported</span></span> | <span data-ttu-id="a3c85-164">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3c85-164">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="a3c85-165">message</span><span class="sxs-lookup"><span data-stu-id="a3c85-165">message</span></span>](../resources/message.md) | <span data-ttu-id="a3c85-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a3c85-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="a3c85-167">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a3c85-167">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="a3c85-168">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a3c85-168">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="a3c85-169">security alert</span><span class="sxs-lookup"><span data-stu-id="a3c85-169">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="a3c85-170">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3c85-170">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="a3c85-171">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="a3c85-171">Not supported</span></span> | <span data-ttu-id="a3c85-172">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3c85-172">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="a3c85-173">user</span><span class="sxs-lookup"><span data-stu-id="a3c85-173">user</span></span>](../resources/user.md) | <span data-ttu-id="a3c85-174">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3c85-174">User.Read.All</span></span> | <span data-ttu-id="a3c85-175">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3c85-175">User.Read.All</span></span> | <span data-ttu-id="a3c85-176">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3c85-176">User.Read.All</span></span> |

> <span data-ttu-id="a3c85-177">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="a3c85-177">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

[!INCLUDE [teams-subscription-notes](../../includes/teams-subscription-notes.md)]

### <a name="driveitem"></a><span data-ttu-id="a3c85-178">driveItem</span><span class="sxs-lookup"><span data-stu-id="a3c85-178">driveItem</span></span>

<span data-ttu-id="a3c85-179">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a3c85-179">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="a3c85-180">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="a3c85-180">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="a3c85-181">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="a3c85-181">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="a3c85-182">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="a3c85-182">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="a3c85-183">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="a3c85-183">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="a3c85-184">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="a3c85-184">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="a3c85-185">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="a3c85-185">contact, event, and message</span></span>

<span data-ttu-id="a3c85-186">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="a3c85-186">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="a3c85-187">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="a3c85-187">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="a3c85-188">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="a3c85-188">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="a3c85-189">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="a3c85-189">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="a3c85-190">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="a3c85-190">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="a3c85-191">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="a3c85-191">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="a3c85-192">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="a3c85-192">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="a3c85-193">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3c85-193">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a3c85-194">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3c85-194">Request headers</span></span>

| <span data-ttu-id="a3c85-195">Имя</span><span class="sxs-lookup"><span data-stu-id="a3c85-195">Name</span></span>       | <span data-ttu-id="a3c85-196">Тип</span><span class="sxs-lookup"><span data-stu-id="a3c85-196">Type</span></span> | <span data-ttu-id="a3c85-197">Описание</span><span class="sxs-lookup"><span data-stu-id="a3c85-197">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a3c85-198">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3c85-198">Authorization</span></span>  | <span data-ttu-id="a3c85-199">string</span><span class="sxs-lookup"><span data-stu-id="a3c85-199">string</span></span>  | <span data-ttu-id="a3c85-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a3c85-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a3c85-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3c85-202">Response</span></span>

<span data-ttu-id="a3c85-203">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a3c85-203">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="a3c85-204">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="a3c85-204">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="a3c85-205">Пример</span><span class="sxs-lookup"><span data-stu-id="a3c85-205">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a3c85-206">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3c85-206">Request</span></span>

<span data-ttu-id="a3c85-207">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3c85-207">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a3c85-208">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3c85-208">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a3c85-209">C#</span><span class="sxs-lookup"><span data-stu-id="a3c85-209">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a3c85-210">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3c85-210">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a3c85-211">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3c85-211">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a3c85-212">Java</span><span class="sxs-lookup"><span data-stu-id="a3c85-212">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a3c85-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3c85-213">Response</span></span>

<span data-ttu-id="a3c85-214">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a3c85-214">Here is an example of the response.</span></span>
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
  "lifecycleNotificationUrl":"https://webhook.azurewebsites.net/api/send/lifecycleNotifications",
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

