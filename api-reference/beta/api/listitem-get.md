---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Получение записи из списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 0864650701f9f6d4ee195373b5875dfe5a86b46a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35449164"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="3220d-102">Получение элемента списка</span><span class="sxs-lookup"><span data-stu-id="3220d-102">Get an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3220d-103">Возвращает метаданные [элемента][] в [списке][].</span><span class="sxs-lookup"><span data-stu-id="3220d-103">Returns the metadata for an [item][] in a [list][].</span></span>

[списке]: ../resources/list.md
[list]: ../resources/list.md
[элемента]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="3220d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3220d-106">Permissions</span></span>

<span data-ttu-id="3220d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3220d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3220d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3220d-109">Permission type</span></span>      | <span data-ttu-id="3220d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3220d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3220d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3220d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3220d-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3220d-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3220d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3220d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3220d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3220d-114">Not supported.</span></span>    |
|<span data-ttu-id="3220d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3220d-115">Application</span></span> | <span data-ttu-id="3220d-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3220d-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3220d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3220d-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="3220d-118">Пример</span><span class="sxs-lookup"><span data-stu-id="3220d-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3220d-119">Запрос</span><span class="sxs-lookup"><span data-stu-id="3220d-119">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3220d-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="3220d-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-item" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3220d-121">C#</span><span class="sxs-lookup"><span data-stu-id="3220d-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3220d-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="3220d-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3220d-123">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3220d-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3220d-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="3220d-124">Response</span></span>

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
