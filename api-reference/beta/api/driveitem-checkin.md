---
author: JeremyKelley
description: Возврат извлеченного ресурса DriveItem, который делает версию документа доступной другим пользователям.
title: 'driveItem: checkin'
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 8cc008e18bd70acfed0bb6b951d3694f3cc9593d
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "43227584"
---
# <a name="driveitem-checkin"></a><span data-ttu-id="6f9af-103">driveItem: checkin</span><span class="sxs-lookup"><span data-stu-id="6f9af-103">driveItem: checkin</span></span>

<span data-ttu-id="6f9af-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f9af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f9af-105">Возврат извлеченного ресурса **driveItem** , который делает версию документа доступной другим пользователям.</span><span class="sxs-lookup"><span data-stu-id="6f9af-105">Check in a checked out **driveItem** resource, which makes the version of the document available to others.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f9af-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6f9af-106">Permissions</span></span>

<span data-ttu-id="6f9af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f9af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f9af-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f9af-109">Permission type</span></span>      | <span data-ttu-id="6f9af-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f9af-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f9af-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f9af-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6f9af-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f9af-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="6f9af-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f9af-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f9af-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f9af-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="6f9af-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f9af-115">Application</span></span> | <span data-ttu-id="6f9af-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f9af-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f9af-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f9af-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkin
POST /groups/{groupId}/drive/items/{itemId}/checkin
POST /me/drive/items/{item-id}/checkin
POST /sites/{siteId}/drive/items/{itemId}/checkin
POST /users/{userId}/drive/items/{itemId}/checkin
```

### <a name="request-body"></a><span data-ttu-id="6f9af-118">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6f9af-118">Request body</span></span>

<span data-ttu-id="6f9af-119">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="6f9af-119">In the request body, provide a JSON object with the following parameters.</span></span>


|   <span data-ttu-id="6f9af-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6f9af-120">Name</span></span>    | <span data-ttu-id="6f9af-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6f9af-121">Value</span></span>  |                                                <span data-ttu-id="6f9af-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6f9af-122">Description</span></span>                                                |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="6f9af-123">checkInAs</span><span class="sxs-lookup"><span data-stu-id="6f9af-123">checkInAs</span></span> | <span data-ttu-id="6f9af-124">string</span><span class="sxs-lookup"><span data-stu-id="6f9af-124">string</span></span> | <span data-ttu-id="6f9af-125">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="6f9af-125">Optional.</span></span> <span data-ttu-id="6f9af-126">Состояние документа после завершения операции возврата.</span><span class="sxs-lookup"><span data-stu-id="6f9af-126">The status of the document after the check-in operation is complete.</span></span> <span data-ttu-id="6f9af-127">Может иметь значение `published` либо значение может быть не указано.</span><span class="sxs-lookup"><span data-stu-id="6f9af-127">Can be `published` or unspecified.</span></span> |
| <span data-ttu-id="6f9af-128">comment</span><span class="sxs-lookup"><span data-stu-id="6f9af-128">comment</span></span>   | <span data-ttu-id="6f9af-129">string</span><span class="sxs-lookup"><span data-stu-id="6f9af-129">string</span></span> | <span data-ttu-id="6f9af-130">Комментарий к возврату, сопоставленный с версией.</span><span class="sxs-lookup"><span data-stu-id="6f9af-130">A check-in comment that is associated with the version.</span></span>                                                   |

## <a name="example"></a><span data-ttu-id="6f9af-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6f9af-131">Example</span></span>

<span data-ttu-id="6f9af-132">В этом примере показано, как возвратить файл, идентифицируемый по `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="6f9af-132">This example checks in a file identified by `{item-id}`.</span></span>


# <a name="http"></a>[<span data-ttu-id="6f9af-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f9af-133">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "checkin-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkin
Content-Type: application/json

{
  "comment": "Updating the latest guidelines"
}
```
# <a name="c"></a>[<span data-ttu-id="6f9af-134">C#</span><span class="sxs-lookup"><span data-stu-id="6f9af-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/checkin-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f9af-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f9af-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/checkin-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f9af-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f9af-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/checkin-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="6f9af-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f9af-137">Response</span></span>

<span data-ttu-id="6f9af-138">При успешном выполнении вызова API возвращается отклик `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="6f9af-138">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="6f9af-139">Замечания</span><span class="sxs-lookup"><span data-stu-id="6f9af-139">Remarks</span></span>


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
