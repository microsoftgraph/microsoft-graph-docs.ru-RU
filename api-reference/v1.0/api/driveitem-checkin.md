---
author: learafa
description: Возврат извлеченного ресурса driveItem, который делает версию документа доступной другим пользователям.
title: 'driveItem: checkin'
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: d6b38b5418b29bd9e86e664c95299a159a82c0f4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009921"
---
# <a name="driveitem-checkin"></a><span data-ttu-id="4ee74-103">driveItem: checkin</span><span class="sxs-lookup"><span data-stu-id="4ee74-103">driveItem: checkin</span></span>

<span data-ttu-id="4ee74-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ee74-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4ee74-105">Возврат извлеченного ресурса **driveItem** , который делает версию документа доступной другим пользователям.</span><span class="sxs-lookup"><span data-stu-id="4ee74-105">Check in a checked out **driveItem** resource, which makes the version of the document available to others.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ee74-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4ee74-106">Permissions</span></span>

<span data-ttu-id="4ee74-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ee74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ee74-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ee74-109">Permission type</span></span>      | <span data-ttu-id="4ee74-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ee74-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ee74-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ee74-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4ee74-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ee74-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4ee74-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ee74-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ee74-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ee74-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="4ee74-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ee74-115">Application</span></span> | <span data-ttu-id="4ee74-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ee74-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ee74-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ee74-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkin
POST /groups/{groupId}/drive/items/{itemId}/checkin
POST /me/drive/items/{item-id}/checkin
POST /sites/{siteId}/drive/items/{itemId}/checkin
POST /users/{userId}/drive/items/{itemId}/checkin
```

## <a name="request-body"></a><span data-ttu-id="4ee74-118">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4ee74-118">Request body</span></span>

<span data-ttu-id="4ee74-119">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4ee74-119">In the request body, provide a JSON object with the following parameters.</span></span>


|   <span data-ttu-id="4ee74-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4ee74-120">Name</span></span>    | <span data-ttu-id="4ee74-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4ee74-121">Value</span></span>  |                                                <span data-ttu-id="4ee74-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4ee74-122">Description</span></span>                                                |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="4ee74-123">checkInAs</span><span class="sxs-lookup"><span data-stu-id="4ee74-123">checkInAs</span></span> | <span data-ttu-id="4ee74-124">string</span><span class="sxs-lookup"><span data-stu-id="4ee74-124">string</span></span> | <span data-ttu-id="4ee74-125">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="4ee74-125">Optional.</span></span> <span data-ttu-id="4ee74-126">Состояние документа после завершения операции возврата.</span><span class="sxs-lookup"><span data-stu-id="4ee74-126">The status of the document after the check-in operation is complete.</span></span> <span data-ttu-id="4ee74-127">Может иметь значение `published` либо значение может быть не указано.</span><span class="sxs-lookup"><span data-stu-id="4ee74-127">Can be `published` or unspecified.</span></span> |
| <span data-ttu-id="4ee74-128">comment</span><span class="sxs-lookup"><span data-stu-id="4ee74-128">comment</span></span>   | <span data-ttu-id="4ee74-129">string</span><span class="sxs-lookup"><span data-stu-id="4ee74-129">string</span></span> | <span data-ttu-id="4ee74-130">Комментарий к возврату, сопоставленный с версией.</span><span class="sxs-lookup"><span data-stu-id="4ee74-130">A check-in comment that is associated with the version.</span></span>                                                   |

## <a name="response"></a><span data-ttu-id="4ee74-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ee74-131">Response</span></span>

<span data-ttu-id="4ee74-132">В случае успеха вызов API возвращает `204 No content` .</span><span class="sxs-lookup"><span data-stu-id="4ee74-132">If successful, the API call returns `204 No content`.</span></span>

## <a name="example"></a><span data-ttu-id="4ee74-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4ee74-133">Example</span></span>

<span data-ttu-id="4ee74-134">В этом примере показано, как возвратить файл, идентифицируемый по `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="4ee74-134">This example checks in a file identified by `{item-id}`.</span></span>

### <a name="request"></a><span data-ttu-id="4ee74-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ee74-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4ee74-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ee74-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "checkin-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkin
Content-Type: application/json

{
  "comment": "Updating the latest guidelines"
}
```
# <a name="c"></a>[<span data-ttu-id="4ee74-137">C#</span><span class="sxs-lookup"><span data-stu-id="4ee74-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/checkin-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ee74-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ee74-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/checkin-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ee74-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ee74-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/checkin-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4ee74-140">Java</span><span class="sxs-lookup"><span data-stu-id="4ee74-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/checkin-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4ee74-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ee74-141">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
  ]
}
-->

