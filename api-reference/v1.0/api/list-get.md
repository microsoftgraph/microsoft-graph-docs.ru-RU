---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Получение списка SharePoint
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 4f623aa940ad71a593d68df1d86e4d18360277b9
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272060"
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="90e27-102">Получение метаданных списка</span><span class="sxs-lookup"><span data-stu-id="90e27-102">Get metadata for a list</span></span>

<span data-ttu-id="90e27-103">Возвращает метаданные для [списка][].</span><span class="sxs-lookup"><span data-stu-id="90e27-103">Returns the metadata for a [list][].</span></span>

[списка]: ../resources/list.md
[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="90e27-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="90e27-105">Permissions</span></span>

<span data-ttu-id="90e27-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90e27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90e27-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90e27-108">Permission type</span></span>      | <span data-ttu-id="90e27-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90e27-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90e27-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90e27-110">Delegated (work or school account)</span></span> | <span data-ttu-id="90e27-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90e27-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="90e27-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90e27-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90e27-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90e27-113">Not supported.</span></span>    |
|<span data-ttu-id="90e27-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90e27-114">Application</span></span> | <span data-ttu-id="90e27-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90e27-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="90e27-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90e27-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="90e27-117">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="90e27-117">Request body</span></span>

<span data-ttu-id="90e27-118">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="90e27-118">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="90e27-119">Пример</span><span class="sxs-lookup"><span data-stu-id="90e27-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="90e27-120">Запрос</span><span class="sxs-lookup"><span data-stu-id="90e27-120">Request</span></span>

<!-- { "blockType": "request", "name": "get-list", "scopes": "sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}
```

#### <a name="response"></a><span data-ttu-id="90e27-121">Отклик</span><span class="sxs-lookup"><span data-stu-id="90e27-121">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="90e27-122">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="90e27-122">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="90e27-123">C#</span><span class="sxs-lookup"><span data-stu-id="90e27-123">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-list-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="90e27-124">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90e27-124">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-list-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="90e27-125">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90e27-125">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-list-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="90e27-126">С помощью операторов `select` и `expand` вы можете получить метаданные списка, определения столбцов и элементы списка в одном запросе.</span><span class="sxs-lookup"><span data-stu-id="90e27-126">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="90e27-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="90e27-127">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-multi-expand", "scopes": "sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}?select=id,name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```

#### <a name="response"></a><span data-ttu-id="90e27-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="90e27-128">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="90e27-129">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="90e27-129">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="90e27-130">C#</span><span class="sxs-lookup"><span data-stu-id="90e27-130">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-list-multi-expand-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="90e27-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90e27-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-list-multi-expand-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="90e27-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90e27-132">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-list-multi-expand-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Get metadata",
  "suppressions": [
    "Error: /api-reference/v1.0/api/list-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/list-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/list-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/list-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/list-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
