---
title: Добавление вложения
description: С помощью этого API можно создать объект Attachment.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: c1b61c1a0f2cfc54760f6bcf6f2ad6781cabd8ae
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275917"
---
# <a name="add-attachment"></a><span data-ttu-id="0842f-103">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="0842f-103">Add attachment</span></span>

<span data-ttu-id="0842f-104">С помощью этого API можно создать объект Attachment.</span><span class="sxs-lookup"><span data-stu-id="0842f-104">Use this API to create a new Attachment.</span></span>

<span data-ttu-id="0842f-105">Допустимые типы вложений:</span><span class="sxs-lookup"><span data-stu-id="0842f-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="0842f-106">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="0842f-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="0842f-107">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="0842f-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="0842f-108">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="0842f-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="0842f-109">Все эти типы ресурсов вложений являются производными от ресурса [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="0842f-109">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="0842f-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0842f-110">Permissions</span></span>
<span data-ttu-id="0842f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0842f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0842f-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0842f-113">Permission type</span></span>      | <span data-ttu-id="0842f-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0842f-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0842f-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0842f-115">Delegated (work or school account)</span></span> | <span data-ttu-id="0842f-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0842f-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0842f-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0842f-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0842f-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0842f-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0842f-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0842f-119">Application</span></span> | <span data-ttu-id="0842f-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0842f-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0842f-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0842f-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="0842f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0842f-122">Request headers</span></span>
| <span data-ttu-id="0842f-123">Имя</span><span class="sxs-lookup"><span data-stu-id="0842f-123">Name</span></span>       | <span data-ttu-id="0842f-124">Тип</span><span class="sxs-lookup"><span data-stu-id="0842f-124">Type</span></span> | <span data-ttu-id="0842f-125">Описание</span><span class="sxs-lookup"><span data-stu-id="0842f-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0842f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="0842f-126">Authorization</span></span>  | <span data-ttu-id="0842f-127">string</span><span class="sxs-lookup"><span data-stu-id="0842f-127">string</span></span>  | <span data-ttu-id="0842f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0842f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0842f-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0842f-130">Content-Type</span></span> | <span data-ttu-id="0842f-131">string</span><span class="sxs-lookup"><span data-stu-id="0842f-131">string</span></span>  | <span data-ttu-id="0842f-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0842f-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0842f-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0842f-134">Request body</span></span>
<span data-ttu-id="0842f-135">Предоставьте в тексте запроса описание объекта [Attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0842f-135">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0842f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0842f-136">Response</span></span>

<span data-ttu-id="0842f-137">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0842f-137">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="0842f-138">Пример (вложенный файл)</span><span class="sxs-lookup"><span data-stu-id="0842f-138">Example (File attachment)</span></span>
##### <a name="request"></a><span data-ttu-id="0842f-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="0842f-139">Request</span></span>
<span data-ttu-id="0842f-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0842f-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "microsoft.graph.fileAttachment",
  "name": "name-value",
  "contentType": "contentType-value",
  "isInline": false,
  "contentLocation": "contentLocation-value",
  "contentBytes": "base64-contentBytes-value"
}
```

<span data-ttu-id="0842f-141">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0842f-141">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="0842f-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="0842f-142">Response</span></span>
<span data-ttu-id="0842f-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0842f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 201 Created
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0842f-146">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="0842f-146">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0842f-147">C#</span><span class="sxs-lookup"><span data-stu-id="0842f-147">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_eventmessage-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0842f-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="0842f-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_eventmessage-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0842f-149">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0842f-149">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_file_attachment_from_eventmessage-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="example-item-attachment"></a><span data-ttu-id="0842f-150">Пример (вложенный элемент)</span><span class="sxs-lookup"><span data-stu-id="0842f-150">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="0842f-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="0842f-151">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/attachments
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#Microsoft.OutlookServices.ItemAttachment",
  "name": "name-value",
  "item": "message or event entity"
}
```

##### <a name="response"></a><span data-ttu-id="0842f-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="0842f-152">Response</span></span>
<span data-ttu-id="0842f-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0842f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 201 Created
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0842f-156">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="0842f-156">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0842f-157">C#</span><span class="sxs-lookup"><span data-stu-id="0842f-157">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_item_attachment_from_eventmessage-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0842f-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="0842f-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_item_attachment_from_eventmessage-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0842f-159">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0842f-159">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_item_attachment_from_eventmessage-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/eventmessage-post-attachments.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/eventmessage-post-attachments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/eventmessage-post-attachments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
