---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Получение записи из списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1cb6a51434aba70964321bc99e72603911af3b7b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266180"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="c886c-102">Получение элемента списка</span><span class="sxs-lookup"><span data-stu-id="c886c-102">Get an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c886c-103">Возвращает метаданные [элемента][] в [списке][].</span><span class="sxs-lookup"><span data-stu-id="c886c-103">Returns the metadata for an [item][] in a [list][].</span></span>

[списке]: ../resources/list.md
[list]: ../resources/list.md
[элемента]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="c886c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c886c-106">Permissions</span></span>

<span data-ttu-id="c886c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c886c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c886c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c886c-109">Permission type</span></span>      | <span data-ttu-id="c886c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c886c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c886c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c886c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c886c-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c886c-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c886c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c886c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c886c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c886c-114">Not supported.</span></span>    |
|<span data-ttu-id="c886c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c886c-115">Application</span></span> | <span data-ttu-id="c886c-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c886c-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c886c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c886c-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="c886c-118">Пример</span><span class="sxs-lookup"><span data-stu-id="c886c-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c886c-119">Запрос</span><span class="sxs-lookup"><span data-stu-id="c886c-119">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="c886c-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="c886c-120">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "d14922d8-43e6-4c8a-b029-e35c5b4e0d63",
  "listItemId": 2,
  "fields": {
    "Name": "Widget",
    "Color": "Blue",
    "Quantity": 2357
    }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c886c-121">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="c886c-121">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c886c-122">C#</span><span class="sxs-lookup"><span data-stu-id="c886c-122">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-list-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c886c-123">Javascript</span><span class="sxs-lookup"><span data-stu-id="c886c-123">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-list-item-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c886c-124">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c886c-124">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-list-item-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata",
  "suppressions": [
    "Error: /api-reference/beta/api/listitem-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/listitem-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/listitem-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
