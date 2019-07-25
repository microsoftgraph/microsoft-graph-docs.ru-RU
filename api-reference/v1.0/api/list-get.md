---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Получение списка SharePoint
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 51a0b856b00069e52b46c493556475d525030f63
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888347"
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="d01a4-102">Получение метаданных списка</span><span class="sxs-lookup"><span data-stu-id="d01a4-102">Get metadata for a list</span></span>

<span data-ttu-id="d01a4-103">Возвращает метаданные для [списка][].</span><span class="sxs-lookup"><span data-stu-id="d01a4-103">Returns the metadata for a [list][].</span></span>

[списка]: ../resources/list.md
[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="d01a4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d01a4-105">Permissions</span></span>

<span data-ttu-id="d01a4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d01a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d01a4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d01a4-108">Permission type</span></span>      | <span data-ttu-id="d01a4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d01a4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d01a4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d01a4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d01a4-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d01a4-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d01a4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d01a4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d01a4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d01a4-113">Not supported.</span></span>    |
|<span data-ttu-id="d01a4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d01a4-114">Application</span></span> | <span data-ttu-id="d01a4-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d01a4-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d01a4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d01a4-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="d01a4-117">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d01a4-117">Request body</span></span>

<span data-ttu-id="d01a4-118">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d01a4-118">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="d01a4-119">Пример</span><span class="sxs-lookup"><span data-stu-id="d01a4-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d01a4-120">Запрос</span><span class="sxs-lookup"><span data-stu-id="d01a4-120">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d01a4-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="d01a4-121">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list", "scopes": "sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d01a4-122">C#</span><span class="sxs-lookup"><span data-stu-id="d01a4-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d01a4-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d01a4-123">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d01a4-124">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d01a4-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d01a4-125">Java</span><span class="sxs-lookup"><span data-stu-id="d01a4-125">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d01a4-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="d01a4-126">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "1234-112-112-4",
  "name": "MicroFeed",
  "createdDateTime": "2016-08-30T08:32:00Z",
  "lastModifiedDateTime": "2016-08-30T08:32:00Z",
  "list": {
    "hidden": false,
    "template": "genericList"
    }
}
```

<span data-ttu-id="d01a4-127">С помощью операторов `select` и `expand` вы можете получить метаданные списка, определения столбцов и элементы списка в одном запросе.</span><span class="sxs-lookup"><span data-stu-id="d01a4-127">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="d01a4-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="d01a4-128">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d01a4-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="d01a4-129">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-multi-expand", "scopes": "sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}?select=id,name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d01a4-130">C#</span><span class="sxs-lookup"><span data-stu-id="d01a4-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-multi-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d01a4-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d01a4-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-multi-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d01a4-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d01a4-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-multi-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d01a4-133">Java</span><span class="sxs-lookup"><span data-stu-id="d01a4-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-multi-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d01a4-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d01a4-134">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "1234-112-112-4",
  "name": "Inventory",
  "lastModifiedDateTime": "2016-08-30T08:32:00Z",
  "columns": [
    {
      "name": "Name",
      "description": "Customer-facing name of the SKU"
    },
    {
      "name": "Color",
      "description": "Color of the item in stock"
    },
    {
      "name": "Quantity",
      "description": "Number of items in stock"
    }
  ],
  "items": [
    {
      "id": "2",
      "fields": {
        "Name": "Gadget",
        "Color": "Red",
        "Quantity": 503
       }
    },
    {
      "id": "4",
      "fields": {
        "Name": "Widget",
        "Color": "Blue",
        "Quantity": 2357
       }
    },
    {
      "id": "7",
      "fields": {
        "Name": "Gizmo",
        "Color": "Green",
        "Quantity": 92
       }
    }
  ]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Get metadata",
  "suppressions": [
  ]
} -->
