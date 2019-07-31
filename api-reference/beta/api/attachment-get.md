---
title: Получение вложения
description: Считывание свойств и связей вложений, вложенных в событие, сообщение, задачу Outlook или POST.
localization_priority: Normal
doc_type: apiPageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 09a336da0f2ead60235240b60b3539007df6bd15
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945363"
---
# <a name="get-attachment"></a><span data-ttu-id="291aa-103">Получение вложения</span><span class="sxs-lookup"><span data-stu-id="291aa-103">Get attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="291aa-104">Считывание свойств и связей вложений, вложенных в [событие](../resources/event.md), [сообщение](../resources/message.md), [задачу Outlook](../resources/outlooktask.md)или [POST](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="291aa-104">Read the properties and relationships of an attachment, attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>

<span data-ttu-id="291aa-105">Допустимые типы вложений:</span><span class="sxs-lookup"><span data-stu-id="291aa-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="291aa-106">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="291aa-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="291aa-107">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="291aa-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span> <span data-ttu-id="291aa-108">Вы можете использовать `$expand` для получения других свойств этого элемента.</span><span class="sxs-lookup"><span data-stu-id="291aa-108">You can use `$expand` to further get the properties of that item.</span></span> <span data-ttu-id="291aa-109">См. [пример](#request-2) ниже.</span><span class="sxs-lookup"><span data-stu-id="291aa-109">See an [example](#request-2) below.</span></span>
* <span data-ttu-id="291aa-110">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="291aa-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="291aa-111">Все эти типы ресурсов вложений являются производными от ресурса [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="291aa-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span>

### <a name="get-the-raw-contents-of-a-file-or-item-attachment"></a><span data-ttu-id="291aa-112">Получение необработанного содержимого вложенного файла или элемента</span><span class="sxs-lookup"><span data-stu-id="291aa-112">Get the raw contents of a file or item attachment</span></span>
<span data-ttu-id="291aa-113">Вы можете добавить сегмент `/$value` пути, чтобы получить необработанное содержимое вложения файла или элемента.</span><span class="sxs-lookup"><span data-stu-id="291aa-113">You can append the path segment `/$value` to get the raw contents of a file or item attachment.</span></span> 

