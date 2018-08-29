---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Создание списка списков SharePoint на сайте
ms.openlocfilehash: 5d88720ecf3d183f806526364130dd2812874f3c
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2018
ms.locfileid: "23267649"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="d7eed-102">Перечисление списков на сайте</span><span class="sxs-lookup"><span data-stu-id="d7eed-102">Enumerate lists in a site</span></span>

<span data-ttu-id="d7eed-103">Получение коллекции [списков][] для [сайта][].</span><span class="sxs-lookup"><span data-stu-id="d7eed-103">Get the collection of [lists][] for a [site][].</span></span>

[списков]: ../resources/list.md
[lists]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="d7eed-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d7eed-106">Permissions</span></span>

<span data-ttu-id="d7eed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d7eed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d7eed-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7eed-109">Permission type</span></span>      | <span data-ttu-id="d7eed-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7eed-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7eed-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7eed-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d7eed-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7eed-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d7eed-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7eed-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7eed-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7eed-114">Not supported.</span></span>    |
|<span data-ttu-id="d7eed-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7eed-115">Application</span></span> | <span data-ttu-id="d7eed-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7eed-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7eed-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7eed-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="d7eed-118">Пример</span><span class="sxs-lookup"><span data-stu-id="d7eed-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d7eed-119">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7eed-119">Request</span></span>

<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

##### <a name="response"></a><span data-ttu-id="d7eed-120">Ответ</span><span class="sxs-lookup"><span data-stu-id="d7eed-120">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "b57af081-936c-4803-a120-d94887b03864",
      "name": "Documents",
      "createdDateTime": "2016-08-30T08:32:00Z",
      "lastModifiedDateTime": "2016-08-30T08:32:00Z",
      "list": {
        "hidden": false,
        "template": "documentLibrary"
       }
    },
    {
      "id": "1234-112-112-4",
      "name": "MicroFeed",
      "createdDateTime": "2016-08-30T08:32:00Z",
      "lastModifiedDateTime": "2016-08-30T08:32:00Z",
      "list": {
        "hidden": false,
        "template": "genericList"
       }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="d7eed-121">Заметки</span><span class="sxs-lookup"><span data-stu-id="d7eed-121">Remarks</span></span>

<span data-ttu-id="d7eed-122">По умолчанию ресурсы list с аспектом [system][] скрыты.</span><span class="sxs-lookup"><span data-stu-id="d7eed-122">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="d7eed-123">Чтобы перечислить их, включите `system` в оператор `$select`.</span><span class="sxs-lookup"><span data-stu-id="d7eed-123">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemFacet.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Enumerate"
} -->
