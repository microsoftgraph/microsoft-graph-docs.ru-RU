---
author: JeremyKelley
description: Выполните поиск в клиенте SharePoint для сайтов, которые совпадают с предоставленными ключевыми словами.
ms.date: 09/10/2017
title: Поиск сайтов SharePoint по ключевому слову
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: dbc66bc734d4ef0a47e30ce1e967918e964489a0
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36724535"
---
# <a name="search-for-sites"></a><span data-ttu-id="79dfa-103">Поиск сайтов</span><span class="sxs-lookup"><span data-stu-id="79dfa-103">Search for sites</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79dfa-104">Выполните поиск в клиенте SharePoint для [сайтов][] , которые совпадают с предоставленными ключевыми словами.</span><span class="sxs-lookup"><span data-stu-id="79dfa-104">Search across a SharePoint tenant for [sites][] that match keywords provided.</span></span>

[сайтов]: ../resources/site.md
[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="79dfa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="79dfa-106">Permissions</span></span>

<span data-ttu-id="79dfa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79dfa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79dfa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79dfa-109">Permission type</span></span>                        | <span data-ttu-id="79dfa-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79dfa-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="79dfa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79dfa-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="79dfa-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79dfa-112">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="79dfa-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79dfa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79dfa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79dfa-114">Not supported.</span></span>
|<span data-ttu-id="79dfa-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79dfa-115">Application</span></span>                            | <span data-ttu-id="79dfa-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79dfa-116">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="79dfa-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79dfa-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="79dfa-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="79dfa-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "search-sites", "scopes": "service.sharepoint sites.readwrite.all" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites?search={query}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="79dfa-119">C#</span><span class="sxs-lookup"><span data-stu-id="79dfa-119">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/search-sites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="79dfa-120">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79dfa-120">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/search-sites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="79dfa-121">Цель — C</span><span class="sxs-lookup"><span data-stu-id="79dfa-121">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/search-sites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="79dfa-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="79dfa-122">Response</span></span>

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
><span data-ttu-id="79dfa-123">**Примечание:** Единственное свойство, которое подходит для сортировки, — **createdDateTime**.</span><span class="sxs-lookup"><span data-stu-id="79dfa-123">**Note:** The only property that works for sorting is **createdDateTime**.</span></span> <span data-ttu-id="79dfa-124">Фильтр поиска — это поиск с произвольным текстом, который использует несколько свойств при получении результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="79dfa-124">The search filter is a free text search that uses multiple properties when retrieving the search results.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Search",
  "suppressions": [
  ]
}
-->
