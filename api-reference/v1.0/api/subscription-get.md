---
title: Получение подписки
description: Получение свойств и связей подписки.
localization_priority: Priority
author: davidmu1
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 422526f04ea9b1b2345c8db5c0d1c2ee74861b6e
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2020
ms.locfileid: "48742211"
---
# <a name="get-subscription"></a><span data-ttu-id="689cb-103">Получение подписки</span><span class="sxs-lookup"><span data-stu-id="689cb-103">Get subscription</span></span>

<span data-ttu-id="689cb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="689cb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="689cb-105">Получение свойств и связей подписки.</span><span class="sxs-lookup"><span data-stu-id="689cb-105">Retrieve the properties and relationships of a subscription.</span></span>

## <a name="permissions"></a><span data-ttu-id="689cb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="689cb-106">Permissions</span></span>

<span data-ttu-id="689cb-107">В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="689cb-107">Depending on the resource and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="689cb-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="689cb-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="689cb-109">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="689cb-109">Supported resource</span></span> | <span data-ttu-id="689cb-110">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="689cb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="689cb-111">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="689cb-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="689cb-112">Приложение</span><span class="sxs-lookup"><span data-stu-id="689cb-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
|[<span data-ttu-id="689cb-113">callRecord</span><span class="sxs-lookup"><span data-stu-id="689cb-113">callRecord</span></span>](../resources/callrecords-callrecord.md) | <span data-ttu-id="689cb-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="689cb-114">Not supported</span></span> | <span data-ttu-id="689cb-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="689cb-115">Not supported</span></span> | <span data-ttu-id="689cb-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="689cb-116">CallRecords.Read.All</span></span> |
|<span data-ttu-id="689cb-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="689cb-117">[chatMessage](../resources/chatmessage.md) (/teams/{id}/channels/{id}/messages)</span></span> | <span data-ttu-id="689cb-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="689cb-118">Not supported</span></span> | <span data-ttu-id="689cb-119">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="689cb-119">Not supported</span></span> | <span data-ttu-id="689cb-120">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="689cb-120">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="689cb-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages — все сообщения канала в организации)</span><span class="sxs-lookup"><span data-stu-id="689cb-121">[chatMessage](../resources/chatmessage.md) (/teams/getAllMessages -- all channel messages in organization)</span></span> | <span data-ttu-id="689cb-122">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="689cb-122">Not supported</span></span> | <span data-ttu-id="689cb-123">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="689cb-123">Not supported</span></span> | <span data-ttu-id="689cb-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="689cb-124">ChannelMessage.Read.All</span></span>  |
|<span data-ttu-id="689cb-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span><span class="sxs-lookup"><span data-stu-id="689cb-125">[chatMessage](../resources/chatmessage.md) (/chats/{id}/messages)</span></span> | <span data-ttu-id="689cb-126">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="689cb-126">Not supported</span></span> | <span data-ttu-id="689cb-127">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="689cb-127">Not supported</span></span> | <span data-ttu-id="689cb-128">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="689cb-128">Chat.Read.All</span></span>  |
|<span data-ttu-id="689cb-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages — все сообщения чата в организации)</span><span class="sxs-lookup"><span data-stu-id="689cb-129">[chatMessage](../resources/chatmessage.md) (/chats/getAllMessages -- all chat messages in organization)</span></span> | <span data-ttu-id="689cb-130">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="689cb-130">Not supported</span></span> | <span data-ttu-id="689cb-131">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="689cb-131">Not supported</span></span> | <span data-ttu-id="689cb-132">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="689cb-132">Chat.Read.All</span></span>  |
|[<span data-ttu-id="689cb-133">contact</span><span class="sxs-lookup"><span data-stu-id="689cb-133">contact</span></span>](../resources/contact.md) | <span data-ttu-id="689cb-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="689cb-134">Contacts.Read</span></span> | <span data-ttu-id="689cb-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="689cb-135">Contacts.Read</span></span> | <span data-ttu-id="689cb-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="689cb-136">Contacts.Read</span></span> |
|<span data-ttu-id="689cb-137">[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя)</span><span class="sxs-lookup"><span data-stu-id="689cb-137">[driveItem](../resources/driveitem.md) (user's personal OneDrive)</span></span> | <span data-ttu-id="689cb-138">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="689cb-138">Not supported</span></span> | <span data-ttu-id="689cb-139">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="689cb-139">Files.ReadWrite</span></span> | <span data-ttu-id="689cb-140">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="689cb-140">Not supported</span></span> |
|<span data-ttu-id="689cb-141">[driveItem](../resources/driveitem.md) (OneDrive для бизнеса)</span><span class="sxs-lookup"><span data-stu-id="689cb-141">[driveItem](../resources/driveitem.md) (OneDrive for Business)</span></span> | <span data-ttu-id="689cb-142">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="689cb-142">Files.ReadWrite.All</span></span> | <span data-ttu-id="689cb-143">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="689cb-143">Not supported</span></span> | <span data-ttu-id="689cb-144">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="689cb-144">Files.ReadWrite.All</span></span> |
|[<span data-ttu-id="689cb-145">event</span><span class="sxs-lookup"><span data-stu-id="689cb-145">event</span></span>](../resources/event.md) | <span data-ttu-id="689cb-146">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="689cb-146">Calendars.Read</span></span> | <span data-ttu-id="689cb-147">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="689cb-147">Calendars.Read</span></span> | <span data-ttu-id="689cb-148">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="689cb-148">Calendars.Read</span></span> |
|[<span data-ttu-id="689cb-149">group</span><span class="sxs-lookup"><span data-stu-id="689cb-149">group</span></span>](../resources/group.md) | <span data-ttu-id="689cb-150">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="689cb-150">Group.Read.All</span></span> | <span data-ttu-id="689cb-151">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="689cb-151">Not supported</span></span> | <span data-ttu-id="689cb-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="689cb-152">Group.Read.All</span></span> |
|[<span data-ttu-id="689cb-153">group conversation</span><span class="sxs-lookup"><span data-stu-id="689cb-153">group conversation</span></span>](../resources/conversation.md) | <span data-ttu-id="689cb-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="689cb-154">Group.Read.All</span></span> | <span data-ttu-id="689cb-155">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="689cb-155">Not supported</span></span> | <span data-ttu-id="689cb-156">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="689cb-156">Not supported</span></span> |
|[<span data-ttu-id="689cb-157">list</span><span class="sxs-lookup"><span data-stu-id="689cb-157">list</span></span>](../resources/list.md) | <span data-ttu-id="689cb-158">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="689cb-158">Sites.ReadWrite.All</span></span> | <span data-ttu-id="689cb-159">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="689cb-159">Not supported</span></span> | <span data-ttu-id="689cb-160">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="689cb-160">Sites.ReadWrite.All</span></span> |
|[<span data-ttu-id="689cb-161">message</span><span class="sxs-lookup"><span data-stu-id="689cb-161">message</span></span>](../resources/message.md) | <span data-ttu-id="689cb-162">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="689cb-162">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="689cb-163">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="689cb-163">Mail.ReadBasic, Mail.Read</span></span> | <span data-ttu-id="689cb-164">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="689cb-164">Mail.ReadBasic, Mail.Read</span></span> |
|[<span data-ttu-id="689cb-165">security alert</span><span class="sxs-lookup"><span data-stu-id="689cb-165">security alert</span></span>](../resources/alert.md) | <span data-ttu-id="689cb-166">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="689cb-166">SecurityEvents.ReadWrite.All</span></span> | <span data-ttu-id="689cb-167">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="689cb-167">Not supported</span></span> | <span data-ttu-id="689cb-168">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="689cb-168">SecurityEvents.ReadWrite.All</span></span> |
|[<span data-ttu-id="689cb-169">user</span><span class="sxs-lookup"><span data-stu-id="689cb-169">user</span></span>](../resources/user.md) | <span data-ttu-id="689cb-170">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="689cb-170">User.Read.All</span></span> | <span data-ttu-id="689cb-171">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="689cb-171">User.Read.All</span></span> | <span data-ttu-id="689cb-172">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="689cb-172">User.Read.All</span></span> |

### <a name="chatmessage"></a><span data-ttu-id="689cb-173">chatMessage</span><span class="sxs-lookup"><span data-stu-id="689cb-173">chatMessage</span></span>

<span data-ttu-id="689cb-174">Подписки **chatMessage** с разрешениями для приложений включают данные ресурса и требуют [шифрования](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="689cb-174">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="689cb-175">Создание подписки завершится сбоем, если не указан [encryptionCertificate](../resources/subscription.md).</span><span class="sxs-lookup"><span data-stu-id="689cb-175">Subscription creation will fail if [encryptionCertificate](../resources/subscription.md) is not specified.</span></span> <span data-ttu-id="689cb-176">Перед созданием подписки **chatMessage** вы должны запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="689cb-176">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="689cb-177">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="689cb-177">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="689cb-178">**Примечание.** `/teams/getAllMessages` и `/chats/getAllMessages` доступны для пользователей с [требуемыми лицензиями](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="689cb-178">**Note:** `/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>

### <a name="driveitem"></a><span data-ttu-id="689cb-179">driveItem</span><span class="sxs-lookup"><span data-stu-id="689cb-179">driveItem</span></span>

<span data-ttu-id="689cb-180">Дополнительные ограничения применяются к подпискам на элементы OneDrive.</span><span class="sxs-lookup"><span data-stu-id="689cb-180">Additional limitations apply for subscriptions on OneDrive items.</span></span> <span data-ttu-id="689cb-181">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="689cb-181">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

<span data-ttu-id="689cb-182">В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище.</span><span class="sxs-lookup"><span data-stu-id="689cb-182">On a personal OneDrive, you can subscribe to the root folder or any subfolder in that drive.</span></span> <span data-ttu-id="689cb-183">В OneDrive для бизнеса можно подписаться только на корневую папку.</span><span class="sxs-lookup"><span data-stu-id="689cb-183">On OneDrive for Business, you can subscribe to only the root folder.</span></span> <span data-ttu-id="689cb-184">Уведомления об изменениях отправляются для определенных типов изменений папки, на которую оформлена подписка, любого файла, папки или других экземпляров **driveItem** в ее иерархии.</span><span class="sxs-lookup"><span data-stu-id="689cb-184">Change notifications are sent for the requested types of changes on the subscribed folder, or any file, folder, or other **driveItem** instances in its hierarchy.</span></span> <span data-ttu-id="689cb-185">Нельзя подписаться на экземпляры **drive** или **driveItem** , не являющиеся папками, например на отдельные файлы.</span><span class="sxs-lookup"><span data-stu-id="689cb-185">You cannot subscribe to **drive** or **driveItem** instances that are not folders, such as individual files.</span></span>

### <a name="contact-event-and-message"></a><span data-ttu-id="689cb-186">contact, event и message</span><span class="sxs-lookup"><span data-stu-id="689cb-186">contact, event, and message</span></span>

<span data-ttu-id="689cb-187">Дополнительные ограничения применяются к подпискам на элементы Outlook.</span><span class="sxs-lookup"><span data-stu-id="689cb-187">Additional limitations apply for subscriptions on Outlook items.</span></span> <span data-ttu-id="689cb-188">Ограничения применяются для создания, а также управления (получение, обновление и удаление) подписками.</span><span class="sxs-lookup"><span data-stu-id="689cb-188">The limitations apply to creating as well as managing (getting, updating, and deleting) subscriptions.</span></span>

- <span data-ttu-id="689cb-189">Делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="689cb-189">Delegated permission supports subscribing to items in folders in only the signed-in user's mailbox.</span></span> <span data-ttu-id="689cb-190">Например, вы не можете использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="689cb-190">For example, you cannot use the delegated permission Calendars.Read to subscribe to events in another user’s mailbox.</span></span>
- <span data-ttu-id="689cb-191">Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:</span><span class="sxs-lookup"><span data-stu-id="689cb-191">To subscribe to change notifications of Outlook contacts, events, or messages in _shared or delegated_ folders:</span></span>

  - <span data-ttu-id="689cb-192">Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="689cb-192">Use the corresponding application permission to subscribe to changes of items in a folder or mailbox of _any_ user in the tenant.</span></span>
  - <span data-ttu-id="689cb-193">Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.</span><span class="sxs-lookup"><span data-stu-id="689cb-193">Do not use the Outlook sharing permissions (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared, and their read/write counterparts), as they do **not** support subscribing to change notifications on items in shared or delegated folders.</span></span>
 

## <a name="http-request"></a><span data-ttu-id="689cb-194">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="689cb-194">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="689cb-195">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="689cb-195">Optional query parameters</span></span>

<span data-ttu-id="689cb-196">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="689cb-196">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="689cb-197">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="689cb-197">Request headers</span></span>

| <span data-ttu-id="689cb-198">Имя</span><span class="sxs-lookup"><span data-stu-id="689cb-198">Name</span></span>       | <span data-ttu-id="689cb-199">Тип</span><span class="sxs-lookup"><span data-stu-id="689cb-199">Type</span></span> | <span data-ttu-id="689cb-200">Описание</span><span class="sxs-lookup"><span data-stu-id="689cb-200">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="689cb-201">Authorization</span><span class="sxs-lookup"><span data-stu-id="689cb-201">Authorization</span></span>  | <span data-ttu-id="689cb-202">string</span><span class="sxs-lookup"><span data-stu-id="689cb-202">string</span></span>  | <span data-ttu-id="689cb-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="689cb-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="689cb-205">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="689cb-205">Request body</span></span>

<span data-ttu-id="689cb-206">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="689cb-206">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="689cb-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="689cb-207">Response</span></span>

<span data-ttu-id="689cb-208">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="689cb-208">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="689cb-209">Пример</span><span class="sxs-lookup"><span data-stu-id="689cb-209">Example</span></span>

##### <a name="request"></a><span data-ttu-id="689cb-210">Запрос</span><span class="sxs-lookup"><span data-stu-id="689cb-210">Request</span></span>

<span data-ttu-id="689cb-211">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="689cb-211">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="689cb-212">HTTP</span><span class="sxs-lookup"><span data-stu-id="689cb-212">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/subscriptions/{id}
```
# <a name="c"></a>[<span data-ttu-id="689cb-213">C#</span><span class="sxs-lookup"><span data-stu-id="689cb-213">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="689cb-214">JavaScript</span><span class="sxs-lookup"><span data-stu-id="689cb-214">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="689cb-215">Objective-C</span><span class="sxs-lookup"><span data-stu-id="689cb-215">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="689cb-216">Java</span><span class="sxs-lookup"><span data-stu-id="689cb-216">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="689cb-217">Отклик</span><span class="sxs-lookup"><span data-stu-id="689cb-217">Response</span></span>

<span data-ttu-id="689cb-218">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="689cb-218">Here is an example of the response.</span></span>
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

