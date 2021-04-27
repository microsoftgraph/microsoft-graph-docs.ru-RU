---
title: Получение вложения
description: Ознакомьтесь с свойствами и отношениями вложения, присоединенных к событию, сообщению, Outlook или сообщению.
localization_priority: Normal
doc_type: apiPageType
author: abheek-das
ms.prod: outlook
ms.openlocfilehash: 39c8be1eb33bd5843fe38c3715a3ee207e57c9f6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048031"
---
# <a name="get-attachment"></a><span data-ttu-id="17382-103">Получение вложения</span><span class="sxs-lookup"><span data-stu-id="17382-103">Get attachment</span></span>

<span data-ttu-id="17382-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17382-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="17382-105">Ознакомьтесь с свойствами, отношениями или необработанные содержимое вложения, присоединенного к событию [пользователя,](../resources/event.md) [сообщению,](../resources/message.md) [Outlook](../resources/outlooktask.md)задаче или групповой [публикации.](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="17382-105">Read the properties, relationships, or raw contents of an attachment that is attached to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or group [post](../resources/post.md).</span></span> 

<span data-ttu-id="17382-106">Допустимые типы вложений:</span><span class="sxs-lookup"><span data-stu-id="17382-106">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="17382-107">Файл.</span><span class="sxs-lookup"><span data-stu-id="17382-107">A file.</span></span> <span data-ttu-id="17382-108">На программном уровне это ресурс [fileAttachment](../resources/fileattachment.md).</span><span class="sxs-lookup"><span data-stu-id="17382-108">Programmatically, this is a [fileAttachment](../resources/fileattachment.md) resource.</span></span> <span data-ttu-id="17382-109">См. [пример 1](#example-1-get-the-properties-of-a-file-attachment).</span><span class="sxs-lookup"><span data-stu-id="17382-109">See [example 1](#example-1-get-the-properties-of-a-file-attachment).</span></span>
* <span data-ttu-id="17382-110">Элемент Outlook (контакт, событие или сообщение).</span><span class="sxs-lookup"><span data-stu-id="17382-110">An Outlook item (contact, event or message).</span></span> <span data-ttu-id="17382-111">На программном уровне вложением элемента является ресурс [itemAttachment](../resources/itemattachment.md).</span><span class="sxs-lookup"><span data-stu-id="17382-111">Programmatically, an item attachment is an [itemAttachment](../resources/itemattachment.md) resource.</span></span> <span data-ttu-id="17382-112">Вы можете использовать параметр `$expand`, чтобы получить дополнительные свойства этого элемента, включая любые вложения (до 30 уровней).</span><span class="sxs-lookup"><span data-stu-id="17382-112">You can use `$expand` to further get the properties of that item, including any nested attachments up to 30 levels.</span></span> <span data-ttu-id="17382-113">См. [пример 3](#example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message) и [пример 4](#example-4-expand-and-get-the-properties-of-an-item-attached-to-a-message-including-any-attachment-to-the-item).</span><span class="sxs-lookup"><span data-stu-id="17382-113">See [example 3](#example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message) and [example 4](#example-4-expand-and-get-the-properties-of-an-item-attached-to-a-message-including-any-attachment-to-the-item).</span></span>
* <span data-ttu-id="17382-114">Ссылка на файл, хранящийся в облаке.</span><span class="sxs-lookup"><span data-stu-id="17382-114">A link to a file stored in the cloud.</span></span> <span data-ttu-id="17382-115">На программном уровне это ресурс [referenceAttachment](../resources/referenceattachment.md).</span><span class="sxs-lookup"><span data-stu-id="17382-115">Programmatically, this is a [referenceAttachment](../resources/referenceattachment.md) resource.</span></span> <span data-ttu-id="17382-116">См. [пример 5](#example-5-get-the-properties-of-a-reference-attachment).</span><span class="sxs-lookup"><span data-stu-id="17382-116">See [example 5](#example-5-get-the-properties-of-a-reference-attachment).</span></span>

<span data-ttu-id="17382-117">Все эти типы вложений являются производными от ресурса [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="17382-117">All these types of attachments are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

### <a name="get-the-raw-contents-of-a-file-or-item-attachment"></a><span data-ttu-id="17382-118">Получение необработанного содержимого вложенного файла или элемента</span><span class="sxs-lookup"><span data-stu-id="17382-118">Get the raw contents of a file or item attachment</span></span>
<span data-ttu-id="17382-119">Чтобы получить необработанное содержимое вложенного файла или элемента, вы можете добавить сегмент пути `/$value`.</span><span class="sxs-lookup"><span data-stu-id="17382-119">You can append the path segment `/$value` to get the raw contents of a file or item attachment.</span></span> 

<span data-ttu-id="17382-120">Для вложенного файла тип содержимого определяется исходя из его исходного типа.</span><span class="sxs-lookup"><span data-stu-id="17382-120">For a file attachment, the content type is based on its original content type.</span></span> <span data-ttu-id="17382-121">Пример [6](#example-6-get-the-raw-contents-of-a-file-attachment-on-a-message).</span><span class="sxs-lookup"><span data-stu-id="17382-121">See an [example 6](#example-6-get-the-raw-contents-of-a-file-attachment-on-a-message).</span></span>

<span data-ttu-id="17382-122">Для вложенного элемента, которое является [контактом ](../resources/contact.md), [событием ](../resources/event.md) и [сообщением](../resources/message.md), возвращаемое необработанное содержимое будет иметь формат MIME.</span><span class="sxs-lookup"><span data-stu-id="17382-122">For an item attachment that is a [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md), the raw contents returned is in MIME format.</span></span>

| <span data-ttu-id="17382-123">тип вложенного элемента</span><span class="sxs-lookup"><span data-stu-id="17382-123">Item attachment type</span></span>  | <span data-ttu-id="17382-124">Возвращаемое необработанное содержимое</span><span class="sxs-lookup"><span data-stu-id="17382-124">Raw contents returned</span></span> |
|:-----------|:----------|
| <span data-ttu-id="17382-125">**контакт**</span><span class="sxs-lookup"><span data-stu-id="17382-125">**contact**</span></span> | <span data-ttu-id="17382-126">[vCard](http://www.faqs.org/rfcs/rfc2426.html) в формате MIME.</span><span class="sxs-lookup"><span data-stu-id="17382-126">[vCard](http://www.faqs.org/rfcs/rfc2426.html) MIME format.</span></span> <span data-ttu-id="17382-127">См. [пример 7](#example-7-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message).</span><span class="sxs-lookup"><span data-stu-id="17382-127">See [example 7](#example-7-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message).</span></span> |
| <span data-ttu-id="17382-128">**событие**</span><span class="sxs-lookup"><span data-stu-id="17382-128">**event**</span></span> | <span data-ttu-id="17382-129">iCal в формате MIME.</span><span class="sxs-lookup"><span data-stu-id="17382-129">iCal MIME format.</span></span> <span data-ttu-id="17382-130">См. [пример 8](#example-8-get-the-mime-raw-contents-of-an-event-attachment-on-a-message).</span><span class="sxs-lookup"><span data-stu-id="17382-130">See [example 8](#example-8-get-the-mime-raw-contents-of-an-event-attachment-on-a-message).</span></span> |
| <span data-ttu-id="17382-131">**сообщение**</span><span class="sxs-lookup"><span data-stu-id="17382-131">**message**</span></span> | <span data-ttu-id="17382-132">Формат MIME.</span><span class="sxs-lookup"><span data-stu-id="17382-132">MIME format.</span></span> <span data-ttu-id="17382-133">См. [пример 9](#example-9-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message).</span><span class="sxs-lookup"><span data-stu-id="17382-133">See [example 9](#example-9-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message).</span></span> |

<span data-ttu-id="17382-134">При попытке получить `$value` вложенной ссылки происходит возврат HTTP 405.</span><span class="sxs-lookup"><span data-stu-id="17382-134">Attempting to get the `$value` of a reference attachment returns HTTP 405.</span></span>

## <a name="permissions"></a><span data-ttu-id="17382-135">Разрешения</span><span class="sxs-lookup"><span data-stu-id="17382-135">Permissions</span></span>

<span data-ttu-id="17382-136">В зависимости от **ресурса (события,** сообщения, **outlookTask** или **сообщения),** к который присоединено вложение и запрашиваемого типа разрешений (делегирован или приложения), разрешение, указанное в следующей таблице, является наименее привилегированным, требуемого для вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="17382-136">Depending on the resource (**event**, **message**, **outlookTask**, or **post**) that the attachment is attached to and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="17382-137">Чтобы получить дополнительные сведения, в том числе о [соблюдении осторожности](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) перед выбором разрешений с повышенными привилегиями, найдите следующие разрешения в разделе [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17382-137">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="17382-138">Поддерживаемый ресурс</span><span class="sxs-lookup"><span data-stu-id="17382-138">Supported resource</span></span> | <span data-ttu-id="17382-139">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="17382-139">Delegated (work or school account)</span></span> | <span data-ttu-id="17382-140">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="17382-140">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17382-141">Для приложений</span><span class="sxs-lookup"><span data-stu-id="17382-141">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="17382-142">event</span><span class="sxs-lookup"><span data-stu-id="17382-142">event</span></span>](../resources/event.md) | <span data-ttu-id="17382-143">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="17382-143">Calendars.Read</span></span> | <span data-ttu-id="17382-144">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="17382-144">Calendars.Read</span></span> | <span data-ttu-id="17382-145">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="17382-145">Calendars.Read</span></span> |
| [<span data-ttu-id="17382-146">message</span><span class="sxs-lookup"><span data-stu-id="17382-146">message</span></span>](../resources/message.md) | <span data-ttu-id="17382-147">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="17382-147">Mail.Read</span></span> | <span data-ttu-id="17382-148">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="17382-148">Mail.Read</span></span> | <span data-ttu-id="17382-149">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="17382-149">Mail.Read</span></span> |
| [<span data-ttu-id="17382-150">outlookTask</span><span class="sxs-lookup"><span data-stu-id="17382-150">outlookTask</span></span>](../resources/outlooktask.md) |  <span data-ttu-id="17382-151">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="17382-151">Tasks.Read</span></span> | <span data-ttu-id="17382-152">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="17382-152">Tasks.Read</span></span> | <span data-ttu-id="17382-153">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="17382-153">Not supported</span></span> |
| [<span data-ttu-id="17382-154">post</span><span class="sxs-lookup"><span data-stu-id="17382-154">post</span></span>](../resources/post.md) | <span data-ttu-id="17382-155">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="17382-155">Group.Read.All</span></span> | <span data-ttu-id="17382-156">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="17382-156">Not supported</span></span> | <span data-ttu-id="17382-157">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="17382-157">Not supported</span></span> |


<!--
* If accessing attachments in group events or posts: Group.Read.All
-->

## <a name="http-request"></a><span data-ttu-id="17382-158">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17382-158">HTTP request</span></span>

<span data-ttu-id="17382-159">В этом разделе показан синтаксис запроса HTTP GET для каждого из сущностями[(событие,](../resources/event.md) [сообщение,](../resources/message.md) [Outlook](../resources/outlooktask.md)задачи и публикации), [](../resources/post.md)которые поддерживают вложения:</span><span class="sxs-lookup"><span data-stu-id="17382-159">This section shows the HTTP GET request syntax for each of the entities ([event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), and [post](../resources/post.md)) that support attachments:</span></span>

- <span data-ttu-id="17382-160">Чтобы получить свойства и связи вложения, укажите ID  вложения для индексации в коллекцию вложений, присоединенную к [](../resources/post.md) указанному событию, [](../resources/event.md)сообщению, [](../resources/message.md)Outlook задаче или почтовому [экземпляру.](../resources/outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="17382-160">To get the properties and relationships of an attachment, specify the attachment ID to index into the **attachments** collection, attached to the specified [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) instance.</span></span>
- <span data-ttu-id="17382-161">Если вложением является файл или элемент Outlook (контакт, событие или сообщение), вы можете также получить необработанное содержимое вложения, добавив сегмент пути `/$value` в URL-адрес запроса.</span><span class="sxs-lookup"><span data-stu-id="17382-161">If the attachment is a file or Outlook item (contact, event, or message), you can further get the raw contents of the attachment by appending the path segment `/$value` to the request URL.</span></span>

<span data-ttu-id="17382-162">Вложение [события:](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="17382-162">An attachment of an [event](../resources/event.md):</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/events/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/events/{id}/attachments/{id}
GET /me/events/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/events/{id}/attachments/{id}/$value
```

<!--
GET /groups/{id}/events/{id}/attachments/{id}
-->

<span data-ttu-id="17382-163">Вложение [сообщения в](../resources/message.md) почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="17382-163">An attachment of a [message](../resources/message.md) in a user's mailbox:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
GET /me/messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}/$value
```

<span data-ttu-id="17382-164">Вложение [сообщения,](../resources/message.md) содержалось в [](../resources/mailfolder.md) почтовом ящике верхнего уровня в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="17382-164">An attachment of a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}/$value
```

<span data-ttu-id="17382-165">Вложение [сообщения,](../resources/message.md) содержалось в детской папке [почтового ящика в](../resources/mailfolder.md) почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="17382-165">An attachment of a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}/$value
```

<span data-ttu-id="17382-166">В предыдущем примере показан один уровень вложения, но сообщение может быть расположено в ребенке ребенка и так далее.</span><span class="sxs-lookup"><span data-stu-id="17382-166">The preceding example shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>

<span data-ttu-id="17382-167">Вложение задачи [Outlook:](../resources/outlooktask.md)</span><span class="sxs-lookup"><span data-stu-id="17382-167">An attachment of an [Outlook task](../resources/outlooktask.md):</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}/attachments/{id}
GET /users/{id}/outlook/tasks/{id}/attachments/{id}
GET /me/outlook/tasks/{id}/attachments/{id}/$value
GET /users/{id}/outlook/tasks/{id}/attachments/{id}/$value
```

<span data-ttu-id="17382-168">Вложение [столба](../resources/post.md) в [потоке,](../resources/conversationthread.md) принадлежащем [разговору](../resources/conversation.md) группы:</span><span class="sxs-lookup"><span data-stu-id="17382-168">An attachment of a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}/$value
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}/$value
```

## <a name="optional-query-parameters"></a><span data-ttu-id="17382-169">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="17382-169">Optional query parameters</span></span>

<span data-ttu-id="17382-170">Этот метод поддерживает некоторые [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="17382-170">This method supports some of the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="17382-171">Используйте параметр `$expand`, чтобы получить свойства вложения элемента (контакта, события или сообщения).</span><span class="sxs-lookup"><span data-stu-id="17382-171">Use `$expand` to get the properties of an item attachment (contact, event, or message).</span></span> <span data-ttu-id="17382-172">См. [пример 3](#example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message) и [пример 4](#example-4-expand-and-get-the-properties-of-an-item-attached-to-a-message-including-any-attachment-to-the-item).</span><span class="sxs-lookup"><span data-stu-id="17382-172">See [example 3](#example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message) and [example 4](#example-4-expand-and-get-the-properties-of-an-item-attached-to-a-message-including-any-attachment-to-the-item).</span></span>

## <a name="request-headers"></a><span data-ttu-id="17382-173">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="17382-173">Request headers</span></span>

| <span data-ttu-id="17382-174">Имя</span><span class="sxs-lookup"><span data-stu-id="17382-174">Name</span></span>       | <span data-ttu-id="17382-175">Тип</span><span class="sxs-lookup"><span data-stu-id="17382-175">Type</span></span> | <span data-ttu-id="17382-176">Описание</span><span class="sxs-lookup"><span data-stu-id="17382-176">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="17382-177">Authorization</span><span class="sxs-lookup"><span data-stu-id="17382-177">Authorization</span></span>  | <span data-ttu-id="17382-178">string</span><span class="sxs-lookup"><span data-stu-id="17382-178">string</span></span>  | <span data-ttu-id="17382-p110">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="17382-p110">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="17382-181">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="17382-181">Request body</span></span>

<span data-ttu-id="17382-182">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="17382-182">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17382-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="17382-183">Response</span></span>

<span data-ttu-id="17382-184">В случае успешной работы метод GET возвращает `200 OK` код ответа.</span><span class="sxs-lookup"><span data-stu-id="17382-184">If successful, the GET method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="17382-185">При получении свойств и связей вложения текст ответа включает объект [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="17382-185">If you're getting the properties and relationships of an attachment, the response body includes an [attachment](../resources/attachment.md) object.</span></span>
<span data-ttu-id="17382-186">Кроме того, возвращаются свойства этого типа вложения: [fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) или [referenceAttachment](../resources/referenceattachment.md).</span><span class="sxs-lookup"><span data-stu-id="17382-186">The properties of that type of attachment are returned: [fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md), or [referenceAttachment](../resources/referenceattachment.md).</span></span>

<span data-ttu-id="17382-187">При получении необработанного содержимого вложенного файла или элемента, текст ответа содержит необработанное значение вложения.</span><span class="sxs-lookup"><span data-stu-id="17382-187">If you're getting the raw contents of a file or item attachment, the response body includes the raw value of the attachment.</span></span>

## <a name="examples"></a><span data-ttu-id="17382-188">Примеры</span><span class="sxs-lookup"><span data-stu-id="17382-188">Examples</span></span>

### <a name="example-1-get-the-properties-of-a-file-attachment"></a><span data-ttu-id="17382-189">Пример 1. Получение свойств вложенного файла</span><span class="sxs-lookup"><span data-stu-id="17382-189">Example 1: Get the properties of a file attachment</span></span>

#### <a name="request"></a><span data-ttu-id="17382-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="17382-190">Request</span></span>

<span data-ttu-id="17382-191">Вот пример запроса на то, чтобы получить свойства вложения файла в сообщении.</span><span class="sxs-lookup"><span data-stu-id="17382-191">Here is an example of the request to get the properties of a file attachment on a message.</span></span>

# <a name="http"></a>[<span data-ttu-id="17382-192">HTTP</span><span class="sxs-lookup"><span data-stu-id="17382-192">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_file_attachment_beta",
  "sampleKeys": ["AAMkAGUzY5QKjAAA=","AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8="]
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkAGUzY5QKjAAA=/attachments/AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=
```
# <a name="c"></a>[<span data-ttu-id="17382-193">C#</span><span class="sxs-lookup"><span data-stu-id="17382-193">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-file-attachment-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="17382-194">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17382-194">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-file-attachment-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="17382-195">Objective-C</span><span class="sxs-lookup"><span data-stu-id="17382-195">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-file-attachment-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="17382-196">Java</span><span class="sxs-lookup"><span data-stu-id="17382-196">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-file-attachment-beta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="17382-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="17382-197">Response</span></span>

<span data-ttu-id="17382-198">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="17382-198">Here is an example of the response.</span></span> <span data-ttu-id="17382-199">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="17382-199">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_file_attachment_beta",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/messages('AAMkAGUzY5QKjAAA%3D')/attachments/$entity",
    "@odata.type": "#microsoft.graph.fileAttachment",
    "id": "AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=",
    "lastModifiedDateTime": "2019-04-02T03:41:29Z",
    "name": "Draft sales invoice template.docx",
    "contentType": "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
    "size": 13068,
    "isInline": false,
    "contentId": null,
    "contentLocation": null,
    "contentBytes": "UEsDBBQABgAIAAAAIQ4AAAAA"
}
```

### <a name="example-2-get-the-properties-of-an-item-attachment"></a><span data-ttu-id="17382-200">Пример 2. Получение свойств вложенного элемента</span><span class="sxs-lookup"><span data-stu-id="17382-200">Example 2: Get the properties of an item attachment</span></span>

#### <a name="request"></a><span data-ttu-id="17382-201">Запрос</span><span class="sxs-lookup"><span data-stu-id="17382-201">Request</span></span>

<span data-ttu-id="17382-202">В следующем примере показано, как получить вложенный элемент в сообщении.</span><span class="sxs-lookup"><span data-stu-id="17382-202">The next example shows how to get an item attachment on a message.</span></span> <span data-ttu-id="17382-203">Возвращаются свойства **itemAttachment**.</span><span class="sxs-lookup"><span data-stu-id="17382-203">The properties of the **itemAttachment** are returned.</span></span>

# <a name="http"></a>[<span data-ttu-id="17382-204">HTTP</span><span class="sxs-lookup"><span data-stu-id="17382-204">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_item_attachment",
  "sampleKeys": ["AAMkADA1M-zAAA=","AAMkADA1M-CJKtzmnlcqVgqI="]
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')
```
# <a name="c"></a>[<span data-ttu-id="17382-205">C#</span><span class="sxs-lookup"><span data-stu-id="17382-205">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="17382-206">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17382-206">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="17382-207">Objective-C</span><span class="sxs-lookup"><span data-stu-id="17382-207">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="17382-208">Java</span><span class="sxs-lookup"><span data-stu-id="17382-208">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="17382-209">Отклик</span><span class="sxs-lookup"><span data-stu-id="17382-209">Response</span></span>
<span data-ttu-id="17382-210">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="17382-210">Here is an example of the response.</span></span> <span data-ttu-id="17382-211">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="17382-211">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_item_attachment",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1M-CJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false
}
```

### <a name="example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message"></a><span data-ttu-id="17382-212">Пример 3. Развертывание и изменение свойств элемента, вложенного в сообщение</span><span class="sxs-lookup"><span data-stu-id="17382-212">Example 3: Expand and get the properties of the item attached to a message</span></span>
#### <a name="request"></a><span data-ttu-id="17382-213">Запрос</span><span class="sxs-lookup"><span data-stu-id="17382-213">Request</span></span>

<span data-ttu-id="17382-214">В следующем примере показано, как использовать `$expand` для получения свойств элемента (контакт, событие или сообщение), вложенного в сообщение.</span><span class="sxs-lookup"><span data-stu-id="17382-214">The next example shows how to use `$expand` to get the properties of the item (contact, event, or message) that is attached to the message.</span></span> <span data-ttu-id="17382-215">В этом примере вложением является сообщением. Свойства вложенного сообщения также возвращаются.</span><span class="sxs-lookup"><span data-stu-id="17382-215">In this example, that item is a message; the properties of that attached message are also returned.</span></span>

# <a name="http"></a>[<span data-ttu-id="17382-216">HTTP</span><span class="sxs-lookup"><span data-stu-id="17382-216">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_and_expand_item_attachment",
  "sampleKeys": ["AAMkADA1M-zAAA=","AAMkADA1M-CJKtzmnlcqVgqI="]
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')/?$expand=microsoft.graph.itemattachment/item
```
# <a name="c"></a>[<span data-ttu-id="17382-217">C#</span><span class="sxs-lookup"><span data-stu-id="17382-217">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-and-expand-item-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="17382-218">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17382-218">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-and-expand-item-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="17382-219">Objective-C</span><span class="sxs-lookup"><span data-stu-id="17382-219">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-and-expand-item-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="17382-220">Java</span><span class="sxs-lookup"><span data-stu-id="17382-220">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-and-expand-item-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="17382-221">Отклик</span><span class="sxs-lookup"><span data-stu-id="17382-221">Response</span></span>
<span data-ttu-id="17382-222">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="17382-222">Here is an example of the response.</span></span> <span data-ttu-id="17382-223">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="17382-223">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_and_expand_item_attachment",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments/$entity",
  "@odata.type":"#microsoft.graph.itemAttachment",
  "id":"AAMkADA1MCJKtzmnlcqVgqI=",
  "lastModifiedDateTime":"2017-07-21T00:20:34Z",
  "name":"Reminder - please bring laptop",
  "contentType":null,
  "size":32005,
  "isInline":false,
  "item@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments('AAMkADA1M-CJKtzmnlcqVgqI%3D')/microsoft.graph.itemAttachment/item/$entity",
  "item":{
    "@odata.type":"#microsoft.graph.message",
    "id":"",
    "createdDateTime":"2017-07-21T00:20:41Z",
    "lastModifiedDateTime":"2017-07-21T00:20:34Z",
    "receivedDateTime":"2017-07-21T00:19:55Z",
    "sentDateTime":"2017-07-21T00:19:52Z",
    "hasAttachments":false,
    "internetMessageId":"<BY2PR15MB05189A084C01F466709E414F9CA40@BY2PR15MB0518.namprd15.prod.outlook.com>",
    "subject":"Reminder - please bring laptop",
    "bodyPreview": "PFA\r\n\r\nThanks,\r\nRob",
    "importance":"normal",
    "conversationId":"AAQkADA1MzMyOGI4LTlkZDctNDkzYy05M2RiLTdiN2E1NDE3MTRkOQAQAMG_NSCMBqdKrLa2EmR-lO0=",
    "conversationIndex":"AQHTAbcSwb41IIwGp0qstrYSZH+U7Q==",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":false,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADA1M3MTRkOQAAAA%3D%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "internetMessageHeaders": [ ],
    "body":{
      "contentType":"html",
      "content":"<html><head>\r\n</head>\r\n<body>\r\n</body>\r\n</html>"
    },
    "sender":{
      "emailAddress":{
        "name":"Adele Vance",
        "address":"AdeleV@contoso.onmicrosoft.com"
      }
    },
    "from":{
      "emailAddress":{
        "name":"Adele Vance",
        "address":"AdeleV@contoso.onmicrosoft.com"
      }
    },
    "toRecipients":[
      {
        "emailAddress":{
          "name":"Alex Wilbur",
          "address":"AlexW@contoso.onmicrosoft.com"
        }
      }
    ],
    "ccRecipients":[
      {
        "emailAddress":{
          "name":"Adele Vance",
          "address":"AdeleV@contoso.onmicrosoft.com"
        }
      }
    ],
    "flag":{
      "flagStatus":"notFlagged"
    }
  }
}
```

### <a name="example-4-expand-and-get-the-properties-of-an-item-attached-to-a-message-including-any-attachment-to-the-item"></a><span data-ttu-id="17382-224">Пример 4. Развертывание и получение свойств элемента, вложенного в сообщение, включая любые вложения элемента</span><span class="sxs-lookup"><span data-stu-id="17382-224">Example 4: Expand and get the properties of an item attached to a message, including any attachment to the item</span></span>
#### <a name="request"></a><span data-ttu-id="17382-225">Запрос</span><span class="sxs-lookup"><span data-stu-id="17382-225">Request</span></span>
<span data-ttu-id="17382-226">В следующем примере используется тот же запрос, что и в [примере 3](#example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message), чтобы получить свойства вложения элемента в сообщении с помощью параметра `$expand`.</span><span class="sxs-lookup"><span data-stu-id="17382-226">The next example uses the same request as in [example 3](#example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message) to get the properties of an item attachment on a message by using `$expand`.</span></span> <span data-ttu-id="17382-227">В данном случае, так как вложенный элемент также содержит вложенный файл, в отклик также включаются свойства вложенного файла.</span><span class="sxs-lookup"><span data-stu-id="17382-227">In this case, because the attached item also has a file attachment, the response includes the properties of the file attachment as well.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_and_expand_nested_item_attachment",
  "sampleKeys": ["AAMkADA1M-zAAA=","AAMkADA1M-CJKtzmnlcqVgqI="]
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')/?$expand=microsoft.graph.itemattachment/item
```

#### <a name="response"></a><span data-ttu-id="17382-228">Отклик</span><span class="sxs-lookup"><span data-stu-id="17382-228">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "get_and_expand_nested_item_attachment",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments(microsoft.graph.itemAttachment/item())/$entity",
    "@odata.type": "#microsoft.graph.itemAttachment",
    "id": "AAMkADA1MCJKtzmnlcqVgqI=",
    "lastModifiedDateTime": "2021-01-06T13:28:11Z",
    "name": "Nested Message With Attachment",
    "contentType": null,
    "size": 465916,
    "isInline": false,
    "item@odata.context": "https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments('AAMkADA1M-CJKtzmnlcqVgqI%3D')/microsoft.graph.itemAttachment/item/$entity",
    "item": {
        "@odata.type": "#microsoft.graph.message",
        "id": "",
        "createdDateTime": "2021-01-06T13:28:30Z",
        "lastModifiedDateTime": "2021-01-06T13:27:40Z",
        "receivedDateTime": "2021-01-06T13:27:25Z",
        "sentDateTime": "2021-01-06T13:27:04Z",
        "hasAttachments": true,
        "internetMessageId": "<BY2PR15MB05189A084C01F466709E414F9CA40@BY2PR15MB0518.namprd15.prod.outlook.com>",
        "subject": "Nested Message With Attachment",
        "bodyPreview": "PFAThanks,Adele",
        "importance": "normal",
        "conversationId": "AAQkADg3NTY5MDg4LWMzYmQtNDQzNi05OTgwLWQyZjg2YWQwMTNkZAAQAO6hkp84oMdGm6ZBsSH72sE=",
        "conversationIndex": "AQHW5C+U7qGSnzigx0abpkGxIfvawQ==",
        "isDeliveryReceiptRequested": false,
        "isReadReceiptRequested": false,
        "isRead": true,
        "isDraft": false,
        "webLink": "https://outlook.office365.com/owa/?ItemID=AAMkADA1M3MTRkOQAAAA%3D%3D&exvsurl=1&viewmodel=ItemAttachment",
        "internetMessageHeaders": [],
        "body": {
            "contentType": "html",
            "content": "<html><head>\r\n</head>\r\n<body>\r\n</body>\r\n</html>"
        },
        "sender": {
            "emailAddress": {
                "name": "Adele Vance",
                "address": "Adele.Vance@microsoft.com"
            }
        },
        "from": {
            "emailAddress": {
                "name": "Adele Vance",
                "address": "Adele.Vance@microsoft.com"
            }
        },
        "toRecipients": [
            {
                "emailAddress": {
                    "name": "Adele Vance",
                    "address": "Adele.Vance@microsoft.com"
                }
            }
        ],
        "flag": {
            "flagStatus": "notFlagged"
        },
        "attachments@odata.context": "https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/messages('AAMkADA1M-zAAA%3D')/attachments('AAMkADA1M-CJKtzmnlcqVgqI%3D')/microsoft.graph.itemAttachment/microsoft.graph.itemAttachment/item/microsoft.graph.message/microsoft.graph.message/microsoft.graph.message/microsoft.graph.message/microsoft.graph.message/microsoft.graph.message/microsoft.graph.message/attachments",
        "attachments": [
            {
                "@odata.type": "#microsoft.graph.fileAttachment",
                "@odata.mediaContentType": "application/pdf",
                "id": "AAMkADg3NTYULmbsDYNg==",
                "lastModifiedDateTime": "2021-01-21T14:56:18Z",
                "name": "Info.pdf",
                "contentType": "application/pdf",
                "size": 417351,
                "isInline": false,
                "contentId": null,
                "contentLocation": null,
                "contentBytes": "JVBERi0xLjUNCiW1tbW1DQoxIDAgb2JqDQo8PC9UeXBlL0NhdGFsb2cvUGFnZXMgMiAwIFIvTGFuZyhlbi1JTikgL1N0cnVjdFRyZWVSb29"
            }
        ]
    }
}
```

### <a name="example-5-get-the-properties-of-a-reference-attachment"></a><span data-ttu-id="17382-229">Пример 5. Получение свойств вложенной ссылки</span><span class="sxs-lookup"><span data-stu-id="17382-229">Example 5: Get the properties of a reference attachment</span></span>

#### <a name="request"></a><span data-ttu-id="17382-230">Запрос</span><span class="sxs-lookup"><span data-stu-id="17382-230">Request</span></span>

<span data-ttu-id="17382-231">Ниже приведен пример запроса на получение вложенной ссылки из данных, касающихся события.</span><span class="sxs-lookup"><span data-stu-id="17382-231">Here is an example of the request to get a reference attachment on an event.</span></span>

# <a name="http"></a>[<span data-ttu-id="17382-232">HTTP</span><span class="sxs-lookup"><span data-stu-id="17382-232">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_reference_attachment",
  "sampleKeys": ["AAMkAGE1M88AADUv0uAAAG=","AAMkAGE1Mg72tgf7hJp0PICVGCc0g="]
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/AAMkAGE1M88AADUv0uAAAG=/attachments/AAMkAGE1Mg72tgf7hJp0PICVGCc0g=
```
# <a name="c"></a>[<span data-ttu-id="17382-233">C#</span><span class="sxs-lookup"><span data-stu-id="17382-233">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-reference-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="17382-234">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17382-234">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-reference-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="17382-235">Objective-C</span><span class="sxs-lookup"><span data-stu-id="17382-235">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-reference-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="17382-236">Java</span><span class="sxs-lookup"><span data-stu-id="17382-236">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-reference-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="17382-237">Отклик</span><span class="sxs-lookup"><span data-stu-id="17382-237">Response</span></span>
<span data-ttu-id="17382-238">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="17382-238">Here is an example of the response.</span></span> <span data-ttu-id="17382-239">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="17382-239">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_reference_attachment",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/ddfcd489-628b-40d7-b48b-57002df800e5/events/AAMkAGE1M88AADUv0uAAAG%3D/attachments/$entity",
  "@odata.type": "#microsoft.graph.referenceAttachment",
  "id": "AAMkAGE1Mg72tgf7hJp0PCGVCIc0g=",
  "lastModifiedDateTime": "2016-03-12T06:04:38Z",
  "name": "Personal pictures",
  "contentType": null,
  "size": 382,
  "isInline": false,
  "sourceUrl": "https://contoso.com/personal/mario_contoso_net/Documents/Pics",
  "providerType": "oneDriveConsumer",
  "thumbnailUrl": null,
  "previewUrl": null,
  "permission": "edit",
  "isFolder": true
}
```


### <a name="example-6-get-the-raw-contents-of-a-file-attachment-on-a-message"></a><span data-ttu-id="17382-240">Пример 6. Получение необработанного содержимого вложенного файла в сообщении</span><span class="sxs-lookup"><span data-stu-id="17382-240">Example 6: Get the raw contents of a file attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="17382-241">Запрос</span><span class="sxs-lookup"><span data-stu-id="17382-241">Request</span></span>

<span data-ttu-id="17382-242">Ниже приведен пример запроса на получение необработанного содержимого файла Word, вложенного в сообщение.</span><span class="sxs-lookup"><span data-stu-id="17382-242">Here is an example of the request to get the raw contents of a Word file that has been attached to a message.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_value_file_attachment",
  "sampleKeys": ["AAMkAGUzY5QKjAAA=","AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGUzY5QKjAAA=/attachments/AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=/$value
```

#### <a name="response"></a><span data-ttu-id="17382-243">Отклик</span><span class="sxs-lookup"><span data-stu-id="17382-243">Response</span></span>
<span data-ttu-id="17382-244">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="17382-244">Here is an example of the response.</span></span> <span data-ttu-id="17382-245">Фактический текст ответа содержит необработанные байты вложенного файла, которые кратко описаны ниже.</span><span class="sxs-lookup"><span data-stu-id="17382-245">The actual response body includes the raw bytes of the file attachment, which are abbreviated here for brevity.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_value_file_attachment",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK

{Raw bytes of the file}
```


### <a name="example-7-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message"></a><span data-ttu-id="17382-246">Пример 7. Получение необработанного содержимого MIME вложенного контакта в сообщении</span><span class="sxs-lookup"><span data-stu-id="17382-246">Example 7: Get the MIME raw contents of a contact attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="17382-247">Запрос</span><span class="sxs-lookup"><span data-stu-id="17382-247">Request</span></span>

<span data-ttu-id="17382-248">Ниже приведен пример запроса на получение необработанного содержимого элемента контакта, вложенного в сообщение.</span><span class="sxs-lookup"><span data-stu-id="17382-248">Here is an example of the request to get the raw contents of a contact item that has been attached to a message.</span></span> 
<!-- {
  "blockType": "ignored",
  "name": "get_value_contact_attachment",
  "sampleKeys": ["AAMkADI5MAAGjk2PxAAA=","AAMkADI5MAAGjk2PxAAABEgAQACEJqrbJZBNIlr3pGFvd9K8="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkADI5MAAGjk2PxAAA=/attachments/AAMkADI5MAAGjk2PxAAABEgAQACEJqrbJZBNIlr3pGFvd9K8=/$value
```

#### <a name="response"></a><span data-ttu-id="17382-249">Отклик</span><span class="sxs-lookup"><span data-stu-id="17382-249">Response</span></span>
<span data-ttu-id="17382-250">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="17382-250">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "ignored",
  "name": "get_value_contact_attachment",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK

BEGIN:VCARD
PROFILE:VCARD
VERSION:3.0
MAILER:Microsoft Exchange
PRODID:Microsoft Exchange
FN:Alex Wilbur
N:Wilbur;Alex;;;
NOTE:Sunday\, June 10\, 2012 5:44 PM:\nGutter\, window cleaning\, pressure 
 washing\, roof debris blowing\n
ORG:Contoso;
CLASS:PUBLIC
ADR;TYPE=WORK,PREF:;;4567 Main St;Buffalo;NY;98052;United States of America
LABEL;TYPE=WORK,PREF:4567 Main St\nBuffalo\, NY 98052
ADR;TYPE=HOME:;;;;;;
ADR;TYPE=POSTAL:;;;;;;
TEL;TYPE=WORK:(425) 555-0100
TITLE:
X-MS-IMADDRESS:
REV;VALUE=DATE-TIME:2019-04-09T02:13:31,161Z
END:VCARD
```


### <a name="example-8-get-the-mime-raw-contents-of-an-event-attachment-on-a-message"></a><span data-ttu-id="17382-251">Пример 8. Получение необработанного содержимого MIME вложенного события в сообщении</span><span class="sxs-lookup"><span data-stu-id="17382-251">Example 8: Get the MIME raw contents of an event attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="17382-252">Запрос</span><span class="sxs-lookup"><span data-stu-id="17382-252">Request</span></span>

<span data-ttu-id="17382-253">Ниже приведен пример запроса на получение необработанного содержимого события, вложенного в сообщение.</span><span class="sxs-lookup"><span data-stu-id="17382-253">Here is an example of the request to get the raw contents of an event that has been attached to a message.</span></span> 
<!-- {
  "blockType": "ignored",
  "name": "get_value_event_attachment",
  "sampleKeys": ["AAMkADVIOAAA=","AAMkADVIOAAABEgAQACvkutl6c4FMifPyS6NvXsM="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkADVIOAAA=/attachments/AAMkADVIOAAABEgAQACvkutl6c4FMifPyS6NvXsM=/$value
```

#### <a name="response"></a><span data-ttu-id="17382-254">Отклик</span><span class="sxs-lookup"><span data-stu-id="17382-254">Response</span></span>
<span data-ttu-id="17382-255">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="17382-255">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "ignored",
  "name": "get_value_event_attachment",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK

BEGIN:VCALENDAR
METHOD:PUBLISH
PRODID:Microsoft Exchange Server 2010
VERSION:2.0
BEGIN:VTIMEZONE
TZID:Pacific Standard Time
BEGIN:STANDARD
DTSTART:16010101T020000
TZOFFSETFROM:-0700
TZOFFSETTO:-0800
RRULE:FREQ=YEARLY;INTERVAL=1;BYDAY=1SU;BYMONTH=11
END:STANDARD
BEGIN:DAYLIGHT
DTSTART:16010101T020000
TZOFFSETFROM:-0800
TZOFFSETTO:-0700
RRULE:FREQ=YEARLY;INTERVAL=1;BYDAY=2SU;BYMONTH=3
END:DAYLIGHT
END:VTIMEZONE
BEGIN:VEVENT
ORGANIZER;CN=Adele Vance:MAILTO:adelev@contoso.com
ATTENDEE;ROLE=REQ-PARTICIPANT;PARTSTAT=NEEDS-ACTION;RSVP=TRUE;CN=Adele Vance:MAILTO:adelev@contoso.com
DESCRIPTION;LANGUAGE=en-US:\n
UID:040000008200
SUMMARY;LANGUAGE=en-US:Review Megan's docs
DTSTART;TZID=Pacific Standard Time:20190409T140000
DTEND;TZID=Pacific Standard Time:20190409T160000
CLASS:PUBLIC
PRIORITY:5
DTSTAMP:20190409T211833Z
TRANSP:OPAQUE
STATUS:CONFIRMED
SEQUENCE:0
LOCATION;LANGUAGE=en-US:
X-MICROSOFT-CDO-APPT-SEQUENCE:0
X-MICROSOFT-CDO-OWNERAPPTID:0
X-MICROSOFT-CDO-BUSYSTATUS:BUSY
X-MICROSOFT-CDO-INTENDEDSTATUS:BUSY
X-MICROSOFT-CDO-ALLDAYEVENT:FALSE
X-MICROSOFT-CDO-IMPORTANCE:1
X-MICROSOFT-CDO-INSTTYPE:0
X-MICROSOFT-DONOTFORWARDMEETING:FALSE
X-MICROSOFT-DISALLOW-COUNTER:FALSE
X-MICROSOFT-LOCATIONS:[]
BEGIN:VALARM
DESCRIPTION:REMINDER
TRIGGER;RELATED=START:-PT15M
ACTION:DISPLAY
END:VALARM
END:VEVENT
END:VCALENDAR
```


### <a name="example-9-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message"></a><span data-ttu-id="17382-256">Пример 9. Получение необработанного содержимого MIME вложенного элемента приглашения на собрание в сообщении</span><span class="sxs-lookup"><span data-stu-id="17382-256">Example 9: Get the MIME raw contents of a meeting invitation item attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="17382-257">Запрос</span><span class="sxs-lookup"><span data-stu-id="17382-257">Request</span></span>

<span data-ttu-id="17382-258">Ниже приведен пример запроса на получение необработанного содержимого приглашения на собрание (типа [eventMessage](../resources/eventmessage.md)), вложенного в сообщение.</span><span class="sxs-lookup"><span data-stu-id="17382-258">Here is an example of the request to get the raw contents of a meeting invitation (of the [eventMessage](../resources/eventmessage.md) type) that has been attached to a message.</span></span> <span data-ttu-id="17382-259">Сущность **eventMessage** основана на типе **сообщения**.</span><span class="sxs-lookup"><span data-stu-id="17382-259">The **eventMessage** entity is based on the **message** type.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_value_message_attachment",
  "sampleKeys": ["AAMkAGUzY5QKiAAA=","AAMkAGUzY5QKiAAABEgAQAK8ktgiIO19OqkvUZAqLmyQ="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGUzY5QKiAAA=/attachments/AAMkAGUzY5QKiAAABEgAQAK8ktgiIO19OqkvUZAqLmyQ=/$value
```

#### <a name="response"></a><span data-ttu-id="17382-260">Отклик</span><span class="sxs-lookup"><span data-stu-id="17382-260">Response</span></span>
<span data-ttu-id="17382-261">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="17382-261">Here is an example of the response.</span></span> 

<span data-ttu-id="17382-262">В тексте ответа содержится приложение **eventMessage** в формате MIME.</span><span class="sxs-lookup"><span data-stu-id="17382-262">The response body includes the **eventMessage** attachment in MIME format.</span></span> <span data-ttu-id="17382-263">Текст **eventMessage** усекается для краткости.</span><span class="sxs-lookup"><span data-stu-id="17382-263">The body of the  **eventMessage** is truncated for brevity.</span></span> <span data-ttu-id="17382-264">Полный текст сообщения возвращается от фактического вызова.</span><span class="sxs-lookup"><span data-stu-id="17382-264">The full message body is returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_value_message_attachment",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK

From: Megan Bowen <MeganB@contoso.OnMicrosoft.com>
To: Adele Vance <AdeleV@contoso.OnMicrosoft.com>
Subject: Let's go for lunch
Thread-Topic: Let's go for lunch
Thread-Index: AdTPqxOmg4AXoJV960a1j5NrJCHYjA==
X-MS-Exchange-MessageSentRepresentingType: 1
Date: Thu, 28 Feb 2019 21:17:58 +0000
Message-ID:
    <CY4PR2201MB1046E9C83FC42478EF4EE283C9750@CY4PR2201MB1046.namprd22.prod.outlook.com>
Content-Language: en-US
X-MS-Has-Attach:
X-MS-Exchange-Organization-SCL: -1
X-MS-TNEF-Correlator:
X-MS-Exchange-Organization-RecordReviewCfmType: 0
Content-Type: multipart/alternative;
    boundary="_000_CY4PR2201MB1046E9C83FC42478EF4EE283C9750CY4PR2201MB1046_"
MIME-Version: 1.0

--_000_CY4PR2201MB1046E9C83FC42478EF4EE283C9750CY4PR2201MB1046_
Content-Type: text/plain; charset="us-ascii"

Does mid month work for you?

--_000_CY4PR2201MB1046E9C83FC42478EF4EE283C9750CY4PR2201MB1046_
Content-Type: text/html; charset="us-ascii"

<html>
<head>
<meta http-equiv="Content-Type" content="text/html; charset=us-ascii">
</head>
<body>
Does mid month work for you?
</body>
</html>

--_000_CY4PR2201MB1046E9C83FC42478EF4EE283C9750CY4PR2201MB1046_
Content-Type: text/calendar; charset="utf-8"; method=REQUEST
Content-Transfer-Encoding: base64

QkVHSU46VkNBTEVOREFSDQpNRVRIT0Q6UkVRVUVTVA0KUFJPRElEOk1pY3Jvc29mdCBFeGNoYW5n


--_000_CY4PR2201MB1046E9C83FC42478EF4EE283C9750CY4PR2201MB1046_--
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
