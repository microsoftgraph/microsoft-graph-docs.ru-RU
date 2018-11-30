---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Создание списка списков SharePoint на сайте
ms.openlocfilehash: 4171947eb2a7ac6be18ba385de39c5befd762f26
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027454"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="1f1e6-102">Перечисление списков на сайте</span><span class="sxs-lookup"><span data-stu-id="1f1e6-102">Enumerate lists in a site</span></span>

<span data-ttu-id="1f1e6-103">Получение коллекции [списков][] для [сайта][].</span><span class="sxs-lookup"><span data-stu-id="1f1e6-103">Get the collection of [lists][] for a [site][].</span></span>

[списков]: ../resources/list.md
[lists]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="1f1e6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1f1e6-106">Permissions</span></span>

<span data-ttu-id="1f1e6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f1e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f1e6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f1e6-109">Permission type</span></span>      | <span data-ttu-id="1f1e6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f1e6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f1e6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f1e6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1f1e6-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f1e6-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="1f1e6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f1e6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f1e6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f1e6-114">Not supported.</span></span>    |
|<span data-ttu-id="1f1e6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f1e6-115">Application</span></span> | <span data-ttu-id="1f1e6-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f1e6-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f1e6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f1e6-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="1f1e6-118">Пример</span><span class="sxs-lookup"><span data-stu-id="1f1e6-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="1f1e6-119">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f1e6-119">Request</span></span>

<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

##### <a name="response"></a><span data-ttu-id="1f1e6-120">Ответ</span><span class="sxs-lookup"><span data-stu-id="1f1e6-120">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="1f1e6-121">Заметки</span><span class="sxs-lookup"><span data-stu-id="1f1e6-121">Remarks</span></span>

<span data-ttu-id="1f1e6-122">По умолчанию ресурсы list с аспектом [system][] скрыты.</span><span class="sxs-lookup"><span data-stu-id="1f1e6-122">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="1f1e6-123">Чтобы перечислить их, включите `system` в оператор `$select`.</span><span class="sxs-lookup"><span data-stu-id="1f1e6-123">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Enumerate"
} -->
