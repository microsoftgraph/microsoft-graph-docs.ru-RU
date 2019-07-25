---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Получение записи из списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 90095dce5b5cfdadfd37696cd9b43a7a5475b6f6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880237"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="117d9-102">Получение элемента списка</span><span class="sxs-lookup"><span data-stu-id="117d9-102">Get an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="117d9-103">Возвращает метаданные [элемента][] в [списке][].</span><span class="sxs-lookup"><span data-stu-id="117d9-103">Returns the metadata for an [item][] in a [list][].</span></span>

[списке]: ../resources/list.md
[list]: ../resources/list.md
[элемента]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="117d9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="117d9-106">Permissions</span></span>

<span data-ttu-id="117d9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="117d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="117d9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="117d9-109">Permission type</span></span>      | <span data-ttu-id="117d9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="117d9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="117d9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="117d9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="117d9-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="117d9-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="117d9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="117d9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="117d9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="117d9-114">Not supported.</span></span>    |
|<span data-ttu-id="117d9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="117d9-115">Application</span></span> | <span data-ttu-id="117d9-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="117d9-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="117d9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="117d9-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="117d9-118">Пример</span><span class="sxs-lookup"><span data-stu-id="117d9-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="117d9-119">Запрос</span><span class="sxs-lookup"><span data-stu-id="117d9-119">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="117d9-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="117d9-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-item" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="117d9-121">C#</span><span class="sxs-lookup"><span data-stu-id="117d9-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="117d9-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="117d9-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="117d9-123">Цель — C</span><span class="sxs-lookup"><span data-stu-id="117d9-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="117d9-124">Java</span><span class="sxs-lookup"><span data-stu-id="117d9-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="117d9-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="117d9-125">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "d14922d8-43e6-4c8a-b029-e35c5b4e0d63",
  "listItemId": 2,
  "fields": {
    "Name": "Widget",
    "Color": "Blue",
    "Quantity": 2357
    }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata",
  "suppressions": [
  ]
}
-->
