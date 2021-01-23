---
title: Удаление подписки
description: Удаление подписки.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c054270a26924ace94225e35b6a69cf80730f46c
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934900"
---
# <a name="delete-subscription"></a><span data-ttu-id="308ec-103">Удаление подписки</span><span class="sxs-lookup"><span data-stu-id="308ec-103">Delete subscription</span></span>

<span data-ttu-id="308ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="308ec-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="308ec-105">Удаление подписки.</span><span class="sxs-lookup"><span data-stu-id="308ec-105">Delete a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="308ec-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="308ec-106">Permissions</span></span>

<span data-ttu-id="308ec-107">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="308ec-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="308ec-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="308ec-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="308ec-109">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="308ec-109">Supported resource</span></span> | <span data-ttu-id="308ec-110">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="308ec-110">Delegated (work or school account)</span></span> | <span data-ttu-id="308ec-111">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="308ec-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="308ec-112">Приложение</span><span class="sxs-lookup"><span data-stu-id="308ec-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="308ec-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="308ec-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="308ec-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="308ec-114">Not supported</span></span> | <span data-ttu-id="308ec-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="308ec-115">Not supported</span></span> | <span data-ttu-id="308ec-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="308ec-116">CallRecords.Read.All</span></span> |
|<span data-ttu-id="308ec-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="308ec-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="308ec-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="308ec-118">Not supported</span></span> | <span data-ttu-id="308ec-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="308ec-119">Not supported</span></span> |  <span data-ttu-id="308ec-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="308ec-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="308ec-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="308ec-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="308ec-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="308ec-122">Not supported</span></span> | <span data-ttu-id="308ec-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="308ec-123">Not supported</span></span> | <span data-ttu-id="308ec-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="308ec-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="308ec-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="308ec-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="308ec-126">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="308ec-126">Not supported</span></span> | <span data-ttu-id="308ec-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="308ec-127">Not supported</span></span> | <span data-ttu-id="308ec-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="308ec-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="308ec-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="308ec-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="308ec-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="308ec-130">Not supported</span></span> | <span data-ttu-id="308ec-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="308ec-131">Not supported</span></span> | <span data-ttu-id="308ec-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="308ec-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="308ec-133">contact</span><span class="sxs-lookup"><span data-stu-id="308ec-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="308ec-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="308ec-134">Contacts.Read</span></span> | <span data-ttu-id="308ec-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="308ec-135">Contacts.Read</span></span> | <span data-ttu-id="308ec-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="308ec-136">Contacts.Read</span></span> |
|<span data-ttu-id="308ec-137">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="308ec-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="308ec-138">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="308ec-138">Not supported</span></span> | <span data-ttu-id="308ec-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="308ec-139">Files.ReadWrite</span></span> | <span data-ttu-id="308ec-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="308ec-140">Not supported</span></span> |
|<span data-ttu-id="308ec-141">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="308ec-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="308ec-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="308ec-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="308ec-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="308ec-143">Not supported</span></span> | <span data-ttu-id="308ec-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="308ec-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="308ec-145">event</span><span class="sxs-lookup"><span data-stu-id="308ec-145">event</span></span>](../resources/event.md) | <span data-ttu-id="308ec-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="308ec-146">Calendars.Read</span></span> | <span data-ttu-id="308ec-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="308ec-147">Calendars.Read</span></span> | <span data-ttu-id="308ec-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="308ec-148">Calendars.Read</span></span> |
|[<span data-ttu-id="308ec-149">group</span><span class="sxs-lookup"><span data-stu-id="308ec-149">group</span></span>](../resources/group.md) | <span data-ttu-id="308ec-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="308ec-150">Group.Read.All</span></span> | <span data-ttu-id="308ec-151">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="308ec-151">Not supported</span></span> | <span data-ttu-id="308ec-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="308ec-152">Group.Read.All</span></span> |
|[<span data-ttu-id="308ec-153">group conversation</span><span class="sxs-lookup"><span data-stu-id="308ec-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="308ec-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="308ec-154">Group.Read.All</span></span> | <span data-ttu-id="308ec-155">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="308ec-155">Not supported</span></span> | <span data-ttu-id="308ec-156">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="308ec-156">Not supported</span></span> |
|[<span data-ttu-id="308ec-157">list</span><span class="sxs-lookup"><span data-stu-id="308ec-157">list</span></span>](../resources/list.md) | <span data-ttu-id="308ec-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="308ec-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="308ec-159">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="308ec-159">Not supported</span></span> | <span data-ttu-id="308ec-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="308ec-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="308ec-161">message</span><span class="sxs-lookup"><span data-stu-id="308ec-161">message</span></span>](../resources/message.md) | <span data-ttu-id="308ec-162">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="308ec-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="308ec-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="308ec-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="308ec-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="308ec-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="308ec-165">security alert</span><span class="sxs-lookup"><span data-stu-id="308ec-165">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="308ec-166">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="308ec-166">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="308ec-167">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="308ec-167">Not supported</span></span> | <span data-ttu-id="308ec-168">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="308ec-168">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="308ec-169">user</span><span class="sxs-lookup"><span data-stu-id="308ec-169">user</span></span>](../resources/user.md) | <span data-ttu-id="308ec-170">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="308ec-170">User.Read.All</span></span> | <span data-ttu-id="308ec-171">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="308ec-171">User.Read.All</span></span> | <span data-ttu-id="308ec-172">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="308ec-172">User.Read.All</span></span> |

