---
title: Удаление подписки
description: Удаление подписки.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c6d83614d082341502474aea261b201361df0249
ms.sourcegitcommit: 775b38baac6a4e7704d6144ef4589f2fc476bd61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/13/2020
ms.locfileid: "48433473"
---
# <a name="delete-subscription"></a><span data-ttu-id="dc4bf-103">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="dc4bf-103">Delete subscription</span></span>

<span data-ttu-id="dc4bf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc4bf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dc4bf-105">Удаление подписки.</span><span class="sxs-lookup"><span data-stu-id="dc4bf-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc4bf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dc4bf-106">Permissions</span></span>

<span data-ttu-id="dc4bf-107">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="dc4bf-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="dc4bf-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc4bf-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dc4bf-109">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="dc4bf-109">Supported resource</span></span> | <span data-ttu-id="dc4bf-110">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc4bf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dc4bf-111">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc4bf-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc4bf-112">Приложение</span><span class="sxs-lookup"><span data-stu-id="dc4bf-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="dc4bf-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="dc4bf-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="dc4bf-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dc4bf-114">Not supported</span></span> | <span data-ttu-id="dc4bf-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dc4bf-115">Not supported</span></span> | <span data-ttu-id="dc4bf-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc4bf-116">CallRecords.Read.All</span></span> |
|<span data-ttu-id="dc4bf-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="dc4bf-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="dc4bf-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dc4bf-118">Not supported</span></span> | <span data-ttu-id="dc4bf-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dc4bf-119">Not supported</span></span> | <span data-ttu-id="dc4bf-120">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc4bf-120">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="dc4bf-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="dc4bf-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="dc4bf-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dc4bf-122">Not supported</span></span> | <span data-ttu-id="dc4bf-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dc4bf-123">Not supported</span></span> | <span data-ttu-id="dc4bf-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc4bf-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="dc4bf-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="dc4bf-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="dc4bf-126">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dc4bf-126">Not supported</span></span> | <span data-ttu-id="dc4bf-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dc4bf-127">Not supported</span></span> | <span data-ttu-id="dc4bf-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc4bf-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="dc4bf-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="dc4bf-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="dc4bf-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dc4bf-130">Not supported</span></span> | <span data-ttu-id="dc4bf-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dc4bf-131">Not supported</span></span> | <span data-ttu-id="dc4bf-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc4bf-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="dc4bf-133">contact</span><span class="sxs-lookup"><span data-stu-id="dc4bf-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="dc4bf-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="dc4bf-134">Contacts.Read</span></span> | <span data-ttu-id="dc4bf-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="dc4bf-135">Contacts.Read</span></span> | <span data-ttu-id="dc4bf-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="dc4bf-136">Contacts.Read</span></span> |
|<span data-ttu-id="dc4bf-137">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="dc4bf-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="dc4bf-138">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dc4bf-138">Not supported</span></span> | <span data-ttu-id="dc4bf-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc4bf-139">Files.ReadWrite</span></span> | <span data-ttu-id="dc4bf-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dc4bf-140">Not supported</span></span> |
|<span data-ttu-id="dc4bf-141">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="dc4bf-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="dc4bf-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc4bf-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="dc4bf-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dc4bf-143">Not supported</span></span> | <span data-ttu-id="dc4bf-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc4bf-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="dc4bf-145">event</span><span class="sxs-lookup"><span data-stu-id="dc4bf-145">event</span></span>](../resources/event.md) | <span data-ttu-id="dc4bf-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="dc4bf-146">Calendars.Read</span></span> | <span data-ttu-id="dc4bf-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="dc4bf-147">Calendars.Read</span></span> | <span data-ttu-id="dc4bf-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="dc4bf-148">Calendars.Read</span></span> |
|[<span data-ttu-id="dc4bf-149">group</span><span class="sxs-lookup"><span data-stu-id="dc4bf-149">group</span></span>](../resources/group.md) | <span data-ttu-id="dc4bf-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc4bf-150">Group.Read.All</span></span> | <span data-ttu-id="dc4bf-151">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dc4bf-151">Not supported</span></span> | <span data-ttu-id="dc4bf-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc4bf-152">Group.Read.All</span></span> |
|[<span data-ttu-id="dc4bf-153">group conversation</span><span class="sxs-lookup"><span data-stu-id="dc4bf-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="dc4bf-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc4bf-154">Group.Read.All</span></span> | <span data-ttu-id="dc4bf-155">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dc4bf-155">Not supported</span></span> | <span data-ttu-id="dc4bf-156">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dc4bf-156">Not supported</span></span> |
|[<span data-ttu-id="dc4bf-157">list</span><span class="sxs-lookup"><span data-stu-id="dc4bf-157">list</span></span>](../resources/list.md) | <span data-ttu-id="dc4bf-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc4bf-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="dc4bf-159">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dc4bf-159">Not supported</span></span> | <span data-ttu-id="dc4bf-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc4bf-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="dc4bf-161">message</span><span class="sxs-lookup"><span data-stu-id="dc4bf-161">message</span></span>](../resources/message.md) | <span data-ttu-id="dc4bf-162">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="dc4bf-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="dc4bf-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="dc4bf-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="dc4bf-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="dc4bf-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="dc4bf-165">security alert</span><span class="sxs-lookup"><span data-stu-id="dc4bf-165">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="dc4bf-166">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc4bf-166">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="dc4bf-167">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="dc4bf-167">Not supported</span></span> | <span data-ttu-id="dc4bf-168">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc4bf-168">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="dc4bf-169">user</span><span class="sxs-lookup"><span data-stu-id="dc4bf-169">user</span></span>](../resources/user.md) | <span data-ttu-id="dc4bf-170">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc4bf-170">User.Read.All</span></span> | <span data-ttu-id="dc4bf-171">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc4bf-171">User.Read.All</span></span> | <span data-ttu-id="dc4bf-172">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="dc4bf-172">User.Read.All</span></span> |

