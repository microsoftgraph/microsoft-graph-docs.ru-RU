---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Получение записи из списка SharePoint
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 36af0d07de3fe217b69b810700e830f74edda2c7
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33598232"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="93ca4-102">Получение элемента списка</span><span class="sxs-lookup"><span data-stu-id="93ca4-102">Get an item in a list</span></span>

<span data-ttu-id="93ca4-103">Возвращает метаданные [элемента][] в [списке][].</span><span class="sxs-lookup"><span data-stu-id="93ca4-103">Returns the metadata for an [item][] in a [list][].</span></span>

[списке]: ../resources/list.md
[list]: ../resources/list.md
[элемента]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="93ca4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="93ca4-106">Permissions</span></span>

<span data-ttu-id="93ca4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93ca4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93ca4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93ca4-109">Permission type</span></span>      | <span data-ttu-id="93ca4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="93ca4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93ca4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93ca4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="93ca4-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93ca4-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="93ca4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93ca4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93ca4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93ca4-114">Not supported.</span></span>    |
|<span data-ttu-id="93ca4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="93ca4-115">Application</span></span> | <span data-ttu-id="93ca4-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93ca4-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="93ca4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93ca4-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="93ca4-118">Пример</span><span class="sxs-lookup"><span data-stu-id="93ca4-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="93ca4-119">Запрос</span><span class="sxs-lookup"><span data-stu-id="93ca4-119">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="93ca4-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="93ca4-120">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "5",
  "fields": {
    "Name": "Widget",
    "Color": "Blue",
    "Quantity": 2357
    }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="93ca4-121">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="93ca4-121">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="93ca4-122">Языках</span><span class="sxs-lookup"><span data-stu-id="93ca4-122">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-list-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="93ca4-123">Язык</span><span class="sxs-lookup"><span data-stu-id="93ca4-123">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-list-item-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata",
  "suppressions": [
    "Error: /api-reference/v1.0/api/listitem-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/listitem-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
