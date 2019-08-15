---
title: Добавление вложения
description: С помощью этого API можно создать объект Attachment.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a6a3aebc1873e2a7b79948a130c783f68f466401
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419820"
---
# <a name="add-attachment"></a><span data-ttu-id="b0f1d-103">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="b0f1d-103">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0f1d-104">С помощью этого API можно создать объект Attachment.</span><span class="sxs-lookup"><span data-stu-id="b0f1d-104">Use this API to create a new Attachment.</span></span>

<span data-ttu-id="b0f1d-105">Допустимые типы вложений:</span><span class="sxs-lookup"><span data-stu-id="b0f1d-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="b0f1d-106">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="b0f1d-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="b0f1d-107">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="b0f1d-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="b0f1d-108">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="b0f1d-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="b0f1d-109">Все эти типы ресурсов вложений являются производными от ресурса [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="b0f1d-109">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b0f1d-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b0f1d-110">Permissions</span></span>
<span data-ttu-id="b0f1d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0f1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0f1d-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0f1d-113">Permission type</span></span>      | <span data-ttu-id="b0f1d-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0f1d-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0f1d-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0f1d-115">Delegated (work or school account)</span></span> | <span data-ttu-id="b0f1d-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0f1d-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b0f1d-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0f1d-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0f1d-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0f1d-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b0f1d-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0f1d-119">Application</span></span> | <span data-ttu-id="b0f1d-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b0f1d-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0f1d-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0f1d-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments
POST /users/{id|userPrincipalName}/messages/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="b0f1d-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0f1d-122">Request headers</span></span>
| <span data-ttu-id="b0f1d-123">Имя</span><span class="sxs-lookup"><span data-stu-id="b0f1d-123">Name</span></span>       | <span data-ttu-id="b0f1d-124">Тип</span><span class="sxs-lookup"><span data-stu-id="b0f1d-124">Type</span></span> | <span data-ttu-id="b0f1d-125">Описание</span><span class="sxs-lookup"><span data-stu-id="b0f1d-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b0f1d-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0f1d-126">Authorization</span></span>  | <span data-ttu-id="b0f1d-127">string</span><span class="sxs-lookup"><span data-stu-id="b0f1d-127">string</span></span>  | <span data-ttu-id="b0f1d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0f1d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b0f1d-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b0f1d-130">Content-Type</span></span> | <span data-ttu-id="b0f1d-131">string</span><span class="sxs-lookup"><span data-stu-id="b0f1d-131">string</span></span>  | <span data-ttu-id="b0f1d-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0f1d-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0f1d-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b0f1d-134">Request body</span></span>
<span data-ttu-id="b0f1d-135">Предоставьте в тексте запроса описание объекта [Attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0f1d-135">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b0f1d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0f1d-136">Response</span></span>

<span data-ttu-id="b0f1d-137">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Attachment](../resources/attachment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b0f1d-137">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="b0f1d-138">Пример (вложенный файл)</span><span class="sxs-lookup"><span data-stu-id="b0f1d-138">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="b0f1d-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0f1d-139">Request</span></span>
<span data-ttu-id="b0f1d-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0f1d-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b0f1d-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0f1d-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/{id}/attachments
Content-type: application/json

{
  "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
  "name": "name-value",
  "contentType": "contentType-value",
  "isInline": false,
  "contentLocation": "contentLocation-value",
  "contentBytes": "contentBytes-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b0f1d-142">C#</span><span class="sxs-lookup"><span data-stu-id="b0f1d-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b0f1d-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0f1d-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b0f1d-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b0f1d-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b0f1d-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0f1d-145">Response</span></span>
<span data-ttu-id="b0f1d-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b0f1d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
```


## <a name="example-item-attachment"></a><span data-ttu-id="b0f1d-149">Пример (вложенный элемент)</span><span class="sxs-lookup"><span data-stu-id="b0f1d-149">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="b0f1d-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0f1d-150">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b0f1d-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0f1d-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/beta/me/events/{id}/attachments
Content-type: application/json

{
  "@odata.type": "#Microsoft.OutlookServices.ItemAttachment",
  "name": "name-value",
  "item": "message or event entity"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b0f1d-152">C#</span><span class="sxs-lookup"><span data-stu-id="b0f1d-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-item-attachment-from-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b0f1d-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0f1d-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-item-attachment-from-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b0f1d-154">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b0f1d-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-item-attachment-from-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b0f1d-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="b0f1d-155">Response</span></span>
<span data-ttu-id="b0f1d-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b0f1d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
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
