---
author: JeremyKelley
title: Получение метаданных списка
description: Возвращаем метаданные для списка.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 5091e8de36ff357b00a9b2517fab968f4a99cd41
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958050"
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="c092c-103">Получение метаданных списка</span><span class="sxs-lookup"><span data-stu-id="c092c-103">Get metadata for a list</span></span>

<span data-ttu-id="c092c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c092c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c092c-105">Возвращение метаданных для [списка][].</span><span class="sxs-lookup"><span data-stu-id="c092c-105">Return the metadata for a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="c092c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c092c-107">Permissions</span></span>

<span data-ttu-id="c092c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c092c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c092c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c092c-110">Permission type</span></span>                        | <span data-ttu-id="c092c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c092c-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="c092c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c092c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c092c-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c092c-113">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="c092c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c092c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c092c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c092c-115">Not supported.</span></span>                              |
| <span data-ttu-id="c092c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c092c-116">Application</span></span>                            | <span data-ttu-id="c092c-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c092c-117">Sites.Read.All, Sites.ReadWrite.All</span></span>         |

## <a name="http-request"></a><span data-ttu-id="c092c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c092c-118">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-title}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="c092c-119">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c092c-119">Request body</span></span>

<span data-ttu-id="c092c-120">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c092c-120">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="c092c-121">Пример</span><span class="sxs-lookup"><span data-stu-id="c092c-121">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c092c-122">Запрос</span><span class="sxs-lookup"><span data-stu-id="c092c-122">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c092c-123">HTTP</span><span class="sxs-lookup"><span data-stu-id="c092c-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-1" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-id}
```
# <a name="c"></a>[<span data-ttu-id="c092c-124">C#</span><span class="sxs-lookup"><span data-stu-id="c092c-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c092c-125">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c092c-125">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c092c-126">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c092c-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c092c-127">Java</span><span class="sxs-lookup"><span data-stu-id="c092c-127">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c092c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="c092c-128">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all service.sharepoint" } -->

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

<span data-ttu-id="c092c-129">С помощью операторов `select` и `expand` вы можете получить метаданные списка, определения столбцов и элементы списка в одном запросе.</span><span class="sxs-lookup"><span data-stu-id="c092c-129">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="c092c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c092c-130">Request</span></span>
<span data-ttu-id="c092c-131">В приведенном ниже примере показано, как получить список из заголовка списка SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="c092c-131">The following example shows how to get a list from a SharePoint Online list title.</span></span>

# <a name="http"></a>[<span data-ttu-id="c092c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c092c-132">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-2" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-title}
```
# <a name="c"></a>[<span data-ttu-id="c092c-133">C#</span><span class="sxs-lookup"><span data-stu-id="c092c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c092c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c092c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c092c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c092c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c092c-136">Java</span><span class="sxs-lookup"><span data-stu-id="c092c-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c092c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="c092c-137">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all service.sharepoint" } -->

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

<span data-ttu-id="c092c-138">С помощью операторов `select` и `expand` вы можете получить метаданные списка, определения столбцов и элементы списка в одном запросе.</span><span class="sxs-lookup"><span data-stu-id="c092c-138">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="c092c-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="c092c-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c092c-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="c092c-140">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-multi-expand" } -->

```msgraph-interactive
GET /sites/{site-id}/lists/{list-id}?select=name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```
# <a name="c"></a>[<span data-ttu-id="c092c-141">C#</span><span class="sxs-lookup"><span data-stu-id="c092c-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-multi-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c092c-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c092c-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-multi-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c092c-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c092c-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-multi-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c092c-144">Java</span><span class="sxs-lookup"><span data-stu-id="c092c-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-multi-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c092c-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="c092c-145">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all service.sharepoint" } -->

```http
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
#### <a name="request"></a><span data-ttu-id="c092c-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="c092c-146">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-multi-expand" } -->

<span data-ttu-id="c092c-147">В следующем примере показано, как получить метаданные для списка, который содержит три столбца: Name, Quantity и Category.</span><span class="sxs-lookup"><span data-stu-id="c092c-147">The following example shows how to get metadata for a list that contains three columns: Name, Quantity, and Category.</span></span>
<span data-ttu-id="c092c-148">[Управляемые столбцы метаданных,](/sharepoint/managed-metadata) такие как значения возврата в виде термина ```Category``` ID и пары имен терминов.</span><span class="sxs-lookup"><span data-stu-id="c092c-148">[Managed Metadata](/sharepoint/managed-metadata) columns like ```Category``` return values as term ID and term name pair.</span></span>
```http
GET /sites/{site-id}/lists/{list-id}?select=name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Quantity,Category))
```

#### <a name="response"></a><span data-ttu-id="c092c-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="c092c-149">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all service.sharepoint" } -->

```http
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


