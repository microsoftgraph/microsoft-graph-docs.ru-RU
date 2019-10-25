---
author: JeremyKelley
description: Возвращает метаданные элемента в списке.
ms.date: 09/11/2017
title: Получение записи из списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 537785e9f9dcb6f8c991d0564dc7be1fbc4d06b7
ms.sourcegitcommit: bbef506636bce5b72351ee3834123771c301b1b1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/25/2019
ms.locfileid: "37726308"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="87ae0-103">Получение элемента списка</span><span class="sxs-lookup"><span data-stu-id="87ae0-103">Get an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87ae0-104">Возвращает метаданные [элемента][] в [списке][].</span><span class="sxs-lookup"><span data-stu-id="87ae0-104">Returns the metadata for an [item][] in a [list][].</span></span>

[списке]: ../resources/list.md
[list]: ../resources/list.md
[элемента]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="87ae0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="87ae0-107">Permissions</span></span>

<span data-ttu-id="87ae0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87ae0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87ae0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87ae0-110">Permission type</span></span>      | <span data-ttu-id="87ae0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="87ae0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87ae0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87ae0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="87ae0-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87ae0-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="87ae0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87ae0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87ae0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87ae0-115">Not supported.</span></span>    |
|<span data-ttu-id="87ae0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="87ae0-116">Application</span></span> | <span data-ttu-id="87ae0-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87ae0-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="87ae0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87ae0-118">HTTP request</span></span>

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET /sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="87ae0-119">Пример</span><span class="sxs-lookup"><span data-stu-id="87ae0-119">Example</span></span>

##### <a name="request"></a><span data-ttu-id="87ae0-120">Запрос</span><span class="sxs-lookup"><span data-stu-id="87ae0-120">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="87ae0-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="87ae0-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-item" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="87ae0-122">C#</span><span class="sxs-lookup"><span data-stu-id="87ae0-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="87ae0-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="87ae0-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="87ae0-124">Objective-C</span><span class="sxs-lookup"><span data-stu-id="87ae0-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="87ae0-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="87ae0-125">Response</span></span>

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
