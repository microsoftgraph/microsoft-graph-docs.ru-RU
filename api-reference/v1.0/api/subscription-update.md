---
title: Обновление подписки
description: Возобновление подписки путем увеличения срока действия.
localization_priority: Normal
author: davidmu1
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 5221f855df88103808f561d720f49c812911355e
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48849097"
---
# <a name="update-subscription"></a><span data-ttu-id="24168-103">Обновление подписки</span><span class="sxs-lookup"><span data-stu-id="24168-103">Update subscription</span></span>

<span data-ttu-id="24168-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24168-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="24168-105">Возобновление подписки путем увеличения срока действия.</span><span class="sxs-lookup"><span data-stu-id="24168-105">Renew a subscription by extending its expiry time.</span></span>

<span data-ttu-id="24168-106">Срок действия подписок истечет через период времени, который зависит от типа ресурса.</span><span class="sxs-lookup"><span data-stu-id="24168-106">Subscriptions expire after a length of time that varies by resource type.</span></span> <span data-ttu-id="24168-107">Чтобы избежать отсутствия уведомлений об изменениях, приложение должно правильно обновить свои подписки до истечения срока их действия.</span><span class="sxs-lookup"><span data-stu-id="24168-107">In order to avoid missing change notifications, an app should renew its subscriptions well in advance of their expiry date.</span></span> <span data-ttu-id="24168-108">В этой [статье приведены сведения](../resources/subscription.md) о максимальной длине подписки для каждого типа ресурсов.</span><span class="sxs-lookup"><span data-stu-id="24168-108">See [subscription](../resources/subscription.md) for maximum length of a subscription for each resource type.</span></span>

## <a name="permissions"></a><span data-ttu-id="24168-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="24168-109">Permissions</span></span>

<span data-ttu-id="24168-110">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="24168-110">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="24168-111">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24168-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="24168-112">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="24168-112">Supported resource</span></span> | <span data-ttu-id="24168-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24168-113">Delegated (work or school account)</span></span> | <span data-ttu-id="24168-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24168-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24168-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="24168-115">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="24168-116">callRecord</span><span class="sxs-lookup"><span data-stu-id="24168-116">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="24168-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="24168-117">Not supported</span></span> | <span data-ttu-id="24168-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="24168-118">Not supported</span></span> | <span data-ttu-id="24168-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="24168-119">CallRecords.Read.All</span></span>  |
|<span data-ttu-id="24168-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="24168-120">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="24168-121">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="24168-121">Not supported</span></span> | <span data-ttu-id="24168-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="24168-122">Not supported</span></span> |  <span data-ttu-id="24168-123">Чаннелмессаже. Read. Group \*, Чаннелмессаже. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="24168-123">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="24168-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="24168-124">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="24168-125">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="24168-125">Not supported</span></span> | <span data-ttu-id="24168-126">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="24168-126">Not supported</span></span> | <span data-ttu-id="24168-127">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="24168-127">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="24168-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="24168-128">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="24168-129">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="24168-129">Not supported</span></span> | <span data-ttu-id="24168-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="24168-130">Not supported</span></span> | <span data-ttu-id="24168-131">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="24168-131">Chat.Read.All</span></span>  |
|<span data-ttu-id="24168-132">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="24168-132">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="24168-133">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="24168-133">Not supported</span></span> | <span data-ttu-id="24168-134">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="24168-134">Not supported</span></span> | <span data-ttu-id="24168-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="24168-135">Chat.Read.All</span></span>  |
|[<span data-ttu-id="24168-136">contact</span><span class="sxs-lookup"><span data-stu-id="24168-136">contact</span></span>](../resources/contact.md) | <span data-ttu-id="24168-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="24168-137">Contacts.Read</span></span> | <span data-ttu-id="24168-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="24168-138">Contacts.Read</span></span> | <span data-ttu-id="24168-139">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="24168-139">Contacts.Read</span></span> |
|<span data-ttu-id="24168-140">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="24168-140">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="24168-141">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="24168-141">Not supported</span></span> | <span data-ttu-id="24168-142">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="24168-142">Files.ReadWrite</span></span> | <span data-ttu-id="24168-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="24168-143">Not supported</span></span> |
|<span data-ttu-id="24168-144">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="24168-144">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="24168-145">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24168-145">Files.ReadWrite.All</span></span> | <span data-ttu-id="24168-146">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="24168-146">Not supported</span></span> | <span data-ttu-id="24168-147">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24168-147">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="24168-148">event</span><span class="sxs-lookup"><span data-stu-id="24168-148">event</span></span>](../resources/event.md) | <span data-ttu-id="24168-149">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="24168-149">Calendars.Read</span></span> | <span data-ttu-id="24168-150">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="24168-150">Calendars.Read</span></span> | <span data-ttu-id="24168-151">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="24168-151">Calendars.Read</span></span> |
|[<span data-ttu-id="24168-152">group</span><span class="sxs-lookup"><span data-stu-id="24168-152">group</span></span>](../resources/group.md) | <span data-ttu-id="24168-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="24168-153">Group.Read.All</span></span> | <span data-ttu-id="24168-154">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="24168-154">Not supported</span></span> | <span data-ttu-id="24168-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="24168-155">Group.Read.All</span></span> |
|[<span data-ttu-id="24168-156">group conversation</span><span class="sxs-lookup"><span data-stu-id="24168-156">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="24168-157">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="24168-157">Group.Read.All</span></span> | <span data-ttu-id="24168-158">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="24168-158">Not supported</span></span> | <span data-ttu-id="24168-159">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="24168-159">Not supported</span></span> |
|[<span data-ttu-id="24168-160">list</span><span class="sxs-lookup"><span data-stu-id="24168-160">list</span></span>](../resources/list.md) | <span data-ttu-id="24168-161">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24168-161">Sites.ReadWrite.All</span></span> | <span data-ttu-id="24168-162">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="24168-162">Not supported</span></span> | <span data-ttu-id="24168-163">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24168-163">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="24168-164">message</span><span class="sxs-lookup"><span data-stu-id="24168-164">message</span></span>](../resources/message.md) | <span data-ttu-id="24168-165">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="24168-165">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="24168-166">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="24168-166">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="24168-167">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="24168-167">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="24168-168">security alert</span><span class="sxs-lookup"><span data-stu-id="24168-168">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="24168-169">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24168-169">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="24168-170">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="24168-170">Not supported</span></span> | <span data-ttu-id="24168-171">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24168-171">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="24168-172">user</span><span class="sxs-lookup"><span data-stu-id="24168-172">user</span></span>](../resources/user.md) | <span data-ttu-id="24168-173">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="24168-173">User.Read.All</span></span> | <span data-ttu-id="24168-174">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="24168-174">User.Read.All</span></span> | <span data-ttu-id="24168-175">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="24168-175">User.Read.All</span></span> |

