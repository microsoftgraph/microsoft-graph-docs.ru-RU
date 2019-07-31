---
title: Добавление вложения
description: С помощью этого API можно добавить вложение к записи. Так как
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2b54818d602d9226303c96cb002cf72e453cae13
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35983420"
---
# <a name="add-attachment"></a><span data-ttu-id="2ee36-104">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="2ee36-104">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ee36-p102">С помощью этого API можно добавить [вложение](../resources/attachment.md) к записи. Так как в настоящее время максимальный общий размер каждого запроса REST составляет 4 МБ, размер добавляемого вложения не может превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="2ee36-p102">Use this API to add an [attachment](../resources/attachment.md) to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

<span data-ttu-id="2ee36-107">Допустимые типы вложений:</span><span class="sxs-lookup"><span data-stu-id="2ee36-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="2ee36-108">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="2ee36-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="2ee36-109">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="2ee36-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="2ee36-110">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="2ee36-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="2ee36-111">Все эти типы ресурсов вложений являются производными от ресурса [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="2ee36-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="2ee36-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ee36-112">Permissions</span></span>
<span data-ttu-id="2ee36-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ee36-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ee36-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ee36-115">Permission type</span></span>      | <span data-ttu-id="2ee36-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ee36-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ee36-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ee36-117">Delegated (work or school account)</span></span> | <span data-ttu-id="2ee36-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ee36-118">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2ee36-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ee36-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ee36-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ee36-120">Not supported.</span></span>    |
|<span data-ttu-id="2ee36-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ee36-121">Application</span></span> | <span data-ttu-id="2ee36-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ee36-122">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ee36-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ee36-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="2ee36-124">Вложения для [записи](../resources/post.md) в [цепочке](../resources/conversationthread.md) [беседы](../resources/conversation.md) в группе.</span><span class="sxs-lookup"><span data-stu-id="2ee36-124">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
POST /groups/{id}/threads/{id}/posts/{id}/attachments
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="2ee36-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ee36-125">Request headers</span></span>
| <span data-ttu-id="2ee36-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2ee36-126">Header</span></span>       | <span data-ttu-id="2ee36-127">Значение</span><span class="sxs-lookup"><span data-stu-id="2ee36-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2ee36-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ee36-128">Authorization</span></span>  | <span data-ttu-id="2ee36-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ee36-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2ee36-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2ee36-131">Request body</span></span>
<span data-ttu-id="2ee36-132">Предоставьте в тексте запроса описание объекта [Attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ee36-132">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2ee36-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ee36-133">Response</span></span>

<span data-ttu-id="2ee36-134">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Attachment](../resources/attachment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2ee36-134">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="2ee36-135">Пример (вложенный файл)</span><span class="sxs-lookup"><span data-stu-id="2ee36-135">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="2ee36-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ee36-136">Request</span></span>
<span data-ttu-id="2ee36-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ee36-137">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2ee36-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ee36-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "name-value",
  "contentBytes": "contentBytes-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2ee36-139">C#</span><span class="sxs-lookup"><span data-stu-id="2ee36-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2ee36-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="2ee36-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2ee36-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2ee36-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2ee36-142">Java</span><span class="sxs-lookup"><span data-stu-id="2ee36-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-file-attachment-from-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="2ee36-143">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ee36-143">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="2ee36-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ee36-144">Response</span></span>
<span data-ttu-id="2ee36-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2ee36-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "2016-10-19T10:37:00Z",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="2ee36-148">Пример (вложенный элемент)</span><span class="sxs-lookup"><span data-stu-id="2ee36-148">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="2ee36-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ee36-149">Request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "name": "name-value",
  "item": { }
}
```


##### <a name="response"></a><span data-ttu-id="2ee36-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ee36-150">Response</span></span>
<span data-ttu-id="2ee36-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2ee36-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "2016-10-19T10:37:00Z",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```

## <a name="example-reference-attachment"></a><span data-ttu-id="2ee36-154">Пример (вложенная ссылка)</span><span class="sxs-lookup"><span data-stu-id="2ee36-154">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="2ee36-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ee36-155">Request</span></span>
<span data-ttu-id="2ee36-156">Ниже приведен пример запроса, который добавляет к существующей записи вложение ссылки.</span><span class="sxs-lookup"><span data-stu-id="2ee36-156">Here is an example of a request that adds a reference attachment to an existing post.</span></span>
<span data-ttu-id="2ee36-157">Вложение указывает на папку в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="2ee36-157">The attachment points to a folder on OneDrive.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2ee36-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ee36-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_reference_attachment_from_post",
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```
POST https://graph.microsoft.com/beta/groups/c75831bdfad/threads/AAQkAGF97XEKhULw/posts/AAMkAGFcAAA/attachments
Content-type: application/json
Content-length: 319

{ 
    "@odata.type": "#microsoft.graph.referenceAttachment", 
    "name": "Personal pictures", 
    "sourceUrl": "https://contoso.com/personal/mario_contoso_net/Documents/Pics", 
    "providerType": "oneDriveConsumer", 
    "permission": "Edit", 
    "isFolder": "True" 
} 
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2ee36-159">C#</span><span class="sxs-lookup"><span data-stu-id="2ee36-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-reference-attachment-from-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2ee36-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="2ee36-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-reference-attachment-from-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2ee36-161">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2ee36-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-reference-attachment-from-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2ee36-162">Java</span><span class="sxs-lookup"><span data-stu-id="2ee36-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-reference-attachment-from-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2ee36-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ee36-163">Response</span></span>
<span data-ttu-id="2ee36-164">Ниже приведен пример полного ответа.</span><span class="sxs-lookup"><span data-stu-id="2ee36-164">Here is an example of a full response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
} -->
```http
HTTP 201 Created

{
  "@odata.context": "https://graph.microsoft.com/beta/groups/c75831bdfad/threads/AAQkAGF97XEKhULw/posts/AAMkAGFcAAA/attachments/$entity",
  "@odata.type": "#microsoft.graph.referenceAttachment",
  "id": "AAMkAGE1Mg72tgf7hJp0PICVGCc0g=",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
