---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Поиск сайтов
description: Выполните поиск в клиенте SharePoint для сайтов, которые совпадают с предоставленными ключевыми словами.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 310d7d6a0dedaec149fff84133c8f1fa9f853f4d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273159"
---
# <a name="search-for-sites"></a><span data-ttu-id="d05fc-103">Поиск сайтов</span><span class="sxs-lookup"><span data-stu-id="d05fc-103">Search for sites</span></span>

<span data-ttu-id="d05fc-104">Выполните поиск в клиенте SharePoint для [сайтов][] , которые совпадают с предоставленными ключевыми словами.</span><span class="sxs-lookup"><span data-stu-id="d05fc-104">Search across a SharePoint tenant for [sites][] that match keywords provided.</span></span>

[сайтов]: ../resources/site.md
[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="d05fc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d05fc-106">Permissions</span></span>

<span data-ttu-id="d05fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d05fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d05fc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d05fc-109">Permission type</span></span>                        | <span data-ttu-id="d05fc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d05fc-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="d05fc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d05fc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d05fc-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d05fc-112">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="d05fc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d05fc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d05fc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d05fc-114">Not supported.</span></span>
|<span data-ttu-id="d05fc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d05fc-115">Application</span></span>                            | <span data-ttu-id="d05fc-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d05fc-116">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="d05fc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d05fc-117">HTTP request</span></span>

<!-- { "blockType": "request", "name": "search-sites", "scopes": "sites.readwrite.all", "tags": "service.sharepoint" } -->

```http
GET /sites?search={query}
```

## <a name="response"></a><span data-ttu-id="d05fc-118">Отклик</span><span class="sxs-lookup"><span data-stu-id="d05fc-118">Response</span></span>

<!-- { "blockType": "response", "@type": "Collection(microsoft.graph.site)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740",
      "name": "Team A Site",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/siteA"
    },
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
      "name": "Team B Site",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/siteB"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d05fc-119">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="d05fc-119">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d05fc-120">C#</span><span class="sxs-lookup"><span data-stu-id="d05fc-120">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/search-sites-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d05fc-121">Javascript</span><span class="sxs-lookup"><span data-stu-id="d05fc-121">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/search-sites-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d05fc-122">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d05fc-122">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/search-sites-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
><span data-ttu-id="d05fc-123">**Примечание:** Единственное свойство, которое подходит для сортировки, — **createdDateTime**.</span><span class="sxs-lookup"><span data-stu-id="d05fc-123">**Note:** The only property that works for sorting is **createdDateTime**.</span></span> <span data-ttu-id="d05fc-124">Фильтр поиска — это поиск с произвольным текстом, который использует несколько свойств при получении результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="d05fc-124">The search filter is a free text search that uses multiple properties when retrieving the search results.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Search",
  "suppressions": [
    "Error: /api-reference/v1.0/api/site-search.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/site-search.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/site-search.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
