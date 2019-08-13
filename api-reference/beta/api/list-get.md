---
author: JeremyKelley
title: Получение метаданных списка
description: Возвращает метаданные для списка.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: ba0760edc006e3e79ff04b18652baa5c4c986e5d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350008"
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="c9dd0-103">Получение метаданных списка</span><span class="sxs-lookup"><span data-stu-id="c9dd0-103">Get metadata for a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9dd0-104">Возвращает метаданные для [списка][].</span><span class="sxs-lookup"><span data-stu-id="c9dd0-104">Return the metadata for a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="c9dd0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c9dd0-106">Permissions</span></span>

<span data-ttu-id="c9dd0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9dd0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9dd0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9dd0-109">Permission type</span></span>      | <span data-ttu-id="c9dd0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9dd0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9dd0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9dd0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c9dd0-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9dd0-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c9dd0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9dd0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9dd0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9dd0-114">Not supported.</span></span>    |
|<span data-ttu-id="c9dd0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9dd0-115">Application</span></span> | <span data-ttu-id="c9dd0-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9dd0-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9dd0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9dd0-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="c9dd0-118">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c9dd0-118">Request body</span></span>

<span data-ttu-id="c9dd0-119">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c9dd0-119">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="c9dd0-120">Пример</span><span class="sxs-lookup"><span data-stu-id="c9dd0-120">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c9dd0-121">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9dd0-121">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c9dd0-122">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9dd0-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list" } -->

```http
GET /sites/{site-id}/lists/{list-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c9dd0-123">C#</span><span class="sxs-lookup"><span data-stu-id="c9dd0-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c9dd0-124">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9dd0-124">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c9dd0-125">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c9dd0-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c9dd0-126">Java</span><span class="sxs-lookup"><span data-stu-id="c9dd0-126">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c9dd0-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9dd0-127">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all service.sharepoint" } -->

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

<span data-ttu-id="c9dd0-128">С помощью операторов `select` и `expand` вы можете получить метаданные списка, определения столбцов и элементы списка в одном запросе.</span><span class="sxs-lookup"><span data-stu-id="c9dd0-128">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="c9dd0-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9dd0-129">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c9dd0-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9dd0-130">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-multi-expand" } -->

```http
GET /sites/{site-id}/lists/{list-id}?select=name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c9dd0-131">C#</span><span class="sxs-lookup"><span data-stu-id="c9dd0-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-multi-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c9dd0-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9dd0-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-multi-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c9dd0-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c9dd0-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-multi-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c9dd0-134">Java</span><span class="sxs-lookup"><span data-stu-id="c9dd0-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-multi-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c9dd0-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9dd0-135">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all service.sharepoint" } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
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
#### <a name="request"></a><span data-ttu-id="c9dd0-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9dd0-136">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-multi-expand" } -->

<span data-ttu-id="c9dd0-137">В приведенном ниже примере показано, как получить метаданные для списка, содержащего три столбца: Name, Quantity и category.</span><span class="sxs-lookup"><span data-stu-id="c9dd0-137">The following example shows how to get metadata for a list that contains three columns: Name, Quantity, and Category.</span></span>
<span data-ttu-id="c9dd0-138">Столбцы [управляемых метаданных](https://docs.microsoft.com/en-us/sharepoint/managed-metadata) , ```Category``` такие как возвращаемые значения, в качестве идентификатора термина и имени термина.</span><span class="sxs-lookup"><span data-stu-id="c9dd0-138">[Managed Metadata](https://docs.microsoft.com/en-us/sharepoint/managed-metadata) columns like ```Category``` return values as term ID and term name pair.</span></span>
```http
GET /sites/{site-id}/lists/{list-id}?select=name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Quantity,Category))
```

#### <a name="response"></a><span data-ttu-id="c9dd0-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9dd0-139">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all service.sharepoint" } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "name": "Inventory",
  "lastModifiedDateTime": "2016-08-30T08:32:00Z",
  "columns": [
    {
      "name": "Name",
      "description": "Customer-facing name of the SKU"
    },
    {
      "name": "Quantity",
      "description": "Number of items in stock"
    },
    {
      "name": "Category",
      "description": "Category of the item"
    }
  ],
  "items": [
    {
      "id": "2",
      "fields": {
        "Name": "Gadget",
        "Quantity": 503,
        "Category": {
          "termId": "791d537a-9c1c-3b05-97b0-1ce7ece7e1a4",
          "name": "Tool"
         }
       }
    },
    {
      "id": "4",
      "fields": {
        "Name": "Widget",
        "Quantity": 2357,
        "Category": {
          "termId": "902e568b-9b2d-4d06-87c2-2cf8ecf9f2b5" ,
          "name": "Mechanical Device"
         }
       }
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Get metadata",
  "suppressions": [
  ]
}
-->
