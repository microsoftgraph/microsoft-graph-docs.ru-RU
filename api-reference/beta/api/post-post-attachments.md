---
title: Добавление вложения
description: С помощью этого API можно добавить вложение к записи. Так как
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: ffcbc9984774f0e0e59fc2953ddb86d3cc3ce195
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33595020"
---
# <a name="add-attachment"></a><span data-ttu-id="483a7-104">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="483a7-104">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="483a7-p102">С помощью этого API можно добавить [вложение](../resources/attachment.md) к записи. Так как в настоящее время максимальный общий размер каждого запроса REST составляет 4 МБ, размер добавляемого вложения не может превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="483a7-p102">Use this API to add an [attachment](../resources/attachment.md) to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

<span data-ttu-id="483a7-107">Допустимые типы вложений:</span><span class="sxs-lookup"><span data-stu-id="483a7-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="483a7-108">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="483a7-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="483a7-109">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="483a7-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="483a7-110">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="483a7-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="483a7-111">Все эти типы ресурсов вложений являются производными от ресурса [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="483a7-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="483a7-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="483a7-112">Permissions</span></span>
<span data-ttu-id="483a7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="483a7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="483a7-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="483a7-115">Permission type</span></span>      | <span data-ttu-id="483a7-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="483a7-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="483a7-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="483a7-117">Delegated (work or school account)</span></span> | <span data-ttu-id="483a7-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="483a7-118">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="483a7-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="483a7-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="483a7-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="483a7-120">Not supported.</span></span>    |
|<span data-ttu-id="483a7-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="483a7-121">Application</span></span> | <span data-ttu-id="483a7-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="483a7-122">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="483a7-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="483a7-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="483a7-124">Вложения для [записи](../resources/post.md) в [цепочке](../resources/conversationthread.md) [беседы](../resources/conversation.md) в группе.</span><span class="sxs-lookup"><span data-stu-id="483a7-124">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
POST /groups/{id}/threads/{id}/posts/{id}/attachments
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="483a7-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="483a7-125">Request headers</span></span>
| <span data-ttu-id="483a7-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="483a7-126">Header</span></span>       | <span data-ttu-id="483a7-127">Значение</span><span class="sxs-lookup"><span data-stu-id="483a7-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="483a7-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="483a7-128">Authorization</span></span>  | <span data-ttu-id="483a7-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="483a7-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="483a7-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="483a7-131">Request body</span></span>
<span data-ttu-id="483a7-132">Предоставьте в тексте запроса описание объекта [Attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="483a7-132">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="483a7-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="483a7-133">Response</span></span>

<span data-ttu-id="483a7-134">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Attachment](../resources/attachment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="483a7-134">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="483a7-135">Пример (вложенный файл)</span><span class="sxs-lookup"><span data-stu-id="483a7-135">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="483a7-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="483a7-136">Request</span></span>
<span data-ttu-id="483a7-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="483a7-137">Here is an example of the request.</span></span>
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

<span data-ttu-id="483a7-138">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="483a7-138">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="483a7-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="483a7-139">Response</span></span>
<span data-ttu-id="483a7-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="483a7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="483a7-143">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="483a7-143">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="483a7-144">Язык</span><span class="sxs-lookup"><span data-stu-id="483a7-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_post-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="example-item-attachment"></a><span data-ttu-id="483a7-145">Пример (вложенный элемент)</span><span class="sxs-lookup"><span data-stu-id="483a7-145">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="483a7-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="483a7-146">Request</span></span>
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

##### <a name="response"></a><span data-ttu-id="483a7-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="483a7-147">Response</span></span>
<span data-ttu-id="483a7-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="483a7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="483a7-151">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="483a7-151">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="483a7-152">Язык</span><span class="sxs-lookup"><span data-stu-id="483a7-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_item_attachment_from_post-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


## <a name="example-reference-attachment"></a><span data-ttu-id="483a7-153">Пример (вложенная ссылка)</span><span class="sxs-lookup"><span data-stu-id="483a7-153">Example (reference attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="483a7-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="483a7-154">Request</span></span>
<span data-ttu-id="483a7-155">Ниже приведен пример запроса, который добавляет к существующей записи вложение ссылки.</span><span class="sxs-lookup"><span data-stu-id="483a7-155">Here is an example of a request that adds a reference attachment to an existing post.</span></span>
<span data-ttu-id="483a7-156">Вложение указывает на папку в OneDrive.</span><span class="sxs-lookup"><span data-stu-id="483a7-156">The attachment points to a folder on OneDrive.</span></span>
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

##### <a name="response"></a><span data-ttu-id="483a7-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="483a7-157">Response</span></span>
<span data-ttu-id="483a7-158">Ниже приведен пример полного ответа.</span><span class="sxs-lookup"><span data-stu-id="483a7-158">Here is an example of a full response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="483a7-159">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="483a7-159">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="483a7-160">Язык</span><span class="sxs-lookup"><span data-stu-id="483a7-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_reference_attachment_from_post-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/post-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/post-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/post-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
