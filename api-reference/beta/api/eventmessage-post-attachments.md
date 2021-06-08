---
title: Добавление вложения
description: С помощью этого API можно создать объект Attachment.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a047967c1b6d1aaadaef56f22390ac8f1b2a1d31
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787009"
---
# <a name="add-attachment"></a><span data-ttu-id="fdef0-103">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="fdef0-103">Add attachment</span></span>

<span data-ttu-id="fdef0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fdef0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdef0-105">С помощью этого API можно создать объект Attachment.</span><span class="sxs-lookup"><span data-stu-id="fdef0-105">Use this API to create a new Attachment.</span></span>

<span data-ttu-id="fdef0-106">Допустимые типы вложений:</span><span class="sxs-lookup"><span data-stu-id="fdef0-106">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="fdef0-107">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="fdef0-107">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="fdef0-108">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="fdef0-108">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="fdef0-109">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="fdef0-109">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="fdef0-110">Все эти типы ресурсов вложений являются производными от ресурса [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="fdef0-110">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="fdef0-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fdef0-111">Permissions</span></span>
<span data-ttu-id="fdef0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdef0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdef0-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fdef0-114">Permission type</span></span>      | <span data-ttu-id="fdef0-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fdef0-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fdef0-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fdef0-116">Delegated (work or school account)</span></span> | <span data-ttu-id="fdef0-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fdef0-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="fdef0-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fdef0-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fdef0-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fdef0-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="fdef0-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fdef0-120">Application</span></span> | <span data-ttu-id="fdef0-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fdef0-121">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fdef0-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fdef0-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments
POST /users/{id|userPrincipalName}/messages/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="fdef0-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fdef0-123">Request headers</span></span>
| <span data-ttu-id="fdef0-124">Имя</span><span class="sxs-lookup"><span data-stu-id="fdef0-124">Name</span></span>       | <span data-ttu-id="fdef0-125">Тип</span><span class="sxs-lookup"><span data-stu-id="fdef0-125">Type</span></span> | <span data-ttu-id="fdef0-126">Описание</span><span class="sxs-lookup"><span data-stu-id="fdef0-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fdef0-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="fdef0-127">Authorization</span></span>  | <span data-ttu-id="fdef0-128">string</span><span class="sxs-lookup"><span data-stu-id="fdef0-128">string</span></span>  | <span data-ttu-id="fdef0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fdef0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fdef0-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fdef0-131">Content-Type</span></span> | <span data-ttu-id="fdef0-132">string</span><span class="sxs-lookup"><span data-stu-id="fdef0-132">string</span></span>  | <span data-ttu-id="fdef0-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fdef0-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fdef0-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fdef0-135">Request body</span></span>
<span data-ttu-id="fdef0-136">Предоставьте в тексте запроса описание объекта [Attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fdef0-136">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fdef0-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="fdef0-137">Response</span></span>

<span data-ttu-id="fdef0-138">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Attachment](../resources/attachment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fdef0-138">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="fdef0-139">Пример (вложенный файл)</span><span class="sxs-lookup"><span data-stu-id="fdef0-139">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="fdef0-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="fdef0-140">Request</span></span>
<span data-ttu-id="fdef0-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fdef0-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fdef0-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="fdef0-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="fdef0-143">C#</span><span class="sxs-lookup"><span data-stu-id="fdef0-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fdef0-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fdef0-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fdef0-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fdef0-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fdef0-146">Java</span><span class="sxs-lookup"><span data-stu-id="fdef0-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-file-attachment-from-eventmessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fdef0-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="fdef0-147">Response</span></span>
<span data-ttu-id="fdef0-p104">Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fdef0-p104">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP 201 Created
```


## <a name="example-item-attachment"></a><span data-ttu-id="fdef0-150">Пример (вложенный элемент)</span><span class="sxs-lookup"><span data-stu-id="fdef0-150">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="fdef0-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="fdef0-151">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fdef0-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="fdef0-152">HTTP</span></span>](#tab/http)
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
  "item": {
    "@odata.type": "microsoft.graph.message"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="fdef0-153">C#</span><span class="sxs-lookup"><span data-stu-id="fdef0-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-item-attachment-from-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fdef0-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fdef0-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-item-attachment-from-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fdef0-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fdef0-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-item-attachment-from-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fdef0-156">Java</span><span class="sxs-lookup"><span data-stu-id="fdef0-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-item-attachment-from-eventmessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fdef0-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="fdef0-157">Response</span></span>
<span data-ttu-id="fdef0-p105">Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fdef0-p105">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response"
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


