---
title: Определение /me как одноэлементного класса
description: Вот что нужно было добавить в документы, чтобы убедиться, что сканер Markdown
localization_priority: Normal
ms.openlocfilehash: 4ccdfdd669efe83d779cc3294b6372c4294d5179
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35459519"
---
# <a name="helpers-examples-that-arent-included-in-the-docs"></a><span data-ttu-id="26d92-103">Вспомогательный код (примеры, не включенные в документы)</span><span class="sxs-lookup"><span data-stu-id="26d92-103">Helpers (examples that aren't included in the docs)</span></span>

<span data-ttu-id="26d92-104">Ниже представлены фрагменты, которые пришлось добавить в документы, чтобы средство Markdown-Scanner могло правильно обработать документы по Graph.</span><span class="sxs-lookup"><span data-stu-id="26d92-104">These are things I had to add in the docs to make sure the Markdown-Scanner tool was able to properly handle the Graph docs.</span></span>


## <a name="define-the-me-as-singleton"></a><span data-ttu-id="26d92-105">Определение /me как одноэлементного класса</span><span class="sxs-lookup"><span data-stu-id="26d92-105">Define the /me as singleton</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="26d92-106">HTTP</span><span class="sxs-lookup"><span data-stu-id="26d92-106">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "get_current_user" } -->
```http
GET https://graph.microsoft.com/v1.0/me
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="26d92-107">C#</span><span class="sxs-lookup"><span data-stu-id="26d92-107">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-current-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="26d92-108">Javascript</span><span class="sxs-lookup"><span data-stu-id="26d92-108">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-current-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="26d92-109">Цель — C</span><span class="sxs-lookup"><span data-stu-id="26d92-109">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-current-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {"blockType": "response", "@odata.type": "microsoft.graph.user", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


## <a name="define-drives-as-an-queryable-entityset"></a><span data-ttu-id="26d92-110">Определение drives как набора EntitySet, поддерживающего запросы</span><span class="sxs-lookup"><span data-stu-id="26d92-110">Define drives as an queryable entityset</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="26d92-111">HTTP</span><span class="sxs-lookup"><span data-stu-id="26d92-111">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "get_drive_from_id" } -->
```http
GET https://graph.microsoft.com/v1.0/drives/{drive-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="26d92-112">C#</span><span class="sxs-lookup"><span data-stu-id="26d92-112">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-from-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="26d92-113">Javascript</span><span class="sxs-lookup"><span data-stu-id="26d92-113">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-from-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="26d92-114">Цель — C</span><span class="sxs-lookup"><span data-stu-id="26d92-114">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-from-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {"blockType": "response", "@odata.type": "microsoft.graph.drive", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


## <a name="define-users-as-an-queryable-entityset"></a><span data-ttu-id="26d92-115">Определение users как EntitySet, поддерживающего запросы</span><span class="sxs-lookup"><span data-stu-id="26d92-115">define users as an queryable entityset</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="26d92-116">HTTP</span><span class="sxs-lookup"><span data-stu-id="26d92-116">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "get_users" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{user-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="26d92-117">C#</span><span class="sxs-lookup"><span data-stu-id="26d92-117">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="26d92-118">Javascript</span><span class="sxs-lookup"><span data-stu-id="26d92-118">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="26d92-119">Цель — C</span><span class="sxs-lookup"><span data-stu-id="26d92-119">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {"blockType": "response", "@odata.type": "microsoft.graph.user", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d73
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Missing Requests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