### <a name="chatmessage"></a><span data-ttu-id="dc4bf-173">chatMessage</span><span class="sxs-lookup"><span data-stu-id="dc4bf-173">chatMessage</span></span>

<span data-ttu-id="dc4bf-174">Подписки **chatMessage** с разрешениями для приложений включают данные ресурса и требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="dc4bf-174">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="dc4bf-175">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="dc4bf-175">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="dc4bf-176">Перед созданием подписки **chatMessage** вы должны запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="dc4bf-176">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="dc4bf-177">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="dc4bf-177">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="dc4bf-178">**Примечание.** `/teams/getAllMessages` и `/chats/getAllMessages` доступны для пользователей с  
[требуемыми лицензиями](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="dc4bf-178">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the 
[required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

### <a name="driveitem"></a><span data-ttu-id="dc4bf-179">driveItem</span><span class="sxs-lookup"><span data-stu-id="dc4bf-179">driveItem</span></span>

<span data-ttu-id="dc4bf-180">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="dc4bf-180">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="dc4bf-181">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="dc4bf-181">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="dc4bf-182">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="dc4bf-182">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="dc4bf-183">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="dc4bf-183">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="dc4bf-184">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="dc4bf-184">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="dc4bf-185">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="dc4bf-185">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="dc4bf-186">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="dc4bf-186">contact, event, and message</span></span>

<span data-ttu-id="dc4bf-187">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="dc4bf-187">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="dc4bf-188">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="dc4bf-188">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="dc4bf-189">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="dc4bf-189">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="dc4bf-190">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="dc4bf-190">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="dc4bf-191">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="dc4bf-191">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="dc4bf-192">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="dc4bf-192">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="dc4bf-193">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="dc4bf-193">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="dc4bf-194">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc4bf-194">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{subscription-id}
```

## <a name="request-headers"></a><span data-ttu-id="dc4bf-195">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dc4bf-195">Request headers</span></span>

| <span data-ttu-id="dc4bf-196">Имя</span><span class="sxs-lookup"><span data-stu-id="dc4bf-196">Name</span></span>       | <span data-ttu-id="dc4bf-197">Тип</span><span class="sxs-lookup"><span data-stu-id="dc4bf-197">Type</span></span> | <span data-ttu-id="dc4bf-198">Описание</span><span class="sxs-lookup"><span data-stu-id="dc4bf-198">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="dc4bf-199">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc4bf-199">Authorization</span></span>  | <span data-ttu-id="dc4bf-200">string</span><span class="sxs-lookup"><span data-stu-id="dc4bf-200">string</span></span>  | <span data-ttu-id="dc4bf-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dc4bf-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dc4bf-203">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dc4bf-203">Request body</span></span>

<span data-ttu-id="dc4bf-204">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dc4bf-204">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc4bf-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc4bf-205">Response</span></span>

<span data-ttu-id="dc4bf-206">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dc4bf-206">If successful, this method returns a `204 No Content` response code.</span></span>
<span data-ttu-id="dc4bf-207">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="dc4bf-207">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="dc4bf-208">Пример</span><span class="sxs-lookup"><span data-stu-id="dc4bf-208">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dc4bf-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc4bf-209">Request</span></span>

<span data-ttu-id="dc4bf-210">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc4bf-210">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dc4bf-211">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc4bf-211">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07
```
# <a name="c"></a>[<span data-ttu-id="dc4bf-212">C#</span><span class="sxs-lookup"><span data-stu-id="dc4bf-212">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dc4bf-213">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc4bf-213">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dc4bf-214">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc4bf-214">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dc4bf-215">Java</span><span class="sxs-lookup"><span data-stu-id="dc4bf-215">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dc4bf-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc4bf-216">Response</span></span>

<span data-ttu-id="dc4bf-217">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dc4bf-217">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 204 No Content
```

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

