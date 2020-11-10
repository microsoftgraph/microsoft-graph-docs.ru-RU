---
author: JeremyKelley
description: Возвращает метаданные элемента в списке.
ms.date: 09/11/2017
title: Получение записи из списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: e66d74493cfb07c0b8ed0071f971037b77f30cf1
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971378"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="c49f5-103">Получение элемента списка</span><span class="sxs-lookup"><span data-stu-id="c49f5-103">Get an item in a list</span></span>

<span data-ttu-id="c49f5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c49f5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c49f5-105">Возвращает метаданные [элемента][] в [списке][].</span><span class="sxs-lookup"><span data-stu-id="c49f5-105">Returns the metadata for an [item][] in a [list][].</span></span>

[списке]: ../resources/list.md
[list]: ../resources/list.md
[элемента]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="c49f5-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c49f5-108">Permissions</span></span>

<span data-ttu-id="c49f5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c49f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c49f5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c49f5-111">Permission type</span></span>      | <span data-ttu-id="c49f5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c49f5-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c49f5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c49f5-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c49f5-114">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c49f5-114">Sites.Read.All, Sites.ReadWrite.All</span></span> |
|<span data-ttu-id="c49f5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c49f5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c49f5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c49f5-116">Not supported.</span></span>    |
|<span data-ttu-id="c49f5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c49f5-117">Application</span></span> | <span data-ttu-id="c49f5-118">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All</span><span class="sxs-lookup"><span data-stu-id="c49f5-118">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All</span></span> |

> <span data-ttu-id="c49f5-119">**Примечание.** : Требуется разрешение для приложений Sites.Manage.All, если в списке SharePoint включены параметры утверждения контента.</span><span class="sxs-lookup"><span data-stu-id="c49f5-119">**Note** : The application permission Sites.Manage.All is required if the SharePoint list has content approval settings turned on.</span></span> <span data-ttu-id="c49f5-120">В противном случае Microsoft Graph не будет получать элементы списка, которые имеют состояние утверждения, отличное от "утверждено".</span><span class="sxs-lookup"><span data-stu-id="c49f5-120">Otherwise, Microsoft Graph won't retrieve list items that have an approval status other than Approved.</span></span>

## <a name="http-request"></a><span data-ttu-id="c49f5-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c49f5-121">HTTP request</span></span>

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET /sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="c49f5-122">Пример</span><span class="sxs-lookup"><span data-stu-id="c49f5-122">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c49f5-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="c49f5-123">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c49f5-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="c49f5-124">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-item" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
# <a name="c"></a>[<span data-ttu-id="c49f5-125">C#</span><span class="sxs-lookup"><span data-stu-id="c49f5-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c49f5-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c49f5-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c49f5-127">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c49f5-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c49f5-128">Java</span><span class="sxs-lookup"><span data-stu-id="c49f5-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c49f5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c49f5-129">Response</span></span>

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


