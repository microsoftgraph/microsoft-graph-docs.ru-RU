---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: "Получение элементов из списка SharePoint"
ms.openlocfilehash: ff414159015b4731b76626e309418c32cb6640d4
ms.sourcegitcommit: 339070a20730bc4d363da7eb346d5f3c1e1d6c3e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2017
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="63721-102">Перечисление элементов списка</span><span class="sxs-lookup"><span data-stu-id="63721-102">Enumerate items in a list</span></span>

<span data-ttu-id="63721-103">Получение коллекции ресурсов [item][item] из объекта [list][].</span><span class="sxs-lookup"><span data-stu-id="63721-103">Get the collection of [items][item] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listItem.md

## <a name="permissions"></a><span data-ttu-id="63721-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="63721-105">Permissions</span></span>

<span data-ttu-id="63721-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="63721-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="63721-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63721-108">Permission type</span></span>      | <span data-ttu-id="63721-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="63721-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63721-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63721-110">Delegated (work or school account)</span></span> | <span data-ttu-id="63721-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63721-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="63721-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63721-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63721-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63721-113">Not supported.</span></span>    |
|<span data-ttu-id="63721-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="63721-114">Application</span></span> | <span data-ttu-id="63721-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63721-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="63721-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63721-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="63721-117">Пример</span><span class="sxs-lookup"><span data-stu-id="63721-117">Example</span></span>

#### <a name="request"></a><span data-ttu-id="63721-118">Запрос</span><span class="sxs-lookup"><span data-stu-id="63721-118">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-items" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```

#### <a name="response"></a><span data-ttu-id="63721-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="63721-119">Response</span></span>

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
