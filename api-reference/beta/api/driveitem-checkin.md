---
author: JeremyKelley
description: В этой статье рассказывается, как возвратить извлеченный ресурс DriveItem, чтобы сделать версию документа доступной другим пользователям.
ms.date: 09/10/2017
title: Возврат файлов
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: ffdddf5e3800d2bfb14038c7bec5b1b8fdcb0809
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321066"
---
# <a name="check-in-changes-to-a-driveitem-resource"></a><span data-ttu-id="709bb-103">Возврат изменений в ресурсе DriveItem</span><span class="sxs-lookup"><span data-stu-id="709bb-103">Check-in changes to a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="709bb-104">В этой статье рассказывается, как возвратить извлеченный ресурс DriveItem, чтобы сделать версию документа доступной другим пользователям.</span><span class="sxs-lookup"><span data-stu-id="709bb-104">Check-in a checked out DriveItem resource, which makes the version of the document available to others.</span></span>

## <a name="permissions"></a><span data-ttu-id="709bb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="709bb-105">Permissions</span></span>

<span data-ttu-id="709bb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="709bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="709bb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="709bb-108">Permission type</span></span>      | <span data-ttu-id="709bb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="709bb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="709bb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="709bb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="709bb-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="709bb-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="709bb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="709bb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="709bb-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="709bb-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="709bb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="709bb-114">Application</span></span> | <span data-ttu-id="709bb-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="709bb-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="709bb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="709bb-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkin
POST /groups/{groupId}/drive/items/{itemId}/checkin
POST /me/drive/items/{item-id}/checkin
POST /sites/{siteId}/drive/items/{itemId}/checkin
POST /users/{userId}/drive/items/{itemId}/checkin
```

### <a name="request-body"></a><span data-ttu-id="709bb-117">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="709bb-117">Request body</span></span>

<span data-ttu-id="709bb-118">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="709bb-118">In the request body, provide a JSON object with the following parameters.</span></span>


|   <span data-ttu-id="709bb-119">Имя</span><span class="sxs-lookup"><span data-stu-id="709bb-119">Name</span></span>    | <span data-ttu-id="709bb-120">Значение</span><span class="sxs-lookup"><span data-stu-id="709bb-120">Value</span></span>  |                                                <span data-ttu-id="709bb-121">Описание</span><span class="sxs-lookup"><span data-stu-id="709bb-121">Description</span></span>                                                |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="709bb-122">checkInAs</span><span class="sxs-lookup"><span data-stu-id="709bb-122">checkInAs</span></span> | <span data-ttu-id="709bb-123">string</span><span class="sxs-lookup"><span data-stu-id="709bb-123">string</span></span> | <span data-ttu-id="709bb-124">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="709bb-124">Optional.</span></span> <span data-ttu-id="709bb-125">Желаемое состояние документа после завершения операции возврата.</span><span class="sxs-lookup"><span data-stu-id="709bb-125">The desired status of the document after the check-in operation is complete.</span></span> <span data-ttu-id="709bb-126">Может иметь значение `published` либо значение может быть не указано.</span><span class="sxs-lookup"><span data-stu-id="709bb-126">Can be `published` or unspecified.</span></span> |
| <span data-ttu-id="709bb-127">comment</span><span class="sxs-lookup"><span data-stu-id="709bb-127">comment</span></span>   | <span data-ttu-id="709bb-128">string</span><span class="sxs-lookup"><span data-stu-id="709bb-128">string</span></span> | <span data-ttu-id="709bb-129">Комментарий к возврату, сопоставленный с версией.</span><span class="sxs-lookup"><span data-stu-id="709bb-129">A check-in comment that is associated with the version.</span></span>                                                   |

## <a name="example"></a><span data-ttu-id="709bb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="709bb-130">Example</span></span>

<span data-ttu-id="709bb-131">В этом примере показано, как возвратить файл, идентифицируемый по `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="709bb-131">This example checks in a file identified by `{item-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="709bb-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="709bb-132">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "checkin-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkin
Content-Type: application/json

{
  "comment": "Updating the latest guidelines"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="709bb-133">C#</span><span class="sxs-lookup"><span data-stu-id="709bb-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/checkin-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="709bb-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="709bb-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/checkin-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="709bb-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="709bb-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/checkin-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="709bb-136">Java</span><span class="sxs-lookup"><span data-stu-id="709bb-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/checkin-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="709bb-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="709bb-137">Response</span></span>

<span data-ttu-id="709bb-138">При успешном выполнении вызова API возвращается отклик `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="709bb-138">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="709bb-139">Замечания</span><span class="sxs-lookup"><span data-stu-id="709bb-139">Remarks</span></span>


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
