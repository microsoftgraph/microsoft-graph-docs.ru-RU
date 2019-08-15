---
author: chackman
ms.author: chackman
description: Отменяйте подписку на элемент, на который подписан пользователь.
title: Отписаться от элемента Drive
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 6599b49ae54fc315802880ae3dccfd585585a7ce
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416620"
---
# <a name="unfollow-drive-item"></a><span data-ttu-id="f17ef-103">Отписаться от элемента Drive</span><span class="sxs-lookup"><span data-stu-id="f17ef-103">Unfollow drive item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f17ef-104">Отменяйте подписку на [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="f17ef-104">Unfollow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="f17ef-105">**Примечание:** Чтобы подписаться на элемент, обратитесь к разделу [Отслеживание элемента](driveitem-follow.md).</span><span class="sxs-lookup"><span data-stu-id="f17ef-105">**Note:** To follow an item, see [Follow Item](driveitem-follow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f17ef-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f17ef-106">Permissions</span></span>

<span data-ttu-id="f17ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f17ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f17ef-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f17ef-109">Permission type</span></span>      | <span data-ttu-id="f17ef-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f17ef-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f17ef-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f17ef-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f17ef-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f17ef-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f17ef-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f17ef-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f17ef-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f17ef-114">Not supported.</span></span>    |
|<span data-ttu-id="f17ef-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f17ef-115">Application</span></span> | <span data-ttu-id="f17ef-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f17ef-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f17ef-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f17ef-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/drive/following/{item-id}
DELETE /users/{user-id}/drive/following/{item-id}
POST /me/drive/items/{item-id}/unfollow
POST /users/{user-id}/drive/items/{item-id}/unfollow
```

## <a name="request-body"></a><span data-ttu-id="f17ef-118">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f17ef-118">Request body</span></span>

<span data-ttu-id="f17ef-119">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="f17ef-119">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="f17ef-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="f17ef-120">Response</span></span>

<span data-ttu-id="f17ef-121">При успешном выполнении вызова API возвращается отклик `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f17ef-121">If successful, the API call returns a `204 No Content`.</span></span> <span data-ttu-id="f17ef-122">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f17ef-122">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f17ef-123">Пример</span><span class="sxs-lookup"><span data-stu-id="f17ef-123">Example</span></span>
### <a name="request"></a><span data-ttu-id="f17ef-124">Запрос</span><span class="sxs-lookup"><span data-stu-id="f17ef-124">Request</span></span>
<span data-ttu-id="f17ef-125">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f17ef-125">Here is an example of the request.</span></span>
<span data-ttu-id="f17ef-126">В этом примере отменяется отслеживание элемента, `{item-id}`указанного в параметре.</span><span class="sxs-lookup"><span data-stu-id="f17ef-126">This example unfollows an item identified by `{item-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f17ef-127">HTTP</span><span class="sxs-lookup"><span data-stu-id="f17ef-127">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "unfollow-item", "scopes": "files.read" } -->

```http
DELETE /me/drive/items/{item-id}/unfollow
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f17ef-128">C#</span><span class="sxs-lookup"><span data-stu-id="f17ef-128">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unfollow-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f17ef-129">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f17ef-129">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unfollow-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f17ef-130">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f17ef-130">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unfollow-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="f17ef-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f17ef-131">Response</span></span>
<!-- { 
    "blockType": "response", 
    "truncated": true 
} -->
```http
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "description": "Unfollow an item that the user is following.",
  "keywords": "unfollow item",
  "section": "documentation",
  "tocPath": "Items/Unfollow",
  "suppressions": [
  ]
}
-->
