---
author: JeremyKelley
description: Возвращает метаданные элемента в списке.
ms.date: 09/11/2017
title: Получение записи из списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 25d0a055840055c822814799346136a6bda6c660
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373582"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="2f8a8-103">Получение элемента списка</span><span class="sxs-lookup"><span data-stu-id="2f8a8-103">Get an item in a list</span></span>

<span data-ttu-id="2f8a8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f8a8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f8a8-105">Возвращает метаданные [элемента][] в [списке][].</span><span class="sxs-lookup"><span data-stu-id="2f8a8-105">Returns the metadata for an [item][] in a [list][].</span></span>

[списке]: ../resources/list.md
[list]: ../resources/list.md
[элемента]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="2f8a8-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2f8a8-108">Permissions</span></span>

<span data-ttu-id="2f8a8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f8a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f8a8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f8a8-111">Permission type</span></span>      | <span data-ttu-id="2f8a8-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f8a8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f8a8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f8a8-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2f8a8-114">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f8a8-114">Sites.Read.All, Sites.ReadWrite.All</span></span> |
|<span data-ttu-id="2f8a8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f8a8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f8a8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f8a8-116">Not supported.</span></span>    |
|<span data-ttu-id="2f8a8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f8a8-117">Application</span></span> | <span data-ttu-id="2f8a8-118">Sites. Read. ALL, sites. ReadWrite. ALL, sites. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="2f8a8-118">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All</span></span> |

> <span data-ttu-id="2f8a8-119">**Note**: Application Permission sites. Manage. ALL является обязательным, если для списка SharePoint включены параметры утверждения контента.</span><span class="sxs-lookup"><span data-stu-id="2f8a8-119">**Note**: The application permission Sites.Manage.All is required if the SharePoint list has content approval settings turned on.</span></span> <span data-ttu-id="2f8a8-120">В противном случае Microsoft Graph не будет получать элементы списка, которые имеют состояние утверждения, отличное от "утверждено".</span><span class="sxs-lookup"><span data-stu-id="2f8a8-120">Otherwise, Microsoft Graph won't retrieve list items that have an approval status other than Approved.</span></span>

## <a name="http-request"></a><span data-ttu-id="2f8a8-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f8a8-121">HTTP request</span></span>

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET /sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="2f8a8-122">Пример</span><span class="sxs-lookup"><span data-stu-id="2f8a8-122">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2f8a8-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f8a8-123">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2f8a8-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f8a8-124">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-item" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
# <a name="c"></a>[<span data-ttu-id="2f8a8-125">C#</span><span class="sxs-lookup"><span data-stu-id="2f8a8-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f8a8-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f8a8-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f8a8-127">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f8a8-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2f8a8-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f8a8-128">Response</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata",
  "suppressions": [
  ]
}
-->


