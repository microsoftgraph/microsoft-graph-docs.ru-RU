---
author: chackman
ms.author: chackman
title: Отписаться от элемента Drive
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: c2e687cb93d64994036cc46e8a245e707dd58b16
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436244"
---
# <a name="unfollow-drive-item"></a><span data-ttu-id="48aeb-102">Отписаться от элемента Drive</span><span class="sxs-lookup"><span data-stu-id="48aeb-102">Unfollow drive item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48aeb-103">Отменяйте подписку на [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="48aeb-103">Unfollow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="48aeb-104">**Примечание:** Чтобы подписаться на элемент, обратитесь к разделу [Отслеживание элемента](driveitem-follow.md).</span><span class="sxs-lookup"><span data-stu-id="48aeb-104">**Note:** To follow an item, see [Follow Item](driveitem-follow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="48aeb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48aeb-105">Permissions</span></span>

<span data-ttu-id="48aeb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48aeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48aeb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48aeb-108">Permission type</span></span>      | <span data-ttu-id="48aeb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="48aeb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48aeb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48aeb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="48aeb-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48aeb-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="48aeb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48aeb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48aeb-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48aeb-113">Not supported.</span></span>    |
|<span data-ttu-id="48aeb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48aeb-114">Application</span></span> | <span data-ttu-id="48aeb-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48aeb-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="48aeb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48aeb-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/drive/following/{item-id} 
DELETE /users/{user-id}/drive/following/{item-id}
```

## <a name="request-body"></a><span data-ttu-id="48aeb-117">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="48aeb-117">Request body</span></span>

<span data-ttu-id="48aeb-118">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="48aeb-118">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="48aeb-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="48aeb-119">Response</span></span>

<span data-ttu-id="48aeb-120">При успешном выполнении вызова API возвращается отклик `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="48aeb-120">If successful, the API call returns a `204 No Content`.</span></span> <span data-ttu-id="48aeb-121">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="48aeb-121">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48aeb-122">Пример</span><span class="sxs-lookup"><span data-stu-id="48aeb-122">Example</span></span>
### <a name="request"></a><span data-ttu-id="48aeb-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="48aeb-123">Request</span></span>
<span data-ttu-id="48aeb-124">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48aeb-124">Here is an example of the request.</span></span>
<span data-ttu-id="48aeb-125">В этом примере отменяется отслеживание элемента, `{item-id}`указанного в параметре.</span><span class="sxs-lookup"><span data-stu-id="48aeb-125">This example unfollows an item identified by `{item-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="48aeb-126">HTTP</span><span class="sxs-lookup"><span data-stu-id="48aeb-126">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "unfollow-item", "scopes": "files.read" } -->

```http
DELETE /me/drive/following/{item-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="48aeb-127">C#</span><span class="sxs-lookup"><span data-stu-id="48aeb-127">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unfollow-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="48aeb-128">Javascript</span><span class="sxs-lookup"><span data-stu-id="48aeb-128">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unfollow-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="48aeb-129">Цель — C</span><span class="sxs-lookup"><span data-stu-id="48aeb-129">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unfollow-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="48aeb-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="48aeb-130">Response</span></span>
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
