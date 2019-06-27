---
title: Добавление вложения
description: С помощью этого API можно добавить вложение к записи. Так как
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: f637b5f6f5d976ac5c4dedac4c45649cb3de33b6
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268203"
---
# <a name="add-attachment"></a><span data-ttu-id="d4f6c-104">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="d4f6c-104">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4f6c-p102">С помощью этого API можно добавить [вложение](../resources/attachment.md) к записи. Так как в настоящее время максимальный общий размер каждого запроса REST составляет 4 МБ, размер добавляемого вложения не может превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="d4f6c-p102">Use this API to add an [attachment](../resources/attachment.md) to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

<span data-ttu-id="d4f6c-107">Допустимые типы вложений:</span><span class="sxs-lookup"><span data-stu-id="d4f6c-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="d4f6c-108">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="d4f6c-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="d4f6c-109">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="d4f6c-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="d4f6c-110">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="d4f6c-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="d4f6c-111">Все эти типы ресурсов вложений являются производными от ресурса [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="d4f6c-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="d4f6c-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d4f6c-112">Permissions</span></span>
<span data-ttu-id="d4f6c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4f6c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4f6c-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4f6c-115">Permission type</span></span>      | <span data-ttu-id="d4f6c-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4f6c-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4f6c-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4f6c-117">Delegated (work or school account)</span></span> | <span data-ttu-id="d4f6c-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4f6c-118">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d4f6c-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4f6c-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4f6c-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d4f6c-120">Not supported.</span></span>    |
|<span data-ttu-id="d4f6c-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4f6c-121">Application</span></span> | <span data-ttu-id="d4f6c-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4f6c-122">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4f6c-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4f6c-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="d4f6c-124">Вложения для [записи](../resources/post.md) в [цепочке](../resources/conversationthread.md) [беседы](../resources/conversation.md) в группе.</span><span class="sxs-lookup"><span data-stu-id="d4f6c-124">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
POST /groups/{id}/threads/{id}/posts/{id}/attachments
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="d4f6c-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4f6c-125">Request headers</span></span>
| <span data-ttu-id="d4f6c-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d4f6c-126">Header</span></span>       | <span data-ttu-id="d4f6c-127">Значение</span><span class="sxs-lookup"><span data-stu-id="d4f6c-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d4f6c-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d4f6c-128">Authorization</span></span>  | <span data-ttu-id="d4f6c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4f6c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d4f6c-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d4f6c-131">Request body</span></span>
<span data-ttu-id="d4f6c-132">Предоставьте в тексте запроса описание объекта [Attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4f6c-132">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d4f6c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4f6c-133">Response</span></span>

<span data-ttu-id="d4f6c-134">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Attachment](../resources/attachment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d4f6c-134">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="d4f6c-135">Пример (вложенный файл)</span><span class="sxs-lookup"><span data-stu-id="d4f6c-135">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="d4f6c-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4f6c-136">Request</span></span>
<span data-ttu-id="d4f6c-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4f6c-137">Here is an example of the request.</span></span>
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

<span data-ttu-id="d4f6c-138">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4f6c-138">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="d4f6c-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4f6c-139">Response</span></span>
<span data-ttu-id="d4f6c-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d4f6c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d4f6c-143">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="d4f6c-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d4f6c-144">C#</span><span class="sxs-lookup"><span data-stu-id="d4f6c-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_post-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d4f6c-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="d4f6c-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_post-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d4f6c-146">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d4f6c-146">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_post-Objective-C-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="example-item-attachment"></a><span data-ttu-id="d4f6c-147">Пример (вложенный элемент)</span><span class="sxs-lookup"><span data-stu-id="d4f6c-147">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="d4f6c-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4f6c-148">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_post"
}-->
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

##### <a name="response"></a><span data-ttu-id="d4f6c-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4f6c-149">Response</span></span>
<span data-ttu-id="d4f6c-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d4f6c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-reference-attachment"></a><span data-ttu-id="d4f6c-153">Пример (вложенная ссылка)</span><span class="sxs-lookup"><span data-stu-id="d4f6c-153">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="d4f6c-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4f6c-154">Request</span></span>
<span data-ttu-id="d4f6c-155">Ниже приведен пример запроса, который добавляет к существующей записи вложение ссылки.</span><span class="sxs-lookup"><span data-stu-id="d4f6c-155">Here is an example of a request that adds a reference attachment to an existing post.</span></span>
<span data-ttu-id="d4f6c-156">Вложение указывает на папку в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="d4f6c-156">The attachment points to a folder on OneDrive.</span></span>
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

##### <a name="response"></a><span data-ttu-id="d4f6c-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4f6c-157">Response</span></span>
<span data-ttu-id="d4f6c-158">Ниже приведен пример полного ответа.</span><span class="sxs-lookup"><span data-stu-id="d4f6c-158">Here is an example of a full response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d4f6c-159">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="d4f6c-159">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d4f6c-160">C#</span><span class="sxs-lookup"><span data-stu-id="d4f6c-160">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_reference_attachment_from_post-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d4f6c-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="d4f6c-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_reference_attachment_from_post-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d4f6c-162">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d4f6c-162">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_reference_attachment_from_post-Objective-C-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/post-post-attachments.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/post-post-attachments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/post-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/post-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/post-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
