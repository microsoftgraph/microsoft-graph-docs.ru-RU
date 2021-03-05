---
author: JeremyKelley
ms.date: 09/11/2017
title: Получение элементов из списка SharePoint
localization_priority: Priority
ms.prod: sharepoint
description: Получение коллекции элементов в списке.
doc_type: apiPageType
ms.openlocfilehash: d81df961f5f7ebe311e8082ac39fc0430cb40502
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473737"
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="b7cb6-103">Перечисление элементов списка</span><span class="sxs-lookup"><span data-stu-id="b7cb6-103">Enumerate items in a list</span></span>

<span data-ttu-id="b7cb6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7cb6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b7cb6-105">Получение коллекции ресурсов [items][item] из объекта [list][].</span><span class="sxs-lookup"><span data-stu-id="b7cb6-105">Get the collection of [items][item] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="b7cb6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b7cb6-107">Permissions</span></span>

<span data-ttu-id="b7cb6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7cb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7cb6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7cb6-110">Permission type</span></span>      | <span data-ttu-id="b7cb6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7cb6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7cb6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7cb6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b7cb6-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7cb6-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b7cb6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7cb6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7cb6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7cb6-115">Not supported.</span></span>    |
|<span data-ttu-id="b7cb6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7cb6-116">Application</span></span> | <span data-ttu-id="b7cb6-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7cb6-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7cb6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7cb6-118">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="b7cb6-119">Пример</span><span class="sxs-lookup"><span data-stu-id="b7cb6-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b7cb6-120">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7cb6-120">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b7cb6-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="b7cb6-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-items", "scopes": "sites.read.all" } -->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```
# <a name="c"></a>[<span data-ttu-id="b7cb6-122">C#</span><span class="sxs-lookup"><span data-stu-id="b7cb6-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-items-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b7cb6-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b7cb6-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-items-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b7cb6-124">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b7cb6-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-items-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b7cb6-125">Java</span><span class="sxs-lookup"><span data-stu-id="b7cb6-125">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-items-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b7cb6-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7cb6-126">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.listItem)", "truncated": true } -->

```http
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

