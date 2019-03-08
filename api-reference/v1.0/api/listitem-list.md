---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Получение элементов из списка SharePoint
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 358fc16065074e3b0b2f8b1d19e7a5c43a4126e6
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480497"
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="74a02-102">Перечисление элементов списка</span><span class="sxs-lookup"><span data-stu-id="74a02-102">Enumerate items in a list</span></span>

<span data-ttu-id="74a02-103">Получение коллекции ресурсов [item][item] из объекта [list][].</span><span class="sxs-lookup"><span data-stu-id="74a02-103">Get the collection of [items][item] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="74a02-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="74a02-105">Permissions</span></span>

<span data-ttu-id="74a02-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74a02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74a02-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74a02-108">Permission type</span></span>      | <span data-ttu-id="74a02-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="74a02-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74a02-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74a02-110">Delegated (work or school account)</span></span> | <span data-ttu-id="74a02-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74a02-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="74a02-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74a02-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74a02-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74a02-113">Not supported.</span></span>    |
|<span data-ttu-id="74a02-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74a02-114">Application</span></span> | <span data-ttu-id="74a02-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74a02-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="74a02-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74a02-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="74a02-117">Пример</span><span class="sxs-lookup"><span data-stu-id="74a02-117">Example</span></span>

#### <a name="request"></a><span data-ttu-id="74a02-118">Запрос</span><span class="sxs-lookup"><span data-stu-id="74a02-118">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-items", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```

#### <a name="response"></a><span data-ttu-id="74a02-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="74a02-119">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.listItem)", "truncated": true } -->

```json
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
  "tocPath": "ListItem/Enumerate"
} -->
