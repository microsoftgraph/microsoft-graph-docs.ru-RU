---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Получение записи из списка SharePoint
ms.openlocfilehash: b650507e8a8bc74b8156117f765220712a2a46d2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026179"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="bbbf3-102">Получение элемента списка</span><span class="sxs-lookup"><span data-stu-id="bbbf3-102">Get an item in a list</span></span>

<span data-ttu-id="bbbf3-103">Возвращает метаданные [элемента][] в [списке][].</span><span class="sxs-lookup"><span data-stu-id="bbbf3-103">Returns the metadata for an [item][] in a [list][].</span></span>

[list]: ../resources/list.md
[элемента]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="bbbf3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bbbf3-106">Permissions</span></span>

<span data-ttu-id="bbbf3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbbf3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbbf3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bbbf3-109">Permission type</span></span>      | <span data-ttu-id="bbbf3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bbbf3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bbbf3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bbbf3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bbbf3-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbbf3-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="bbbf3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bbbf3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbbf3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbbf3-114">Not supported.</span></span>    |
|<span data-ttu-id="bbbf3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bbbf3-115">Application</span></span> | <span data-ttu-id="bbbf3-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbbf3-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bbbf3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bbbf3-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="bbbf3-118">Пример</span><span class="sxs-lookup"><span data-stu-id="bbbf3-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bbbf3-119">Запрос</span><span class="sxs-lookup"><span data-stu-id="bbbf3-119">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="bbbf3-120">Ответ</span><span class="sxs-lookup"><span data-stu-id="bbbf3-120">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata"
} -->
