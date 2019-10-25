---
author: JeremyKelley
description: Получение коллекции элементов в списке.
ms.date: 09/11/2017
title: Получение элементов из списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 1cd2bdf856f89068708ac670c239b6d27fd7ded2
ms.sourcegitcommit: bbef506636bce5b72351ee3834123771c301b1b1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/25/2019
ms.locfileid: "37726306"
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="3c19a-103">Перечисление элементов списка</span><span class="sxs-lookup"><span data-stu-id="3c19a-103">Enumerate items in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c19a-104">Получение коллекции ресурсов [items][item] из объекта [list][].</span><span class="sxs-lookup"><span data-stu-id="3c19a-104">Get the collection of [items][item] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="3c19a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3c19a-106">Permissions</span></span>

<span data-ttu-id="3c19a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c19a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c19a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c19a-109">Permission type</span></span>      | <span data-ttu-id="3c19a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c19a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c19a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c19a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3c19a-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c19a-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3c19a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c19a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c19a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c19a-114">Not supported.</span></span>    |
|<span data-ttu-id="3c19a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c19a-115">Application</span></span> | <span data-ttu-id="3c19a-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c19a-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c19a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c19a-117">HTTP request</span></span>

```http
GET /sites/{site-id}/lists/{list-id}/items
GET /sites/{site-id}/lists/{list-id}/items?expand=fields
GET /sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="3c19a-118">Пример</span><span class="sxs-lookup"><span data-stu-id="3c19a-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3c19a-119">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c19a-119">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3c19a-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c19a-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-items" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3c19a-121">C#</span><span class="sxs-lookup"><span data-stu-id="3c19a-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-items-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3c19a-122">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c19a-122">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-items-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3c19a-123">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c19a-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-items-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3c19a-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c19a-124">Response</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Enumerate",
  "suppressions": [
  ]
}
-->
