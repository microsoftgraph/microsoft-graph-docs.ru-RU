---
title: Добавление вложения
description: С помощью этого API можно добавить вложение к записи. Так как
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 16b054b093a90f6017c073c77b5656ea56c8bbc3
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275189"
---
# <a name="add-attachment"></a><span data-ttu-id="74b51-104">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="74b51-104">Add attachment</span></span>

<span data-ttu-id="74b51-p102">С помощью этого API можно добавить [вложение](../resources/attachment.md) к записи. Так как в настоящее время максимальный общий размер каждого запроса REST составляет 4 МБ, размер добавляемого вложения не может превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="74b51-p102">Use this API to add an [attachment](../resources/attachment.md) to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

<span data-ttu-id="74b51-107">Допустимые типы вложений:</span><span class="sxs-lookup"><span data-stu-id="74b51-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="74b51-108">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="74b51-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="74b51-109">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="74b51-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="74b51-110">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="74b51-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="74b51-111">Все эти типы ресурсов вложений являются производными от ресурса [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="74b51-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="74b51-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="74b51-112">Permissions</span></span>
<span data-ttu-id="74b51-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74b51-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74b51-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74b51-115">Permission type</span></span>      | <span data-ttu-id="74b51-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="74b51-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74b51-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74b51-117">Delegated (work or school account)</span></span> | <span data-ttu-id="74b51-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74b51-118">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="74b51-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74b51-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74b51-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74b51-120">Not supported.</span></span>    |
|<span data-ttu-id="74b51-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74b51-121">Application</span></span> | <span data-ttu-id="74b51-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74b51-122">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="74b51-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74b51-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="74b51-124">Вложения для [записи](../resources/post.md) в [цепочке](../resources/conversationthread.md) [беседы](../resources/conversation.md) в группе.</span><span class="sxs-lookup"><span data-stu-id="74b51-124">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
POST /groups/{id}/threads/{id}/posts/{id}/attachments
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="74b51-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="74b51-125">Request headers</span></span>
| <span data-ttu-id="74b51-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="74b51-126">Header</span></span>       | <span data-ttu-id="74b51-127">Значение</span><span class="sxs-lookup"><span data-stu-id="74b51-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="74b51-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="74b51-128">Authorization</span></span>  | <span data-ttu-id="74b51-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74b51-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="74b51-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="74b51-131">Request body</span></span>
<span data-ttu-id="74b51-132">Предоставьте в тексте запроса описание объекта [Attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74b51-132">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="74b51-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="74b51-133">Response</span></span>

<span data-ttu-id="74b51-134">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Attachment](../resources/attachment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="74b51-134">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="74b51-135">Пример (вложенный файл)</span><span class="sxs-lookup"><span data-stu-id="74b51-135">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="74b51-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="74b51-136">Request</span></span>
<span data-ttu-id="74b51-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="74b51-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "name-value",
  "contentBytes": "base64-contentBytes-value"
}
```

<span data-ttu-id="74b51-138">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74b51-138">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="74b51-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="74b51-139">Response</span></span>
<span data-ttu-id="74b51-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="74b51-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="74b51-143">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="74b51-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="74b51-144">C#</span><span class="sxs-lookup"><span data-stu-id="74b51-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_post-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="74b51-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="74b51-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_post-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="74b51-146">Цель — C</span><span class="sxs-lookup"><span data-stu-id="74b51-146">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_post-Objective-C-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="example-item-attachment"></a><span data-ttu-id="74b51-147">Пример (вложенный элемент)</span><span class="sxs-lookup"><span data-stu-id="74b51-147">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="74b51-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="74b51-148">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "name": "name-value",
  "item": { }
}
```

##### <a name="response"></a><span data-ttu-id="74b51-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="74b51-149">Response</span></span>
<span data-ttu-id="74b51-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="74b51-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/post-post-attachments.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/post-post-attachments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/post-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/post-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
