---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Получение списка SharePoint
ms.openlocfilehash: 042e9d6352d99f3a9e8d57daed685b6d9b2f7f65
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2018
ms.locfileid: "23264016"
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="d20d6-102">Получение метаданных списка</span><span class="sxs-lookup"><span data-stu-id="d20d6-102">Get metadata for a list</span></span>

<span data-ttu-id="d20d6-103">Возвращает метаданные для [списка][].</span><span class="sxs-lookup"><span data-stu-id="d20d6-103">Returns the metadata for a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="d20d6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d20d6-105">Permissions</span></span>

<span data-ttu-id="d20d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d20d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d20d6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d20d6-108">Permission type</span></span>      | <span data-ttu-id="d20d6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d20d6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d20d6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d20d6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d20d6-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d20d6-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d20d6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d20d6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d20d6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d20d6-113">Not supported.</span></span>    |
|<span data-ttu-id="d20d6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d20d6-114">Application</span></span> | <span data-ttu-id="d20d6-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d20d6-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d20d6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d20d6-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="d20d6-117">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d20d6-117">Request body</span></span>

<span data-ttu-id="d20d6-118">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d20d6-118">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="d20d6-119">Пример</span><span class="sxs-lookup"><span data-stu-id="d20d6-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d20d6-120">Запрос</span><span class="sxs-lookup"><span data-stu-id="d20d6-120">Request</span></span>

<!-- { "blockType": "request", "name": "get-list", "scopes": "sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}
```

#### <a name="response"></a><span data-ttu-id="d20d6-121">Ответ</span><span class="sxs-lookup"><span data-stu-id="d20d6-121">Response</span></span>

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

<span data-ttu-id="d20d6-122">С помощью операторов `select` и `expand` вы можете получить метаданные списка, определения столбцов и элементы списка в одном запросе.</span><span class="sxs-lookup"><span data-stu-id="d20d6-122">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="d20d6-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="d20d6-123">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-multi-expand", "scopes": "sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}?select=id,name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```

#### <a name="response"></a><span data-ttu-id="d20d6-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="d20d6-124">Response</span></span>

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
  "tocPath": "Lists/Get metadata"
} -->
