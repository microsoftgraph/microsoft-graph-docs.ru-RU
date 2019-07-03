---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Получение элементов из списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 640702bc65ef36f50a0b548e0e10720a71a2c807
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35449150"
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="f8bb4-102">Перечисление элементов списка</span><span class="sxs-lookup"><span data-stu-id="f8bb4-102">Enumerate items in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8bb4-103">Получение коллекции ресурсов [item][item] из объекта [list][].</span><span class="sxs-lookup"><span data-stu-id="f8bb4-103">Get the collection of [items][item] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="f8bb4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f8bb4-105">Permissions</span></span>

<span data-ttu-id="f8bb4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8bb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8bb4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8bb4-108">Permission type</span></span>      | <span data-ttu-id="f8bb4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8bb4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8bb4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8bb4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f8bb4-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8bb4-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f8bb4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8bb4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8bb4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8bb4-113">Not supported.</span></span>    |
|<span data-ttu-id="f8bb4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f8bb4-114">Application</span></span> | <span data-ttu-id="f8bb4-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8bb4-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8bb4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8bb4-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="f8bb4-117">Пример</span><span class="sxs-lookup"><span data-stu-id="f8bb4-117">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f8bb4-118">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8bb4-118">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f8bb4-119">HTTP</span><span class="sxs-lookup"><span data-stu-id="f8bb4-119">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-items" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f8bb4-120">C#</span><span class="sxs-lookup"><span data-stu-id="f8bb4-120">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-items-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f8bb4-121">Javascript</span><span class="sxs-lookup"><span data-stu-id="f8bb4-121">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-items-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f8bb4-122">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f8bb4-122">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-items-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f8bb4-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8bb4-123">Response</span></span>

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
