---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: "Получение записи из списка SharePoint"
ms.openlocfilehash: eaa97e169a8fcfdcb676679bb6dedd3a192925d8
ms.sourcegitcommit: 339070a20730bc4d363da7eb346d5f3c1e1d6c3e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2017
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="25342-102">Получение элемента списка</span><span class="sxs-lookup"><span data-stu-id="25342-102">Get an item in a list</span></span>

<span data-ttu-id="25342-103">Возвращает метаданные [элемента][] в [списке][].</span><span class="sxs-lookup"><span data-stu-id="25342-103">Returns the metadata for an [item][] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listItem.md

## <a name="permissions"></a><span data-ttu-id="25342-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="25342-106">Permissions</span></span>

<span data-ttu-id="25342-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="25342-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="25342-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25342-109">Permission type</span></span>      | <span data-ttu-id="25342-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="25342-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25342-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25342-111">Delegated (work or school account)</span></span> | <span data-ttu-id="25342-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25342-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="25342-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25342-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25342-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25342-114">Not supported.</span></span>    |
|<span data-ttu-id="25342-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25342-115">Application</span></span> | <span data-ttu-id="25342-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25342-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="25342-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25342-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="25342-118">Пример</span><span class="sxs-lookup"><span data-stu-id="25342-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="25342-119">Запрос</span><span class="sxs-lookup"><span data-stu-id="25342-119">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="25342-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="25342-120">Response</span></span>

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
