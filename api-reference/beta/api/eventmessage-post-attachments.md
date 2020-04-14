---
title: Добавление вложения
description: С помощью этого API можно создать объект Attachment.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e2d389df4ffe2e1abc2b9e9749f4fc626f5ed654
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43364165"
---
# <a name="add-attachment"></a><span data-ttu-id="0d666-103">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="0d666-103">Add attachment</span></span>

<span data-ttu-id="0d666-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d666-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d666-105">С помощью этого API можно создать объект Attachment.</span><span class="sxs-lookup"><span data-stu-id="0d666-105">Use this API to create a new Attachment.</span></span>

<span data-ttu-id="0d666-106">Допустимые типы вложений:</span><span class="sxs-lookup"><span data-stu-id="0d666-106">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="0d666-107">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="0d666-107">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="0d666-108">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="0d666-108">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="0d666-109">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="0d666-109">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="0d666-110">Все эти типы ресурсов вложений являются производными от ресурса [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="0d666-110">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="0d666-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0d666-111">Permissions</span></span>
<span data-ttu-id="0d666-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d666-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d666-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d666-114">Permission type</span></span>      | <span data-ttu-id="0d666-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d666-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d666-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d666-116">Delegated (work or school account)</span></span> | <span data-ttu-id="0d666-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d666-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0d666-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d666-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d666-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d666-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0d666-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d666-120">Application</span></span> | <span data-ttu-id="0d666-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d666-121">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d666-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d666-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments
POST /users/{id|userPrincipalName}/messages/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="0d666-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d666-123">Request headers</span></span>
| <span data-ttu-id="0d666-124">Имя</span><span class="sxs-lookup"><span data-stu-id="0d666-124">Name</span></span>       | <span data-ttu-id="0d666-125">Тип</span><span class="sxs-lookup"><span data-stu-id="0d666-125">Type</span></span> | <span data-ttu-id="0d666-126">Описание</span><span class="sxs-lookup"><span data-stu-id="0d666-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0d666-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d666-127">Authorization</span></span>  | <span data-ttu-id="0d666-128">string</span><span class="sxs-lookup"><span data-stu-id="0d666-128">string</span></span>  | <span data-ttu-id="0d666-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d666-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0d666-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0d666-131">Content-Type</span></span> | <span data-ttu-id="0d666-132">string</span><span class="sxs-lookup"><span data-stu-id="0d666-132">string</span></span>  | <span data-ttu-id="0d666-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d666-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d666-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0d666-135">Request body</span></span>
<span data-ttu-id="0d666-136">Предоставьте в тексте запроса описание объекта [Attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d666-136">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0d666-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d666-137">Response</span></span>

<span data-ttu-id="0d666-138">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Attachment](../resources/attachment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0d666-138">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="0d666-139">Пример (вложенный файл)</span><span class="sxs-lookup"><span data-stu-id="0d666-139">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="0d666-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d666-140">Request</span></span>
<span data-ttu-id="0d666-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d666-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0d666-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d666-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0d666-143">C#</span><span class="sxs-lookup"><span data-stu-id="0d666-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d666-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d666-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d666-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d666-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0d666-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d666-146">Response</span></span>
<span data-ttu-id="0d666-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0d666-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
```


## <a name="example-item-attachment"></a><span data-ttu-id="0d666-150">Пример (вложенный элемент)</span><span class="sxs-lookup"><span data-stu-id="0d666-150">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="0d666-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d666-151">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0d666-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d666-152">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0d666-153">C#</span><span class="sxs-lookup"><span data-stu-id="0d666-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-item-attachment-from-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d666-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d666-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-item-attachment-from-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d666-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d666-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-item-attachment-from-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0d666-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d666-156">Response</span></span>
<span data-ttu-id="0d666-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0d666-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
