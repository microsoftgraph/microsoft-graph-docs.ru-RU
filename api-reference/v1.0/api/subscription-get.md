---
title: Получение подписки
description: Получение свойств и связей подписки.
localization_priority: Priority
author: davidmu1
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 52a0676db0e14a985b518799766f13a9f007c58a
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848193"
---
# <a name="get-subscription"></a><span data-ttu-id="89193-103">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="89193-103">Get subscription</span></span>

<span data-ttu-id="89193-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89193-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="89193-105">Получение свойств и связей подписки.</span><span class="sxs-lookup"><span data-stu-id="89193-105">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="89193-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="89193-106">Permissions</span></span>

<span data-ttu-id="89193-107">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="89193-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="89193-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89193-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="89193-109">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="89193-109">Supported resource</span></span> | <span data-ttu-id="89193-110">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89193-110">Delegated (work or school account)</span></span> | <span data-ttu-id="89193-111">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89193-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89193-112">Приложение</span><span class="sxs-lookup"><span data-stu-id="89193-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="89193-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="89193-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="89193-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="89193-114">Not supported</span></span> | <span data-ttu-id="89193-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="89193-115">Not supported</span></span> | <span data-ttu-id="89193-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="89193-116">CallRecords.Read.All</span></span> |
|<span data-ttu-id="89193-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="89193-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="89193-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="89193-118">Not supported</span></span> | <span data-ttu-id="89193-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="89193-119">Not supported</span></span> |  <span data-ttu-id="89193-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="89193-120">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="89193-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="89193-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="89193-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="89193-122">Not supported</span></span> | <span data-ttu-id="89193-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="89193-123">Not supported</span></span> | <span data-ttu-id="89193-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="89193-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="89193-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="89193-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="89193-126">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="89193-126">Not supported</span></span> | <span data-ttu-id="89193-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="89193-127">Not supported</span></span> | <span data-ttu-id="89193-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="89193-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="89193-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="89193-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="89193-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="89193-130">Not supported</span></span> | <span data-ttu-id="89193-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="89193-131">Not supported</span></span> | <span data-ttu-id="89193-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="89193-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="89193-133">contact</span><span class="sxs-lookup"><span data-stu-id="89193-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="89193-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="89193-134">Contacts.Read</span></span> | <span data-ttu-id="89193-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="89193-135">Contacts.Read</span></span> | <span data-ttu-id="89193-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="89193-136">Contacts.Read</span></span> |
|<span data-ttu-id="89193-137">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="89193-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="89193-138">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="89193-138">Not supported</span></span> | <span data-ttu-id="89193-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89193-139">Files.ReadWrite</span></span> | <span data-ttu-id="89193-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="89193-140">Not supported</span></span> |
|<span data-ttu-id="89193-141">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="89193-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="89193-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89193-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="89193-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="89193-143">Not supported</span></span> | <span data-ttu-id="89193-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89193-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="89193-145">event</span><span class="sxs-lookup"><span data-stu-id="89193-145">event</span></span>](../resources/event.md) | <span data-ttu-id="89193-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="89193-146">Calendars.Read</span></span> | <span data-ttu-id="89193-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="89193-147">Calendars.Read</span></span> | <span data-ttu-id="89193-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="89193-148">Calendars.Read</span></span> |
|[<span data-ttu-id="89193-149">group</span><span class="sxs-lookup"><span data-stu-id="89193-149">group</span></span>](../resources/group.md) | <span data-ttu-id="89193-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="89193-150">Group.Read.All</span></span> | <span data-ttu-id="89193-151">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="89193-151">Not supported</span></span> | <span data-ttu-id="89193-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="89193-152">Group.Read.All</span></span> |
|[<span data-ttu-id="89193-153">group conversation</span><span class="sxs-lookup"><span data-stu-id="89193-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="89193-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="89193-154">Group.Read.All</span></span> | <span data-ttu-id="89193-155">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="89193-155">Not supported</span></span> | <span data-ttu-id="89193-156">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="89193-156">Not supported</span></span> |
|[<span data-ttu-id="89193-157">list</span><span class="sxs-lookup"><span data-stu-id="89193-157">list</span></span>](../resources/list.md) | <span data-ttu-id="89193-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89193-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="89193-159">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="89193-159">Not supported</span></span> | <span data-ttu-id="89193-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89193-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="89193-161">message</span><span class="sxs-lookup"><span data-stu-id="89193-161">message</span></span>](../resources/message.md) | <span data-ttu-id="89193-162">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="89193-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="89193-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="89193-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="89193-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="89193-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="89193-165">security alert</span><span class="sxs-lookup"><span data-stu-id="89193-165">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="89193-166">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89193-166">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="89193-167">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="89193-167">Not supported</span></span> | <span data-ttu-id="89193-168">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89193-168">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="89193-169">user</span><span class="sxs-lookup"><span data-stu-id="89193-169">user</span></span>](../resources/user.md) | <span data-ttu-id="89193-170">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="89193-170">User.Read.All</span></span> | <span data-ttu-id="89193-171">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="89193-171">User.Read.All</span></span> | <span data-ttu-id="89193-172">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="89193-172">User.Read.All</span></span> |

