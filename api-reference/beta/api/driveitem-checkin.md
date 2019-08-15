---
author: JeremyKelley
description: В этой статье рассказывается, как возвратить извлеченный ресурс DriveItem, чтобы сделать версию документа доступной другим пользователям.
ms.date: 09/10/2017
title: Возврат файлов
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 23dd00bcaeff1b6dcf23afa9eae7213cd7ee7e8d
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416879"
---
# <a name="check-in-changes-to-a-driveitem-resource"></a><span data-ttu-id="5ff6d-103">Возврат изменений в ресурсе DriveItem</span><span class="sxs-lookup"><span data-stu-id="5ff6d-103">Check-in changes to a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ff6d-104">В этой статье рассказывается, как возвратить извлеченный ресурс DriveItem, чтобы сделать версию документа доступной другим пользователям.</span><span class="sxs-lookup"><span data-stu-id="5ff6d-104">Check-in a checked out DriveItem resource, which makes the version of the document available to others.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ff6d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5ff6d-105">Permissions</span></span>

<span data-ttu-id="5ff6d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ff6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ff6d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ff6d-108">Permission type</span></span>      | <span data-ttu-id="5ff6d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ff6d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ff6d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ff6d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5ff6d-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ff6d-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="5ff6d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ff6d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ff6d-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ff6d-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="5ff6d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5ff6d-114">Application</span></span> | <span data-ttu-id="5ff6d-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ff6d-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ff6d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ff6d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkin
POST /groups/{groupId}/drive/items/{itemId}/checkin
POST /me/drive/items/{item-id}/checkin
POST /sites/{siteId}/drive/items/{itemId}/checkin
POST /users/{userId}/drive/items/{itemId}/checkin
```

### <a name="request-body"></a><span data-ttu-id="5ff6d-117">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5ff6d-117">Request body</span></span>

<span data-ttu-id="5ff6d-118">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="5ff6d-118">In the request body, provide a JSON object with the following parameters.</span></span>


|   <span data-ttu-id="5ff6d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5ff6d-119">Name</span></span>    | <span data-ttu-id="5ff6d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="5ff6d-120">Value</span></span>  |                                                <span data-ttu-id="5ff6d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="5ff6d-121">Description</span></span>                                                |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="5ff6d-122">checkInAs</span><span class="sxs-lookup"><span data-stu-id="5ff6d-122">checkInAs</span></span> | <span data-ttu-id="5ff6d-123">string</span><span class="sxs-lookup"><span data-stu-id="5ff6d-123">string</span></span> | <span data-ttu-id="5ff6d-124">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="5ff6d-124">Optional.</span></span> <span data-ttu-id="5ff6d-125">Желаемое состояние документа после завершения операции возврата.</span><span class="sxs-lookup"><span data-stu-id="5ff6d-125">The desired status of the document after the check-in operation is complete.</span></span> <span data-ttu-id="5ff6d-126">Может иметь значение `published` либо значение может быть не указано.</span><span class="sxs-lookup"><span data-stu-id="5ff6d-126">Can be `published` or unspecified.</span></span> |
| <span data-ttu-id="5ff6d-127">comment</span><span class="sxs-lookup"><span data-stu-id="5ff6d-127">comment</span></span>   | <span data-ttu-id="5ff6d-128">string</span><span class="sxs-lookup"><span data-stu-id="5ff6d-128">string</span></span> | <span data-ttu-id="5ff6d-129">Комментарий к возврату, сопоставленный с версией.</span><span class="sxs-lookup"><span data-stu-id="5ff6d-129">A check-in comment that is associated with the version.</span></span>                                                   |

## <a name="example"></a><span data-ttu-id="5ff6d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5ff6d-130">Example</span></span>

<span data-ttu-id="5ff6d-131">В этом примере показано, как возвратить файл, идентифицируемый по `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="5ff6d-131">This example checks in a file identified by `{item-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5ff6d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ff6d-132">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "checkin-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkin
Content-Type: application/json

{
  "comment": "Updating the latest guidelines"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5ff6d-133">C#</span><span class="sxs-lookup"><span data-stu-id="5ff6d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/checkin-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5ff6d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ff6d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/checkin-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5ff6d-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="5ff6d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/checkin-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="5ff6d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ff6d-136">Response</span></span>

<span data-ttu-id="5ff6d-137">При успешном выполнении вызова API возвращается отклик `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="5ff6d-137">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="5ff6d-138">Замечания</span><span class="sxs-lookup"><span data-stu-id="5ff6d-138">Remarks</span></span>


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
