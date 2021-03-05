---
author: JeremyKelley
title: Получение списка SharePoint
localization_priority: Priority
ms.prod: sharepoint
description: Возвращает метаданные для списка.
doc_type: apiPageType
ms.openlocfilehash: e75f0b0431368b5937395857cf358ae10da6ded4
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471707"
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="84062-103">Получение метаданных списка</span><span class="sxs-lookup"><span data-stu-id="84062-103">Get metadata for a list</span></span>

<span data-ttu-id="84062-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84062-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="84062-105">Возвращает метаданные для [списка][].</span><span class="sxs-lookup"><span data-stu-id="84062-105">Returns the metadata for a [list][].</span></span>

[списка]: ../resources/list.md
[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="84062-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="84062-107">Permissions</span></span>

<span data-ttu-id="84062-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84062-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="84062-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84062-110">Permission type</span></span>                        | <span data-ttu-id="84062-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="84062-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="84062-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84062-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="84062-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84062-113">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="84062-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84062-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84062-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84062-115">Not supported.</span></span>                              |
| <span data-ttu-id="84062-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84062-116">Application</span></span>                            | <span data-ttu-id="84062-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84062-117">Sites.Read.All, Sites.ReadWrite.All</span></span>         |

## <a name="http-request"></a><span data-ttu-id="84062-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84062-118">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-title}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="84062-119">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="84062-119">Request body</span></span>

<span data-ttu-id="84062-120">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="84062-120">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="84062-121">Пример</span><span class="sxs-lookup"><span data-stu-id="84062-121">Example</span></span>

#### <a name="request"></a><span data-ttu-id="84062-122">Запрос</span><span class="sxs-lookup"><span data-stu-id="84062-122">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="84062-123">HTTP</span><span class="sxs-lookup"><span data-stu-id="84062-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list", "scopes": "sites.read.all" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-id}
```
# <a name="c"></a>[<span data-ttu-id="84062-124">C#</span><span class="sxs-lookup"><span data-stu-id="84062-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84062-125">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84062-125">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84062-126">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84062-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="84062-127">Java</span><span class="sxs-lookup"><span data-stu-id="84062-127">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="84062-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="84062-128">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
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

<span data-ttu-id="84062-129">С помощью операторов `select` и `expand` вы можете получить метаданные списка, определения столбцов и элементы списка в одном запросе.</span><span class="sxs-lookup"><span data-stu-id="84062-129">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="84062-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="84062-130">Request</span></span>
<span data-ttu-id="84062-131">В приведенном ниже примере показано, как получить список из заголовка списка SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="84062-131">The following example shows how to get a list from a SharePoint Online list title.</span></span>

# <a name="http"></a>[<span data-ttu-id="84062-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="84062-132">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list", "scopes": "sites.read.all" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-title}
```
# <a name="c"></a>[<span data-ttu-id="84062-133">C#</span><span class="sxs-lookup"><span data-stu-id="84062-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84062-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84062-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84062-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84062-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="84062-136">Java</span><span class="sxs-lookup"><span data-stu-id="84062-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="84062-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="84062-137">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
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

<span data-ttu-id="84062-138">С помощью операторов `select` и `expand` вы можете получить метаданные списка, определения столбцов и элементы списка в одном запросе.</span><span class="sxs-lookup"><span data-stu-id="84062-138">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="84062-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="84062-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="84062-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="84062-140">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-multi-expand", "scopes": "sites.read.all" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-id}?select=id,name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```
# <a name="c"></a>[<span data-ttu-id="84062-141">C#</span><span class="sxs-lookup"><span data-stu-id="84062-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-multi-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84062-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84062-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-multi-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84062-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84062-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-multi-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="84062-144">Java</span><span class="sxs-lookup"><span data-stu-id="84062-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-multi-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="84062-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="84062-145">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
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