<span data-ttu-id="291aa-114">Для вложенного файла тип контента основан на исходном типе контента.</span><span class="sxs-lookup"><span data-stu-id="291aa-114">For a file attachment, the content type is based on its original content type.</span></span> <span data-ttu-id="291aa-115">См. [пример](#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message) ниже.</span><span class="sxs-lookup"><span data-stu-id="291aa-115">See an [example](#example-5-get-the-raw-contents-of-a-file-attachment-on-a-message) below.</span></span>

<span data-ttu-id="291aa-116">Для вложенного элемента, который является [контактом](../resources/contact.md), [событием](../resources/event.md)или [сообщением](../resources/message.md), возвращенное содержимое имеет формат MIME.</span><span class="sxs-lookup"><span data-stu-id="291aa-116">For an item attachment that is a [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md), the raw contents returned is in MIME format.</span></span>

| <span data-ttu-id="291aa-117">Тип вложения элемента</span><span class="sxs-lookup"><span data-stu-id="291aa-117">Item attachment type</span></span>  | <span data-ttu-id="291aa-118">Возвращено необработанное содержимое</span><span class="sxs-lookup"><span data-stu-id="291aa-118">Raw contents returned</span></span> |
|:-----------|:----------|
| <span data-ttu-id="291aa-119">**contact**</span><span class="sxs-lookup"><span data-stu-id="291aa-119">**contact**</span></span> | <span data-ttu-id="291aa-120">[vCard](http://www.faqs.org/rfcs/rfc2426.html) Формат MIME.</span><span class="sxs-lookup"><span data-stu-id="291aa-120">[vCard](http://www.faqs.org/rfcs/rfc2426.html) MIME format.</span></span> <span data-ttu-id="291aa-121">Смотрите [Пример](#example-6-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message).</span><span class="sxs-lookup"><span data-stu-id="291aa-121">See [example](#example-6-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message).</span></span> |
| <span data-ttu-id="291aa-122">**event**</span><span class="sxs-lookup"><span data-stu-id="291aa-122">**event**</span></span> | <span data-ttu-id="291aa-123">формат MIME iCal.</span><span class="sxs-lookup"><span data-stu-id="291aa-123">iCal MIME format.</span></span> <span data-ttu-id="291aa-124">Смотрите [Пример](#example-7-get-the-mime-raw-contents-of-an-event-attachment-on-a-message).</span><span class="sxs-lookup"><span data-stu-id="291aa-124">See [example](#example-7-get-the-mime-raw-contents-of-an-event-attachment-on-a-message).</span></span> |
| <span data-ttu-id="291aa-125">**message**</span><span class="sxs-lookup"><span data-stu-id="291aa-125">**message**</span></span> | <span data-ttu-id="291aa-126">Формат MIME.</span><span class="sxs-lookup"><span data-stu-id="291aa-126">MIME format.</span></span> <span data-ttu-id="291aa-127">Смотрите [Пример](#example-8-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message).</span><span class="sxs-lookup"><span data-stu-id="291aa-127">See [example](#example-8-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message).</span></span> |

<span data-ttu-id="291aa-128">При попытке получить `$value` вложение ссылки возвращается HTTP 405.</span><span class="sxs-lookup"><span data-stu-id="291aa-128">Attempting to get the `$value` of a reference attachment returns HTTP 405.</span></span>

## <a name="permissions"></a><span data-ttu-id="291aa-129">Разрешения</span><span class="sxs-lookup"><span data-stu-id="291aa-129">Permissions</span></span>

<span data-ttu-id="291aa-p106">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="291aa-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="291aa-132">При доступе к вложениям в сообщениях: mail. Read</span><span class="sxs-lookup"><span data-stu-id="291aa-132">If accessing attachments in messages: Mail.Read</span></span>
* <span data-ttu-id="291aa-133">При доступе к вложениям в событиях: Calendars. Read</span><span class="sxs-lookup"><span data-stu-id="291aa-133">If accessing attachments in events: Calendars.Read</span></span>
* <span data-ttu-id="291aa-134">При доступе к вложениям в задачах Outlook: Tasks. Read</span><span class="sxs-lookup"><span data-stu-id="291aa-134">If accessing attachments in Outlook tasks: Tasks.Read</span></span>
* <span data-ttu-id="291aa-135">При доступе к вложениям в записях групп: Group. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="291aa-135">If accessing attachments in group posts: Group.Read.All</span></span>

<!--
* If accessing attachments in group events or posts: Group.Read.All
-->

## <a name="http-request"></a><span data-ttu-id="291aa-136">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="291aa-136">HTTP request</span></span>

<span data-ttu-id="291aa-137">В этом разделе показан синтаксис HTTP-запроса GET для каждой сущности ([событие](../resources/event.md), [сообщение](../resources/message.md), [задача Outlook](../resources/outlooktask.md)или [POST](../resources/post.md)), поддерживающих вложения:</span><span class="sxs-lookup"><span data-stu-id="291aa-137">This section shows the HTTP GET request syntax for each of the entities ([event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md)) that support attachments:</span></span>

- <span data-ttu-id="291aa-138">Чтобы получить свойства и связи вложения, укажите идентификатор вложения для индексирования в коллекции вложений, \*\*\*\* прикрепленных к указанному событию [](../resources/event.md), [сообщению](../resources/message.md), [задаче Outlook](../resources/outlooktask.md)или экземпляру [POST](../resources/post.md) .</span><span class="sxs-lookup"><span data-stu-id="291aa-138">To get the properties and relationships of an attachment, specify the attachment ID to index into the **attachments** collection, attached to the specified [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) instance.</span></span>
- <span data-ttu-id="291aa-139">Если вложение представляет собой файл или элемент Outlook (контакт, событие или сообщение), вы можете получить необработанное содержимое вложения, добавив сегмент `/$value` пути в URL-адрес запроса.</span><span class="sxs-lookup"><span data-stu-id="291aa-139">If the attachment is a file or Outlook item (contact, event, or message), you can further get the raw contents of the attachment by appending the path segment `/$value` to the request URL.</span></span>

<span data-ttu-id="291aa-140">Вложение [события](../resources/event.md):</span><span class="sxs-lookup"><span data-stu-id="291aa-140">An attachment of an [event](../resources/event.md):</span></span>

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

<span data-ttu-id="291aa-141">Вложение [сообщения](../resources/message.md) в почтовый ящик пользователя:</span><span class="sxs-lookup"><span data-stu-id="291aa-141">An attachment of a [message](../resources/message.md) in a user's mailbox:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}
GET /me/messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/messages/{id}/attachments/{id}/$value
```

<span data-ttu-id="291aa-142">Вложение [сообщения](../resources/message.md) , содержащегося на верхнем уровне [mailFolder](../resources/mailfolder.md) в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="291aa-142">An attachment of a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}
GET /me/mailFolders/{id}/messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments/{id}/$value
```

<span data-ttu-id="291aa-143">Вложение [сообщения](../resources/message.md) , содержащегося в дочерней папке [mailFolder](../resources/mailfolder.md) в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="291aa-143">An attachment of a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}/$value
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}/$value
```

<span data-ttu-id="291aa-144">В предыдущем примере показан один уровень вложенности, но сообщение может находиться в дочернем элементе дочернего элемента и т. д.</span><span class="sxs-lookup"><span data-stu-id="291aa-144">The preceding example shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>

<span data-ttu-id="291aa-145">Вложение [задачи Outlook](../resources/outlooktask.md):</span><span class="sxs-lookup"><span data-stu-id="291aa-145">An attachment of an [Outlook task](../resources/outlooktask.md):</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}/attachments/{id}
GET /users/{id}/outlook/tasks/{id}/attachments/{id}
GET /me/outlook/tasks/{id}/attachments/{id}/$value
GET /users/{id}/outlook/tasks/{id}/attachments/{id}/$value
```

<span data-ttu-id="291aa-146">Вложение [записи](../resources/post.md) в [поток](../resources/conversationthread.md) , принадлежащее беседе группы [](../resources/conversation.md) :</span><span class="sxs-lookup"><span data-stu-id="291aa-146">An attachment of a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}/$value
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments/{id}/$value
```

## <a name="optional-query-parameters"></a><span data-ttu-id="291aa-147">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="291aa-147">Optional query parameters</span></span>

<span data-ttu-id="291aa-148">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="291aa-148">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="291aa-149">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="291aa-149">Request headers</span></span>

| <span data-ttu-id="291aa-150">Имя</span><span class="sxs-lookup"><span data-stu-id="291aa-150">Name</span></span>       | <span data-ttu-id="291aa-151">Тип</span><span class="sxs-lookup"><span data-stu-id="291aa-151">Type</span></span> | <span data-ttu-id="291aa-152">Описание</span><span class="sxs-lookup"><span data-stu-id="291aa-152">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="291aa-153">Authorization</span><span class="sxs-lookup"><span data-stu-id="291aa-153">Authorization</span></span>  | <span data-ttu-id="291aa-154">string</span><span class="sxs-lookup"><span data-stu-id="291aa-154">string</span></span>  | <span data-ttu-id="291aa-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="291aa-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="291aa-157">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="291aa-157">Request body</span></span>

<span data-ttu-id="291aa-158">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="291aa-158">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="291aa-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="291aa-159">Response</span></span>

<span data-ttu-id="291aa-160">В случае успешного выполнения метод GET возвращает код `200 OK` отклика.</span><span class="sxs-lookup"><span data-stu-id="291aa-160">If successful, the GET method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="291aa-161">Если вы получаете свойства и связи вложения, текст отклика включает объект [вложения](../resources/attachment.md) .</span><span class="sxs-lookup"><span data-stu-id="291aa-161">If you're getting the properties and relationships of an attachment, the response body includes an [attachment](../resources/attachment.md) object.</span></span>

<span data-ttu-id="291aa-162">Если вы получаете необработанное содержимое вложения файла или элемента, текст отклика включает необработанное значение вложения.</span><span class="sxs-lookup"><span data-stu-id="291aa-162">If you're getting the raw contents of a file or item attachment, the response body includes the raw value of the attachment.</span></span>

## <a name="examples"></a><span data-ttu-id="291aa-163">Примеры</span><span class="sxs-lookup"><span data-stu-id="291aa-163">Examples</span></span>

### <a name="example-1-get-the-properties-of-a-file-attachment"></a><span data-ttu-id="291aa-164">Пример 1: получение свойств вложенного файла</span><span class="sxs-lookup"><span data-stu-id="291aa-164">Example 1: Get the properties of a file attachment</span></span>

#### <a name="request"></a><span data-ttu-id="291aa-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="291aa-165">Request</span></span>

<span data-ttu-id="291aa-166">Ниже приведен пример запроса на получение свойств вложенного файла сообщения.</span><span class="sxs-lookup"><span data-stu-id="291aa-166">Here is an example of the request to get the properties of a file attachment on a message.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="291aa-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="291aa-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_file_attachment",
  "sampleKeys": ["AAMkAGUzY5QKjAAA=","AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGUzY5QKjAAA=/attachments/AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="291aa-168">C#</span><span class="sxs-lookup"><span data-stu-id="291aa-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-file-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="291aa-169">Javascript</span><span class="sxs-lookup"><span data-stu-id="291aa-169">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-file-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="291aa-170">Цель — C</span><span class="sxs-lookup"><span data-stu-id="291aa-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-file-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="291aa-171">Java</span><span class="sxs-lookup"><span data-stu-id="291aa-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-file-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="291aa-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="291aa-172">Response</span></span>

<span data-ttu-id="291aa-p108">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="291aa-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_file_attachment",
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
    "contentBytes": "base64,UEsDBBQABgAIAAAAIQ4AAAAA"
}
```

### <a name="example-2-get-the-properties-of-an-item-attachment"></a><span data-ttu-id="291aa-176">Пример 2: получение свойств вложения элемента</span><span class="sxs-lookup"><span data-stu-id="291aa-176">Example 2: Get the properties of an item attachment</span></span>

#### <a name="request"></a><span data-ttu-id="291aa-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="291aa-177">Request</span></span>

<span data-ttu-id="291aa-178">В первом примере показано, как получить вложенный элемент в сообщении.</span><span class="sxs-lookup"><span data-stu-id="291aa-178">The first example shows how to get an item attachment on a message.</span></span> <span data-ttu-id="291aa-179">Возвращаются свойства **itemAttachment**.</span><span class="sxs-lookup"><span data-stu-id="291aa-179">The properties of the **itemAttachment** are returned.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="291aa-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="291aa-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_item_attachment",
  "sampleKeys": ["AAMkADA1M-zAAA=","AAMkADA1M-CJKtzmnlcqVgqI="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="291aa-181">C#</span><span class="sxs-lookup"><span data-stu-id="291aa-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="291aa-182">Javascript</span><span class="sxs-lookup"><span data-stu-id="291aa-182">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="291aa-183">Цель — C</span><span class="sxs-lookup"><span data-stu-id="291aa-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="291aa-184">Java</span><span class="sxs-lookup"><span data-stu-id="291aa-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="291aa-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="291aa-185">Response</span></span>
<span data-ttu-id="291aa-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="291aa-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-3-expand-and-get-the-properties-of-the-item-attached-to-a-message"></a><span data-ttu-id="291aa-189">Пример 3: разверните и получите свойства элемента, вложенного в сообщение.</span><span class="sxs-lookup"><span data-stu-id="291aa-189">Example 3: Expand and get the properties of the item attached to a message</span></span>
#### <a name="request"></a><span data-ttu-id="291aa-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="291aa-190">Request</span></span>

<span data-ttu-id="291aa-191">В следующем примере показано, как `$expand` получить свойства элемента (Event, Message, Task Task или POST), вложенных в сообщение.</span><span class="sxs-lookup"><span data-stu-id="291aa-191">The next example shows how to use `$expand` to get the properties of the item (event, message, Outlook task, or post) that is attached to the message.</span></span> <span data-ttu-id="291aa-192">В этом примере вложением является сообщением. Свойства вложенного сообщения также возвращаются.</span><span class="sxs-lookup"><span data-stu-id="291aa-192">In this example, that item is a message; the properties of that attached message are also returned.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="291aa-193">HTTP</span><span class="sxs-lookup"><span data-stu-id="291aa-193">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_and_expand_item_attachment",
  "sampleKeys": ["AAMkADA1M-zAAA=","AAMkADA1M-CJKtzmnlcqVgqI="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages('AAMkADA1M-zAAA=')/attachments('AAMkADA1M-CJKtzmnlcqVgqI=')/?$expand=microsoft.graph.itemattachment/item
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="291aa-194">C#</span><span class="sxs-lookup"><span data-stu-id="291aa-194">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-and-expand-item-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="291aa-195">Javascript</span><span class="sxs-lookup"><span data-stu-id="291aa-195">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-and-expand-item-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="291aa-196">Цель — C</span><span class="sxs-lookup"><span data-stu-id="291aa-196">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-and-expand-item-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="291aa-197">Java</span><span class="sxs-lookup"><span data-stu-id="291aa-197">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-and-expand-item-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="291aa-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="291aa-198">Response</span></span>
<span data-ttu-id="291aa-p112">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="291aa-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "importance":"normal",
    "conversationId":"AAQkADA1MzMyOGI4LTlkZDctNDkzYy05M2RiLTdiN2E1NDE3MTRkOQAQAMG_NSCMBqdKrLa2EmR-lO0=",
    "conversationIndex":"AQHTAbcSwb41IIwGp0qstrYSZH+U7Q==",
    "isDeliveryReceiptRequested":false,
    "isReadReceiptRequested":false,
    "isRead":false,
    "isDraft":false,
    "webLink":"https://outlook.office365.com/owa/?ItemID=AAMkADA1M3MTRkOQAAAA%3D%3D&exvsurl=1&viewmodel=ReadMessageItem",
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

### <a name="example-4-get-the-properties-of-a-reference-attachment"></a><span data-ttu-id="291aa-202">Пример 4: получение свойств вложения для ссылки</span><span class="sxs-lookup"><span data-stu-id="291aa-202">Example 4: Get the properties of a reference attachment</span></span>

#### <a name="request"></a><span data-ttu-id="291aa-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="291aa-203">Request</span></span>

<span data-ttu-id="291aa-204">Ниже приведен пример запроса на получение вложенной ссылки из данных, касающихся события.</span><span class="sxs-lookup"><span data-stu-id="291aa-204">Here is an example of the request to get a reference attachment on an event.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="291aa-205">HTTP</span><span class="sxs-lookup"><span data-stu-id="291aa-205">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_reference_attachment",
  "sampleKeys": ["AAMkAGE1M88AADUv0uAAAG=","AAMkAGE1Mg72tgf7hJp0PICVGCc0g="]
}-->

```http
GET https://graph.microsoft.com/beta/me/events/AAMkAGE1M88AADUv0uAAAG=/attachments/AAMkAGE1Mg72tgf7hJp0PICVGCc0g=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="291aa-206">C#</span><span class="sxs-lookup"><span data-stu-id="291aa-206">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-reference-attachment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="291aa-207">Javascript</span><span class="sxs-lookup"><span data-stu-id="291aa-207">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-reference-attachment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="291aa-208">Цель — C</span><span class="sxs-lookup"><span data-stu-id="291aa-208">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-reference-attachment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="291aa-209">Java</span><span class="sxs-lookup"><span data-stu-id="291aa-209">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-reference-attachment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="291aa-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="291aa-210">Response</span></span>
<span data-ttu-id="291aa-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="291aa-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


### <a name="example-5-get-the-raw-contents-of-a-file-attachment-on-a-message"></a><span data-ttu-id="291aa-214">Пример 5: получение необработанного содержимого вложенного файла сообщения</span><span class="sxs-lookup"><span data-stu-id="291aa-214">Example 5: Get the raw contents of a file attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="291aa-215">Запрос</span><span class="sxs-lookup"><span data-stu-id="291aa-215">Request</span></span>

<span data-ttu-id="291aa-216">Ниже приведен пример запроса на получение необработанного содержимого файла Word, вложенного в сообщение.</span><span class="sxs-lookup"><span data-stu-id="291aa-216">Here is an example of the request to get the raw contents of a Word file that has been attached to a message.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_value_file_attachment",
  "sampleKeys": ["AAMkAGUzY5QKjAAA=","AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGUzY5QKjAAA=/attachments/AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=/$value
```

#### <a name="response"></a><span data-ttu-id="291aa-217">Ответ</span><span class="sxs-lookup"><span data-stu-id="291aa-217">Response</span></span>
<span data-ttu-id="291aa-218">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="291aa-218">Here is an example of the response.</span></span> <span data-ttu-id="291aa-219">Текст фактического ответа содержит необработанные байты вложенного файла, которые кратко указаны ниже.</span><span class="sxs-lookup"><span data-stu-id="291aa-219">The actual response body includes the raw bytes of the file attachment, which are abbreviated here for brevity.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_value_file_attachment",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK

{Raw bytes of the file}
```


### <a name="example-6-get-the-mime-raw-contents-of-a-contact-attachment-on-a-message"></a><span data-ttu-id="291aa-220">Пример 6: получение необработанного MIME содержимого контакта из вложения в сообщении</span><span class="sxs-lookup"><span data-stu-id="291aa-220">Example 6: Get the MIME raw contents of a contact attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="291aa-221">Запрос</span><span class="sxs-lookup"><span data-stu-id="291aa-221">Request</span></span>

<span data-ttu-id="291aa-222">Ниже приведен пример запроса на получение необработанного содержимого элемента контакта, вложенного в сообщение.</span><span class="sxs-lookup"><span data-stu-id="291aa-222">Here is an example of the request to get the raw contents of a contact item that has been attached to a message.</span></span> 
<!-- {
  "blockType": "ignored",
  "name": "get_value_contact_attachment",
  "sampleKeys": ["AAMkADI5MAAGjk2PxAAA=","AAMkADI5MAAGjk2PxAAABEgAQACEJqrbJZBNIlr3pGFvd9K8="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkADI5MAAGjk2PxAAA=/attachments/AAMkADI5MAAGjk2PxAAABEgAQACEJqrbJZBNIlr3pGFvd9K8=/$value
```

#### <a name="response"></a><span data-ttu-id="291aa-223">Ответ</span><span class="sxs-lookup"><span data-stu-id="291aa-223">Response</span></span>
<span data-ttu-id="291aa-224">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="291aa-224">Here is an example of the response.</span></span> 

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


### <a name="example-7-get-the-mime-raw-contents-of-an-event-attachment-on-a-message"></a><span data-ttu-id="291aa-225">Пример 7: получение необработанного MIME содержимого вложения события в сообщении</span><span class="sxs-lookup"><span data-stu-id="291aa-225">Example 7: Get the MIME raw contents of an event attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="291aa-226">Запрос</span><span class="sxs-lookup"><span data-stu-id="291aa-226">Request</span></span>

<span data-ttu-id="291aa-227">Ниже приведен пример запроса на получение необработанного содержимого события, вложенного в сообщение.</span><span class="sxs-lookup"><span data-stu-id="291aa-227">Here is an example of the request to get the raw contents of an event that has been attached to a message.</span></span> 
<!-- {
  "blockType": "ignored",
  "name": "get_value_event_attachment",
  "sampleKeys": ["AAMkADVIOAAA=","AAMkADVIOAAABEgAQACvkutl6c4FMifPyS6NvXsM="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkADVIOAAA=/attachments/AAMkADVIOAAABEgAQACvkutl6c4FMifPyS6NvXsM=/$value
```

#### <a name="response"></a><span data-ttu-id="291aa-228">Отклик</span><span class="sxs-lookup"><span data-stu-id="291aa-228">Response</span></span>
<span data-ttu-id="291aa-229">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="291aa-229">Here is an example of the response.</span></span> 

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


### <a name="example-8-get-the-mime-raw-contents-of-a-meeting-invitation-item-attachment-on-a-message"></a><span data-ttu-id="291aa-230">Пример 8: получение необработанного MIME содержимого приглашения на собрание, вложенного в сообщение</span><span class="sxs-lookup"><span data-stu-id="291aa-230">Example 8: Get the MIME raw contents of a meeting invitation item attachment on a message</span></span>

#### <a name="request"></a><span data-ttu-id="291aa-231">Запрос</span><span class="sxs-lookup"><span data-stu-id="291aa-231">Request</span></span>

<span data-ttu-id="291aa-232">Ниже приведен пример запроса на получение необработанного содержимого приглашения на собрание (из типа [eventMessage](../resources/eventmessage.md) ), которое было прикреплено к сообщению.</span><span class="sxs-lookup"><span data-stu-id="291aa-232">Here is an example of the request to get the raw contents of a meeting invitation (of the [eventMessage](../resources/eventmessage.md) type) that has been attached to a message.</span></span> <span data-ttu-id="291aa-233">Объект **eventMessage** основан на типе **сообщения** .</span><span class="sxs-lookup"><span data-stu-id="291aa-233">The **eventMessage** entity is based on the **message** type.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_value_message_attachment",
  "sampleKeys": ["AAMkAGUzY5QKiAAA=","AAMkAGUzY5QKiAAABEgAQAK8ktgiIO19OqkvUZAqLmyQ="]
}-->

```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGUzY5QKiAAA=/attachments/AAMkAGUzY5QKiAAABEgAQAK8ktgiIO19OqkvUZAqLmyQ=/$value
```

#### <a name="response"></a><span data-ttu-id="291aa-234">Отклик</span><span class="sxs-lookup"><span data-stu-id="291aa-234">Response</span></span>
<span data-ttu-id="291aa-235">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="291aa-235">Here is an example of the response.</span></span> 

<span data-ttu-id="291aa-236">Текст отклика включает вложение **eventMessage** в формате MIME.</span><span class="sxs-lookup"><span data-stu-id="291aa-236">The response body includes the **eventMessage** attachment in MIME format.</span></span> <span data-ttu-id="291aa-237">Текст **eventMessage** усекается для краткости.</span><span class="sxs-lookup"><span data-stu-id="291aa-237">The body of the  **eventMessage** is truncated for brevity.</span></span> <span data-ttu-id="291aa-238">Весь текст сообщения возвращается при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="291aa-238">The full message body is returned from an actual call.</span></span>

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