> <span data-ttu-id="24168-176">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="24168-176">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="chatmessage"></a><span data-ttu-id="24168-177">chatMessage</span><span class="sxs-lookup"><span data-stu-id="24168-177">chatMessage</span></span>

<span data-ttu-id="24168-178">Подписки **chatMessage** с разрешениями для приложений включают данные ресурса и требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="24168-178">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="24168-179">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="24168-179">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="24168-180">Перед созданием подписки **chatMessage** вы должны запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="24168-180">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="24168-181">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="24168-181">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="24168-182">**Примечание.** `/teams/getAllMessages` и `/chats/getAllMessages` доступны для пользователей с [требуемыми лицензиями](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="24168-182">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

### <a name="driveitem"></a><span data-ttu-id="24168-183">driveItem</span><span class="sxs-lookup"><span data-stu-id="24168-183">driveItem</span></span>

<span data-ttu-id="24168-184">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="24168-184">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="24168-185">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="24168-185">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="24168-186">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="24168-186">On personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="24168-187">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="24168-187">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="24168-188">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="24168-188">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="24168-189">Нельзя подписаться на экземпляры **drive** или **driveItem** , не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="24168-189">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="24168-190">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="24168-190">contact, event, and message</span></span>

<span data-ttu-id="24168-191">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="24168-191">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="24168-192">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="24168-192">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="24168-193">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="24168-193">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="24168-194">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="24168-194">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="24168-195">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="24168-195">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="24168-196">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="24168-196">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="24168-197">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="24168-197">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>

## <a name="http-request"></a><span data-ttu-id="24168-198">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24168-198">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a><span data-ttu-id="24168-199">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="24168-199">Request headers</span></span>

| <span data-ttu-id="24168-200">Имя</span><span class="sxs-lookup"><span data-stu-id="24168-200">Name</span></span>       | <span data-ttu-id="24168-201">Тип</span><span class="sxs-lookup"><span data-stu-id="24168-201">Type</span></span> | <span data-ttu-id="24168-202">Описание</span><span class="sxs-lookup"><span data-stu-id="24168-202">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="24168-203">Authorization</span><span class="sxs-lookup"><span data-stu-id="24168-203">Authorization</span></span>  | <span data-ttu-id="24168-204">string</span><span class="sxs-lookup"><span data-stu-id="24168-204">string</span></span>  | <span data-ttu-id="24168-p108">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24168-p108">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="24168-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="24168-207">Response</span></span>

<span data-ttu-id="24168-208">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="24168-208">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

<span data-ttu-id="24168-209">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="24168-209">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="24168-210">Пример</span><span class="sxs-lookup"><span data-stu-id="24168-210">Example</span></span>

##### <a name="request"></a><span data-ttu-id="24168-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="24168-211">Request</span></span>

<span data-ttu-id="24168-212">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24168-212">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="24168-213">HTTP</span><span class="sxs-lookup"><span data-stu-id="24168-213">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="24168-214">C#</span><span class="sxs-lookup"><span data-stu-id="24168-214">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="24168-215">JavaScript</span><span class="sxs-lookup"><span data-stu-id="24168-215">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="24168-216">Objective-C</span><span class="sxs-lookup"><span data-stu-id="24168-216">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="24168-217">Java</span><span class="sxs-lookup"><span data-stu-id="24168-217">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="24168-218">Отклик</span><span class="sxs-lookup"><span data-stu-id="24168-218">Response</span></span>

<span data-ttu-id="24168-219">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="24168-219">Here is an example of the response.</span></span>
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

