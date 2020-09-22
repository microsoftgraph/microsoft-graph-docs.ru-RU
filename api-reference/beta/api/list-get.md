---
author: JeremyKelley
title: Получение метаданных списка
description: Возвращает метаданные для списка.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 117a6c04cebc19927b7f62ec82aa585ca51f4863
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48068051"
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="56bb6-103">Получение метаданных списка</span><span class="sxs-lookup"><span data-stu-id="56bb6-103">Get metadata for a list</span></span>

<span data-ttu-id="56bb6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56bb6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56bb6-105">Возвращает метаданные для [списка][].</span><span class="sxs-lookup"><span data-stu-id="56bb6-105">Return the metadata for a [list][].</span></span>

[списка]: ../resources/list.md
[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="56bb6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="56bb6-107">Permissions</span></span>

<span data-ttu-id="56bb6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56bb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="56bb6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56bb6-110">Permission type</span></span>                        | <span data-ttu-id="56bb6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="56bb6-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="56bb6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56bb6-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="56bb6-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56bb6-113">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="56bb6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56bb6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56bb6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56bb6-115">Not supported.</span></span>                              |
| <span data-ttu-id="56bb6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="56bb6-116">Application</span></span>                            | <span data-ttu-id="56bb6-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56bb6-117">Sites.Read.All, Sites.ReadWrite.All</span></span>         |

## <a name="http-request"></a><span data-ttu-id="56bb6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56bb6-118">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-title}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="56bb6-119">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="56bb6-119">Request body</span></span>

<span data-ttu-id="56bb6-120">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="56bb6-120">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="56bb6-121">Пример</span><span class="sxs-lookup"><span data-stu-id="56bb6-121">Example</span></span>

#### <a name="request"></a><span data-ttu-id="56bb6-122">Запрос</span><span class="sxs-lookup"><span data-stu-id="56bb6-122">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="56bb6-123">HTTP</span><span class="sxs-lookup"><span data-stu-id="56bb6-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-id}
```
# <a name="c"></a>[<span data-ttu-id="56bb6-124">C#</span><span class="sxs-lookup"><span data-stu-id="56bb6-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="56bb6-125">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56bb6-125">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="56bb6-126">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56bb6-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="56bb6-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="56bb6-127">Response</span></span>

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

<span data-ttu-id="56bb6-128">С помощью операторов `select` и `expand` вы можете получить метаданные списка, определения столбцов и элементы списка в одном запросе.</span><span class="sxs-lookup"><span data-stu-id="56bb6-128">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="56bb6-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="56bb6-129">Request</span></span>
<span data-ttu-id="56bb6-130">В приведенном ниже примере показано, как получить список из заголовка списка SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="56bb6-130">The following example shows how to get a list from a SharePoint Online list title.</span></span>

# <a name="http"></a>[<span data-ttu-id="56bb6-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="56bb6-131">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-title}
```
# <a name="c"></a>[<span data-ttu-id="56bb6-132">C#</span><span class="sxs-lookup"><span data-stu-id="56bb6-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="56bb6-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56bb6-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="56bb6-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56bb6-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="56bb6-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="56bb6-135">Response</span></span>

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

<span data-ttu-id="56bb6-136">С помощью операторов `select` и `expand` вы можете получить метаданные списка, определения столбцов и элементы списка в одном запросе.</span><span class="sxs-lookup"><span data-stu-id="56bb6-136">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="56bb6-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="56bb6-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="56bb6-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="56bb6-138">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-multi-expand" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-id}?select=name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```
# <a name="c"></a>[<span data-ttu-id="56bb6-139">C#</span><span class="sxs-lookup"><span data-stu-id="56bb6-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-multi-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="56bb6-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56bb6-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-multi-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="56bb6-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56bb6-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-multi-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="56bb6-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="56bb6-142">Response</span></span>

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
#### <a name="request"></a><span data-ttu-id="56bb6-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="56bb6-143">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-multi-expand" } -->

<span data-ttu-id="56bb6-144">В приведенном ниже примере показано, как получить метаданные для списка, содержащего три столбца: Name, Quantity и category.</span><span class="sxs-lookup"><span data-stu-id="56bb6-144">The following example shows how to get metadata for a list that contains three columns: Name, Quantity, and Category.</span></span>
<span data-ttu-id="56bb6-145">Столбцы [управляемых метаданных](/sharepoint/managed-metadata) ```Category``` , такие как возвращаемые значения, в качестве идентификатора термина и имени термина.</span><span class="sxs-lookup"><span data-stu-id="56bb6-145">[Managed Metadata](/sharepoint/managed-metadata) columns like ```Category``` return values as term ID and term name pair.</span></span>
```http
GET /sites/{site-id}/lists/{list-id}?select=name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Quantity,Category))
```

#### <a name="response"></a><span data-ttu-id="56bb6-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="56bb6-146">Response</span></span>

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