> <span data-ttu-id="308ec-173">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="308ec-173">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="chatmessage"></a><span data-ttu-id="308ec-174">chatMessage</span><span class="sxs-lookup"><span data-stu-id="308ec-174">chatMessage</span></span>

<span data-ttu-id="308ec-175">Подписки **chatMessage** с разрешениями для приложений включают данные ресурса и требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="308ec-175">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="308ec-176">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="308ec-176">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="308ec-177">Перед созданием подписки **chatMessage** вы должны запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="308ec-177">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="308ec-178">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="308ec-178">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="308ec-179">**Примечание.** `/teams/getAllMessages` и `/chats/getAllMessages` доступны для пользователей с [требуемыми лицензиями](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="308ec-179">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>
<span data-ttu-id="308ec-180">В будущем корпорация Майкрософт может потребовать от вас или ваших клиентов оплаты дополнительных платежей в зависимости от объема данных, доступных через API.</span><span class="sxs-lookup"><span data-stu-id="308ec-180">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data accessed through the API.</span></span>

### <a name="driveitem"></a><span data-ttu-id="308ec-181">driveItem</span><span class="sxs-lookup"><span data-stu-id="308ec-181">driveItem</span></span>

<span data-ttu-id="308ec-182">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="308ec-182">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="308ec-183">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="308ec-183">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="308ec-184">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="308ec-184">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="308ec-185">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="308ec-185">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="308ec-186">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="308ec-186">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="308ec-187">Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="308ec-187">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="308ec-188">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="308ec-188">contact, event, and message</span></span>

<span data-ttu-id="308ec-189">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="308ec-189">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="308ec-190">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="308ec-190">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="308ec-191">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="308ec-191">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="308ec-192">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="308ec-192">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="308ec-193">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="308ec-193">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="308ec-194">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="308ec-194">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="308ec-195">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="308ec-195">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>


## <a name="http-request"></a><span data-ttu-id="308ec-196">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="308ec-196">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /subscriptions/{subscription-id}
```

## <a name="request-headers"></a><span data-ttu-id="308ec-197">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="308ec-197">Request headers</span></span>

| <span data-ttu-id="308ec-198">Имя</span><span class="sxs-lookup"><span data-stu-id="308ec-198">Name</span></span>       | <span data-ttu-id="308ec-199">Тип</span><span class="sxs-lookup"><span data-stu-id="308ec-199">Type</span></span> | <span data-ttu-id="308ec-200">Описание</span><span class="sxs-lookup"><span data-stu-id="308ec-200">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="308ec-201">Authorization</span><span class="sxs-lookup"><span data-stu-id="308ec-201">Authorization</span></span>  | <span data-ttu-id="308ec-202">string</span><span class="sxs-lookup"><span data-stu-id="308ec-202">string</span></span>  | <span data-ttu-id="308ec-p108">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="308ec-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="308ec-205">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="308ec-205">Request body</span></span>

<span data-ttu-id="308ec-206">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="308ec-206">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="308ec-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="308ec-207">Response</span></span>

<span data-ttu-id="308ec-208">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="308ec-208">If successful, this method returns a `204 No Content` response code.</span></span>
<span data-ttu-id="308ec-209">Подробнее о том, как возвращаются ошибки, см. в статье [Возвращение ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="308ec-209">For details about how errors are returned, see [Error responses][error-response].</span></span>

## <a name="example"></a><span data-ttu-id="308ec-210">Пример</span><span class="sxs-lookup"><span data-stu-id="308ec-210">Example</span></span>

##### <a name="request"></a><span data-ttu-id="308ec-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="308ec-211">Request</span></span>

<span data-ttu-id="308ec-212">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="308ec-212">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="308ec-213">HTTP</span><span class="sxs-lookup"><span data-stu-id="308ec-213">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/7f105c7d-2dc5-4530-97cd-4e7ae6534c07
```
# <a name="c"></a>[<span data-ttu-id="308ec-214">C#</span><span class="sxs-lookup"><span data-stu-id="308ec-214">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="308ec-215">JavaScript</span><span class="sxs-lookup"><span data-stu-id="308ec-215">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="308ec-216">Objective-C</span><span class="sxs-lookup"><span data-stu-id="308ec-216">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="308ec-217">Java</span><span class="sxs-lookup"><span data-stu-id="308ec-217">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="308ec-218">Отклик</span><span class="sxs-lookup"><span data-stu-id="308ec-218">Response</span></span>

<span data-ttu-id="308ec-219">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="308ec-219">Here is an example of the response.</span></span>
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

