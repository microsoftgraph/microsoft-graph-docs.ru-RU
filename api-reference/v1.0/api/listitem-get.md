---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Получение записи из списка SharePoint
localization_priority: Priority
ms.openlocfilehash: ab263c074497d43bb03ea7c69748bb1c64fd9425
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881132"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="7e83f-102">Получение элемента списка</span><span class="sxs-lookup"><span data-stu-id="7e83f-102">Get an item in a list</span></span>

<span data-ttu-id="7e83f-103">Возвращает метаданные [элемента][] в [списке][].</span><span class="sxs-lookup"><span data-stu-id="7e83f-103">Returns the metadata for an [item][] in a [list][].</span></span>

[list]: ../resources/list.md
[элемента]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="7e83f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7e83f-106">Permissions</span></span>

<span data-ttu-id="7e83f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e83f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e83f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e83f-109">Permission type</span></span>      | <span data-ttu-id="7e83f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e83f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e83f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e83f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7e83f-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e83f-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7e83f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e83f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e83f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e83f-114">Not supported.</span></span>    |
|<span data-ttu-id="7e83f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7e83f-115">Application</span></span> | <span data-ttu-id="7e83f-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e83f-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e83f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e83f-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="7e83f-118">Пример</span><span class="sxs-lookup"><span data-stu-id="7e83f-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7e83f-119">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e83f-119">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="7e83f-120">Ответ</span><span class="sxs-lookup"><span data-stu-id="7e83f-120">Response</span></span>

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
