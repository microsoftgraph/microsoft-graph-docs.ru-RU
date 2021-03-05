---
author: JeremyKelley
description: Возвращает метаданные элемента в списке.
ms.date: 09/11/2017
title: Получение записи из списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: d3d2e431bfa73e92fd99a146ad9820b46d21b4dc
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475858"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="a629e-103">Получение элемента списка</span><span class="sxs-lookup"><span data-stu-id="a629e-103">Get an item in a list</span></span>

<span data-ttu-id="a629e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a629e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a629e-105">Возвращает метаданные [элемента][] в [списке][].</span><span class="sxs-lookup"><span data-stu-id="a629e-105">Returns the metadata for an [item][] in a [list][].</span></span>

[списке]: ../resources/list.md
[list]: ../resources/list.md
[элемента]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="a629e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a629e-108">Permissions</span></span>

<span data-ttu-id="a629e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a629e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a629e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a629e-111">Permission type</span></span>      | <span data-ttu-id="a629e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a629e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a629e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a629e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a629e-114">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a629e-114">Sites.Read.All, Sites.ReadWrite.All</span></span> |
|<span data-ttu-id="a629e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a629e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a629e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a629e-116">Not supported.</span></span>    |
|<span data-ttu-id="a629e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a629e-117">Application</span></span> | <span data-ttu-id="a629e-118">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All</span><span class="sxs-lookup"><span data-stu-id="a629e-118">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All</span></span> |

> <span data-ttu-id="a629e-119">**Примечание.**: Требуется разрешение для приложений Sites.Manage.All, если в списке SharePoint включены параметры утверждения контента.</span><span class="sxs-lookup"><span data-stu-id="a629e-119">**Note**: The application permission Sites.Manage.All is required if the SharePoint list has content approval settings turned on.</span></span> <span data-ttu-id="a629e-120">В противном случае Microsoft Graph не будет получать элементы списков, которые имеют статус утверждения, кроме утвержденных.</span><span class="sxs-lookup"><span data-stu-id="a629e-120">Otherwise, Microsoft Graph won't retrieve list items that have an approval status other than Approved.</span></span>

## <a name="http-request"></a><span data-ttu-id="a629e-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a629e-121">HTTP request</span></span>

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET /sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="a629e-122">Пример</span><span class="sxs-lookup"><span data-stu-id="a629e-122">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a629e-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="a629e-123">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a629e-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="a629e-124">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-item" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
# <a name="c"></a>[<span data-ttu-id="a629e-125">C#</span><span class="sxs-lookup"><span data-stu-id="a629e-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a629e-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a629e-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a629e-127">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a629e-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a629e-128">Java</span><span class="sxs-lookup"><span data-stu-id="a629e-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a629e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a629e-129">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```http
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


