---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Получение элементов из списка SharePoint
localization_priority: Priority
ms.prod: sharepoint
description: Получение коллекции элементов в списке.
doc_type: apiPageType
ms.openlocfilehash: 49ca1090411a1a53be3db193821c14df51edef61
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023117"
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="cf18b-103">Перечисление элементов списка</span><span class="sxs-lookup"><span data-stu-id="cf18b-103">Enumerate items in a list</span></span>

<span data-ttu-id="cf18b-104">Получение коллекции ресурсов [items][item] из объекта [list][].</span><span class="sxs-lookup"><span data-stu-id="cf18b-104">Get the collection of [items][item] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="cf18b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cf18b-106">Permissions</span></span>

<span data-ttu-id="cf18b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf18b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf18b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf18b-109">Permission type</span></span>      | <span data-ttu-id="cf18b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf18b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf18b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf18b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cf18b-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf18b-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="cf18b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf18b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf18b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf18b-114">Not supported.</span></span>    |
|<span data-ttu-id="cf18b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf18b-115">Application</span></span> | <span data-ttu-id="cf18b-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf18b-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf18b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf18b-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="cf18b-118">Пример</span><span class="sxs-lookup"><span data-stu-id="cf18b-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="cf18b-119">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf18b-119">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="cf18b-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf18b-120">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-items", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cf18b-121">C#</span><span class="sxs-lookup"><span data-stu-id="cf18b-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-items-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cf18b-122">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf18b-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-items-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cf18b-123">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cf18b-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-items-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cf18b-124">Java</span><span class="sxs-lookup"><span data-stu-id="cf18b-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-items-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cf18b-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf18b-125">Response</span></span>

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
