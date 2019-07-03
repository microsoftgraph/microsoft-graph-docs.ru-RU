---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Возврат файлов
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 84958a6dcbadb0b92d7a25bfb36bb53edbd3189a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436524"
---
# <a name="check-in-changes-to-a-driveitem-resource"></a><span data-ttu-id="1ee71-102">Возврат изменений в ресурсе DriveItem</span><span class="sxs-lookup"><span data-stu-id="1ee71-102">Check-in changes to a DriveItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ee71-103">В этой статье рассказывается, как возвратить извлеченный ресурс DriveItem, чтобы сделать версию документа доступной другим пользователям.</span><span class="sxs-lookup"><span data-stu-id="1ee71-103">Check-in a checked out DriveItem resource, which makes the version of the document available to others.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ee71-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1ee71-104">Permissions</span></span>

<span data-ttu-id="1ee71-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ee71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ee71-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ee71-107">Permission type</span></span>      | <span data-ttu-id="1ee71-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ee71-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ee71-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ee71-109">Delegated (work or school account)</span></span> | <span data-ttu-id="1ee71-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ee71-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="1ee71-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ee71-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ee71-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ee71-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="1ee71-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1ee71-113">Application</span></span> | <span data-ttu-id="1ee71-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ee71-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ee71-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ee71-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkin
POST /groups/{groupId}/drive/items/{itemId}/checkin
POST /me/drive/items/{item-id}/checkin
POST /sites/{siteId}/drive/items/{itemId}/checkin
POST /users/{userId}/drive/items/{itemId}/checkin
```

### <a name="request-body"></a><span data-ttu-id="1ee71-116">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1ee71-116">Request body</span></span>

<span data-ttu-id="1ee71-117">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="1ee71-117">In the request body, provide a JSON object with the following parameters.</span></span>


|   <span data-ttu-id="1ee71-118">Имя</span><span class="sxs-lookup"><span data-stu-id="1ee71-118">Name</span></span>    | <span data-ttu-id="1ee71-119">Значение</span><span class="sxs-lookup"><span data-stu-id="1ee71-119">Value</span></span>  |                                                <span data-ttu-id="1ee71-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1ee71-120">Description</span></span>                                                |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="1ee71-121">checkInAs</span><span class="sxs-lookup"><span data-stu-id="1ee71-121">checkInAs</span></span> | <span data-ttu-id="1ee71-122">string</span><span class="sxs-lookup"><span data-stu-id="1ee71-122">string</span></span> | <span data-ttu-id="1ee71-123">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="1ee71-123">Optional.</span></span> <span data-ttu-id="1ee71-124">Желаемое состояние документа после завершения операции возврата.</span><span class="sxs-lookup"><span data-stu-id="1ee71-124">The desired status of the document after the check-in operation is complete.</span></span> <span data-ttu-id="1ee71-125">Может иметь значение `published` либо значение может быть не указано.</span><span class="sxs-lookup"><span data-stu-id="1ee71-125">Can be `published` or unspecified.</span></span> |
| <span data-ttu-id="1ee71-126">comment</span><span class="sxs-lookup"><span data-stu-id="1ee71-126">comment</span></span>   | <span data-ttu-id="1ee71-127">string</span><span class="sxs-lookup"><span data-stu-id="1ee71-127">string</span></span> | <span data-ttu-id="1ee71-128">Комментарий к возврату, сопоставленный с версией.</span><span class="sxs-lookup"><span data-stu-id="1ee71-128">A check-in comment that is associated with the version.</span></span>                                                   |

## <a name="example"></a><span data-ttu-id="1ee71-129">Пример</span><span class="sxs-lookup"><span data-stu-id="1ee71-129">Example</span></span>

<span data-ttu-id="1ee71-130">В этом примере показано, как возвратить файл, идентифицируемый по `{item-id}`.</span><span class="sxs-lookup"><span data-stu-id="1ee71-130">This example checks in a file identified by `{item-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1ee71-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ee71-131">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "checkin-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkin
Content-Type: application/json

{
  "comment": "Updating the latest guidelines"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1ee71-132">C#</span><span class="sxs-lookup"><span data-stu-id="1ee71-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/checkin-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1ee71-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="1ee71-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/checkin-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1ee71-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="1ee71-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/checkin-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="1ee71-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ee71-135">Response</span></span>

<span data-ttu-id="1ee71-136">При успешном выполнении вызова API возвращается отклик `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="1ee71-136">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="1ee71-137">Замечания</span><span class="sxs-lookup"><span data-stu-id="1ee71-137">Remarks</span></span>


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
