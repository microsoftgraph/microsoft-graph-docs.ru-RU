---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Получение записи из списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ad77cbc3ccaa393cbb9717a7c9cfabef64099d37
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936272"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="31cb2-102">Получение элемента списка</span><span class="sxs-lookup"><span data-stu-id="31cb2-102">Get an item in a list</span></span>

> <span data-ttu-id="31cb2-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="31cb2-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31cb2-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31cb2-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="31cb2-105">Возвращает метаданные [элемента][] в [списке][].</span><span class="sxs-lookup"><span data-stu-id="31cb2-105">Returns the metadata for an [item][] in a [list][].</span></span>

[list]: ../resources/list.md
[элемента]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="31cb2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="31cb2-108">Permissions</span></span>

<span data-ttu-id="31cb2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31cb2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31cb2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31cb2-111">Permission type</span></span>      | <span data-ttu-id="31cb2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="31cb2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31cb2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31cb2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="31cb2-114">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31cb2-114">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="31cb2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31cb2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31cb2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31cb2-116">Not supported.</span></span>    |
|<span data-ttu-id="31cb2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="31cb2-117">Application</span></span> | <span data-ttu-id="31cb2-118">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31cb2-118">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="31cb2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31cb2-119">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="31cb2-120">Пример</span><span class="sxs-lookup"><span data-stu-id="31cb2-120">Example</span></span>

##### <a name="request"></a><span data-ttu-id="31cb2-121">Запрос</span><span class="sxs-lookup"><span data-stu-id="31cb2-121">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="31cb2-122">Ответ</span><span class="sxs-lookup"><span data-stu-id="31cb2-122">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata"
} -->
