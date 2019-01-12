---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Получение элементов из списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5da54754567fdaf3517b551aa41e25e8273d596f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958252"
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="9c1e2-102">Перечисление элементов списка</span><span class="sxs-lookup"><span data-stu-id="9c1e2-102">Enumerate items in a list</span></span>

> <span data-ttu-id="9c1e2-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9c1e2-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9c1e2-105">Получение коллекции ресурсов [item][item] из объекта [list][].</span><span class="sxs-lookup"><span data-stu-id="9c1e2-105">Get the collection of [items][item] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="9c1e2-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9c1e2-107">Permissions</span></span>

<span data-ttu-id="9c1e2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c1e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c1e2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c1e2-110">Permission type</span></span>      | <span data-ttu-id="9c1e2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c1e2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c1e2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c1e2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9c1e2-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c1e2-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="9c1e2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c1e2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c1e2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c1e2-115">Not supported.</span></span>    |
|<span data-ttu-id="9c1e2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9c1e2-116">Application</span></span> | <span data-ttu-id="9c1e2-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c1e2-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c1e2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c1e2-118">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="9c1e2-119">Пример</span><span class="sxs-lookup"><span data-stu-id="9c1e2-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9c1e2-120">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c1e2-120">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-items" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```

#### <a name="response"></a><span data-ttu-id="9c1e2-121">Ответ</span><span class="sxs-lookup"><span data-stu-id="9c1e2-121">Response</span></span>

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
