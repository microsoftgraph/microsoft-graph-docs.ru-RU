---
title: Добавление вложения
description: С помощью этого API можно создать объект Attachment.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ce7d77147df3dc04aad54e76f7c065b5e1a7f2ec
ms.sourcegitcommit: 6314172db76ba9f2c192d8c099d818c5e772d2b8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2021
ms.locfileid: "49910554"
---
# <a name="add-attachment"></a><span data-ttu-id="5a4de-103">Добавление вложения</span><span class="sxs-lookup"><span data-stu-id="5a4de-103">Add attachment</span></span>

<span data-ttu-id="5a4de-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a4de-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5a4de-105">С помощью этого API можно создать объект Attachment.</span><span class="sxs-lookup"><span data-stu-id="5a4de-105">Use this API to create a new Attachment.</span></span>

<span data-ttu-id="5a4de-106">Допустимые типы вложений:</span><span class="sxs-lookup"><span data-stu-id="5a4de-106">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="5a4de-107">файл (ресурс [fileAttachment](../resources/fileattachment.md));</span><span class="sxs-lookup"><span data-stu-id="5a4de-107">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="5a4de-108">элемент (контакт, событие или сообщение, представленные ресурсом [itemAttachment](../resources/itemattachment.md));</span><span class="sxs-lookup"><span data-stu-id="5a4de-108">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="5a4de-109">ссылка на файл (ресурс [referenceAttachment](../resources/referenceattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="5a4de-109">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="5a4de-110">Все эти типы ресурсов вложений являются производными от ресурса [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="5a4de-110">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="5a4de-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5a4de-111">Permissions</span></span>
<span data-ttu-id="5a4de-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a4de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a4de-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a4de-114">Permission type</span></span>      | <span data-ttu-id="5a4de-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a4de-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a4de-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a4de-116">Delegated (work or school account)</span></span> | <span data-ttu-id="5a4de-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a4de-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5a4de-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a4de-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a4de-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a4de-119">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5a4de-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a4de-120">Application</span></span> | <span data-ttu-id="5a4de-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a4de-121">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a4de-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a4de-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="5a4de-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a4de-123">Request headers</span></span>
| <span data-ttu-id="5a4de-124">Имя</span><span class="sxs-lookup"><span data-stu-id="5a4de-124">Name</span></span>       | <span data-ttu-id="5a4de-125">Тип</span><span class="sxs-lookup"><span data-stu-id="5a4de-125">Type</span></span> | <span data-ttu-id="5a4de-126">Описание</span><span class="sxs-lookup"><span data-stu-id="5a4de-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5a4de-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a4de-127">Authorization</span></span>  | <span data-ttu-id="5a4de-128">string</span><span class="sxs-lookup"><span data-stu-id="5a4de-128">string</span></span>  | <span data-ttu-id="5a4de-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5a4de-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5a4de-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5a4de-131">Content-Type</span></span> | <span data-ttu-id="5a4de-132">string</span><span class="sxs-lookup"><span data-stu-id="5a4de-132">string</span></span>  | <span data-ttu-id="5a4de-p103">Характер данных в теле объекта. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5a4de-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a4de-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5a4de-135">Request body</span></span>
<span data-ttu-id="5a4de-136">Предоставьте в тексте запроса описание объекта [Attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a4de-136">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5a4de-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a4de-137">Response</span></span>

<span data-ttu-id="5a4de-138">В случае успеха этот метод возвращает код отклика `201 Created` и объект [Attachment](../resources/attachment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5a4de-138">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="5a4de-139">Пример (вложенный файл)</span><span class="sxs-lookup"><span data-stu-id="5a4de-139">Example (File attachment)</span></span>
##### <a name="request"></a><span data-ttu-id="5a4de-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a4de-140">Request</span></span>
<span data-ttu-id="5a4de-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a4de-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5a4de-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a4de-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5a4de-143">C#</span><span class="sxs-lookup"><span data-stu-id="5a4de-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-file-attachment-from-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5a4de-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a4de-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-file-attachment-from-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5a4de-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a4de-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-file-attachment-from-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5a4de-146">Java</span><span class="sxs-lookup"><span data-stu-id="5a4de-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-file-attachment-from-eventmessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="5a4de-147">Предоставьте в тексте запроса описание объекта [attachment](../resources/attachment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a4de-147">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="5a4de-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a4de-148">Response</span></span>
<span data-ttu-id="5a4de-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5a4de-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 201 Created
```

## <a name="example-item-attachment"></a><span data-ttu-id="5a4de-152">Пример (вложенный элемент)</span><span class="sxs-lookup"><span data-stu-id="5a4de-152">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="5a4de-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a4de-153">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5a4de-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a4de-154">HTTP</span></span>](#tab/http)
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
  "item": {
    "@odata.type": "microsoft.graph.message"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="5a4de-155">C#</span><span class="sxs-lookup"><span data-stu-id="5a4de-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-item-attachment-from-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5a4de-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a4de-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-item-attachment-from-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5a4de-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a4de-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-item-attachment-from-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5a4de-158">Java</span><span class="sxs-lookup"><span data-stu-id="5a4de-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-item-attachment-from-eventmessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5a4de-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a4de-159">Response</span></span>
<span data-ttu-id="5a4de-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5a4de-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 201 Created
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
  ]
}-->