> <span data-ttu-id="89193-173">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="89193-173">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

### <a name="chatmessage"></a><span data-ttu-id="89193-174">chatMessage</span><span class="sxs-lookup"><span data-stu-id="89193-174">chatMessage</span></span>

<span data-ttu-id="89193-175">Подписки **chatMessage** с разрешениями для приложений включают данные ресурса и требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="89193-175">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="89193-176">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="89193-176">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="89193-177">Перед созданием подписки **chatMessage** вы должны запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="89193-177">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="89193-178">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="89193-178">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="89193-179">**Примечание.** `/teams/getAllMessages` и `/chats/getAllMessages` доступны для пользователей с [требуемыми лицензиями](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="89193-179">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

### <a name="driveitem"></a><span data-ttu-id="89193-180">driveItem</span><span class="sxs-lookup"><span data-stu-id="89193-180">driveItem</span></span>

<span data-ttu-id="89193-181">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="89193-181">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="89193-182">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="89193-182">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="89193-183">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="89193-183">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="89193-184">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="89193-184">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="89193-185">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="89193-185">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="89193-186">Нельзя подписаться на экземпляры **drive** или **driveItem** , не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="89193-186">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="89193-187">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="89193-187">contact, event, and message</span></span>

<span data-ttu-id="89193-188">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="89193-188">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="89193-189">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="89193-189">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="89193-190">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="89193-190">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="89193-191">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="89193-191">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="89193-192">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="89193-192">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="89193-193">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="89193-193">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="89193-194">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="89193-194">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>
 

## <a name="http-request"></a><span data-ttu-id="89193-195">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89193-195">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="89193-196">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="89193-196">Optional query parameters</span></span>

<span data-ttu-id="89193-197">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="89193-197">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="89193-198">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="89193-198">Request headers</span></span>

| <span data-ttu-id="89193-199">Имя</span><span class="sxs-lookup"><span data-stu-id="89193-199">Name</span></span>       | <span data-ttu-id="89193-200">Тип</span><span class="sxs-lookup"><span data-stu-id="89193-200">Type</span></span> | <span data-ttu-id="89193-201">Описание</span><span class="sxs-lookup"><span data-stu-id="89193-201">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="89193-202">Authorization</span><span class="sxs-lookup"><span data-stu-id="89193-202">Authorization</span></span>  | <span data-ttu-id="89193-203">string</span><span class="sxs-lookup"><span data-stu-id="89193-203">string</span></span>  | <span data-ttu-id="89193-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89193-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="89193-206">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="89193-206">Request body</span></span>

<span data-ttu-id="89193-207">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="89193-207">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89193-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="89193-208">Response</span></span>

<span data-ttu-id="89193-209">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="89193-209">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89193-210">Пример</span><span class="sxs-lookup"><span data-stu-id="89193-210">Example</span></span>

##### <a name="request"></a><span data-ttu-id="89193-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="89193-211">Request</span></span>

<span data-ttu-id="89193-212">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89193-212">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="89193-213">HTTP</span><span class="sxs-lookup"><span data-stu-id="89193-213">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="89193-214">C#</span><span class="sxs-lookup"><span data-stu-id="89193-214">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="89193-215">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89193-215">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="89193-216">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89193-216">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="89193-217">Java</span><span class="sxs-lookup"><span data-stu-id="89193-217">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="89193-218">Отклик</span><span class="sxs-lookup"><span data-stu-id="89193-218">Response</span></span>

<span data-ttu-id="89193-219">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="89193-219">Here is an example of the response.</span></span>
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
  "includeResourceData": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

