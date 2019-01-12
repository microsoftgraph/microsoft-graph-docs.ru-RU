---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Получение списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f9744ec25d852359246e84c83ba3bd1dec92ff17
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927956"
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="05eb5-102">Получение метаданных списка</span><span class="sxs-lookup"><span data-stu-id="05eb5-102">Get metadata for a list</span></span>

> <span data-ttu-id="05eb5-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="05eb5-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="05eb5-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05eb5-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="05eb5-105">Возвращает метаданные для [списка][].</span><span class="sxs-lookup"><span data-stu-id="05eb5-105">Returns the metadata for a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="05eb5-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="05eb5-107">Permissions</span></span>

<span data-ttu-id="05eb5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05eb5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05eb5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05eb5-110">Permission type</span></span>      | <span data-ttu-id="05eb5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="05eb5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05eb5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05eb5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="05eb5-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05eb5-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="05eb5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05eb5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05eb5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05eb5-115">Not supported.</span></span>    |
|<span data-ttu-id="05eb5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05eb5-116">Application</span></span> | <span data-ttu-id="05eb5-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05eb5-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="05eb5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05eb5-118">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="05eb5-119">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="05eb5-119">Request body</span></span>

<span data-ttu-id="05eb5-120">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="05eb5-120">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="05eb5-121">Пример</span><span class="sxs-lookup"><span data-stu-id="05eb5-121">Example</span></span>

#### <a name="request"></a><span data-ttu-id="05eb5-122">Запрос</span><span class="sxs-lookup"><span data-stu-id="05eb5-122">Request</span></span>

<!-- { "blockType": "request", "name": "get-list" } -->

```http
GET /sites/{site-id}/lists/{list-id}
```

#### <a name="response"></a><span data-ttu-id="05eb5-123">Ответ</span><span class="sxs-lookup"><span data-stu-id="05eb5-123">Response</span></span>

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

<span data-ttu-id="05eb5-124">С помощью операторов `select` и `expand` вы можете получить метаданные списка, определения столбцов и элементы списка в одном запросе.</span><span class="sxs-lookup"><span data-stu-id="05eb5-124">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="05eb5-125">Запрос</span><span class="sxs-lookup"><span data-stu-id="05eb5-125">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-multi-expand" } -->

```http
GET /sites/{site-id}/lists/{list-id}?select=name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```

#### <a name="response"></a><span data-ttu-id="05eb5-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="05eb5-126">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Get metadata"
} -->
