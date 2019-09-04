---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Получение элементов из списка SharePoint
localization_priority: Priority
ms.prod: sharepoint
description: Получение коллекции элементов в списке.
doc_type: apiPageType
ms.openlocfilehash: f930d916c3531a7e2c2502d4824834078f129c45
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36728792"
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="1daf9-103">Перечисление элементов списка</span><span class="sxs-lookup"><span data-stu-id="1daf9-103">Enumerate items in a list</span></span>

<span data-ttu-id="1daf9-104">Получение коллекции ресурсов [items][item] из объекта [list][].</span><span class="sxs-lookup"><span data-stu-id="1daf9-104">Get the collection of [items][item] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="1daf9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1daf9-106">Permissions</span></span>

<span data-ttu-id="1daf9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1daf9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1daf9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1daf9-109">Permission type</span></span>      | <span data-ttu-id="1daf9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1daf9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1daf9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1daf9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1daf9-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1daf9-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="1daf9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1daf9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1daf9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1daf9-114">Not supported.</span></span>    |
|<span data-ttu-id="1daf9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1daf9-115">Application</span></span> | <span data-ttu-id="1daf9-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1daf9-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1daf9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1daf9-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="1daf9-118">Пример</span><span class="sxs-lookup"><span data-stu-id="1daf9-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="1daf9-119">Запрос</span><span class="sxs-lookup"><span data-stu-id="1daf9-119">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1daf9-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="1daf9-120">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-items", "scopes": "sites.read.all" } -->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1daf9-121">C#</span><span class="sxs-lookup"><span data-stu-id="1daf9-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-items-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1daf9-122">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1daf9-122">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-items-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1daf9-123">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1daf9-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-items-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1daf9-124">Java</span><span class="sxs-lookup"><span data-stu-id="1daf9-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-items-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1daf9-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="1daf9-125">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.listItem)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
  "tocPath": "ListItem/Enumerate",
  "suppressions": [
  ]
} -->
