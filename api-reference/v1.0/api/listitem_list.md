---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: "Получение элементов из списка SharePoint"
ms.openlocfilehash: a7f66db11ef201d0ae5afb2cc49887ee10dc89d7
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="68799-102">Перечисление элементов списка</span><span class="sxs-lookup"><span data-stu-id="68799-102">Enumerate items in a list</span></span>

<span data-ttu-id="68799-103">Получение коллекции ресурсов [item][item] из объекта [list][].</span><span class="sxs-lookup"><span data-stu-id="68799-103">Get the collection of [items][item] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listItem.md

## <a name="permissions"></a><span data-ttu-id="68799-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="68799-105">Permissions</span></span>

<span data-ttu-id="68799-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="68799-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="68799-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68799-108">Permission type</span></span>      | <span data-ttu-id="68799-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="68799-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68799-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68799-110">Delegated (work or school account)</span></span> | <span data-ttu-id="68799-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68799-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="68799-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68799-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68799-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68799-113">Not supported.</span></span>    |
|<span data-ttu-id="68799-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68799-114">Application</span></span> | <span data-ttu-id="68799-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68799-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="68799-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68799-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="68799-117">Пример</span><span class="sxs-lookup"><span data-stu-id="68799-117">Example</span></span>

#### <a name="request"></a><span data-ttu-id="68799-118">Запрос</span><span class="sxs-lookup"><span data-stu-id="68799-118">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-items" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```

#### <a name="response"></a><span data-ttu-id="68799-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="68799-119">Response</span></span>

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
