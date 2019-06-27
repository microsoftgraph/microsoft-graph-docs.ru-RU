---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Создание списка списков SharePoint на сайте
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9ea4d8445d9a74a1d557f944427abecbea2a590d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264591"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="66626-102">Перечисление списков на сайте</span><span class="sxs-lookup"><span data-stu-id="66626-102">Enumerate lists in a site</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66626-103">Получение коллекции [списков][] для [сайта][].</span><span class="sxs-lookup"><span data-stu-id="66626-103">Get the collection of [lists][] for a [site][].</span></span>

[списков]: ../resources/list.md
[lists]: ../resources/list.md
[сайта]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="66626-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="66626-106">Permissions</span></span>

<span data-ttu-id="66626-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66626-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66626-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66626-109">Permission type</span></span>      | <span data-ttu-id="66626-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="66626-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66626-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66626-111">Delegated (work or school account)</span></span> | <span data-ttu-id="66626-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66626-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="66626-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66626-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66626-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66626-114">Not supported.</span></span>    |
|<span data-ttu-id="66626-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="66626-115">Application</span></span> | <span data-ttu-id="66626-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66626-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="66626-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66626-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="66626-118">Пример</span><span class="sxs-lookup"><span data-stu-id="66626-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="66626-119">Запрос</span><span class="sxs-lookup"><span data-stu-id="66626-119">Request</span></span>

<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all service.sharepoint" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

##### <a name="response"></a><span data-ttu-id="66626-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="66626-120">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="66626-121">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="66626-121">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="66626-122">C#</span><span class="sxs-lookup"><span data-stu-id="66626-122">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/enum-lists-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="66626-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66626-123">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/enum-lists-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="66626-124">Цель — C</span><span class="sxs-lookup"><span data-stu-id="66626-124">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/enum-lists-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a><span data-ttu-id="66626-125">Комментарии</span><span class="sxs-lookup"><span data-stu-id="66626-125">Remarks</span></span>

<span data-ttu-id="66626-126">По умолчанию ресурсы list с аспектом [system][] скрыты.</span><span class="sxs-lookup"><span data-stu-id="66626-126">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="66626-127">Чтобы перечислить их, включите `system` в оператор `$select`.</span><span class="sxs-lookup"><span data-stu-id="66626-127">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemfacet.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Enumerate",
  "suppressions": [
    "Error: /api-reference/beta/api/list-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/list-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/list-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
