---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Получение записи из списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1f50d31dd58bb0839113a1954fb16f0d824da5f9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333495"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="efebc-102">Получение элемента списка</span><span class="sxs-lookup"><span data-stu-id="efebc-102">Get an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efebc-103">Возвращает метаданные [элемента][] в [списке][].</span><span class="sxs-lookup"><span data-stu-id="efebc-103">Returns the metadata for an [item][] in a [list][].</span></span>

[списке]: ../resources/list.md
[list]: ../resources/list.md
[элемента]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="efebc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="efebc-106">Permissions</span></span>

<span data-ttu-id="efebc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efebc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efebc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="efebc-109">Permission type</span></span>      | <span data-ttu-id="efebc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="efebc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="efebc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="efebc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="efebc-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efebc-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="efebc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="efebc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="efebc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efebc-114">Not supported.</span></span>    |
|<span data-ttu-id="efebc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="efebc-115">Application</span></span> | <span data-ttu-id="efebc-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efebc-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="efebc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="efebc-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="efebc-118">Пример</span><span class="sxs-lookup"><span data-stu-id="efebc-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="efebc-119">Запрос</span><span class="sxs-lookup"><span data-stu-id="efebc-119">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="efebc-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="efebc-120">Response</span></span>

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
  "suppressions": []
}
-->
