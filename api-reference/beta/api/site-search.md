---
author: JeremyKelley
description: Выполните поиск в клиенте SharePoint для сайтов, которые совпадают с предоставленными ключевыми словами.
ms.date: 09/10/2017
title: Поиск сайтов SharePoint по ключевому слову
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: e43b63e42e5c4f5be806e13d025a9ebd9ce5c03c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991235"
---
# <a name="search-for-sites"></a><span data-ttu-id="dd755-103">Поиск сайтов</span><span class="sxs-lookup"><span data-stu-id="dd755-103">Search for sites</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd755-104">Выполните поиск в клиенте SharePoint для [сайтов][] , которые совпадают с предоставленными ключевыми словами.</span><span class="sxs-lookup"><span data-stu-id="dd755-104">Search across a SharePoint tenant for [sites][] that match keywords provided.</span></span>

[сайтов]: ../resources/site.md
[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="dd755-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd755-106">Permissions</span></span>

<span data-ttu-id="dd755-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd755-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd755-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd755-109">Permission type</span></span>                        | <span data-ttu-id="dd755-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd755-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="dd755-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd755-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dd755-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd755-112">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="dd755-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd755-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd755-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd755-114">Not supported.</span></span>
|<span data-ttu-id="dd755-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd755-115">Application</span></span>                            | <span data-ttu-id="dd755-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd755-116">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="dd755-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd755-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dd755-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd755-118">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "search-sites", "scopes": "service.sharepoint sites.readwrite.all" } -->

```http
GET https://graph.microsoft.com/beta/sites?search={query}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dd755-119">C#</span><span class="sxs-lookup"><span data-stu-id="dd755-119">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/search-sites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dd755-120">Javascript</span><span class="sxs-lookup"><span data-stu-id="dd755-120">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/search-sites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dd755-121">Цель — C</span><span class="sxs-lookup"><span data-stu-id="dd755-121">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/search-sites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dd755-122">Java</span><span class="sxs-lookup"><span data-stu-id="dd755-122">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/search-sites-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="dd755-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd755-123">Response</span></span>

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
><span data-ttu-id="dd755-124">**Примечание:** Единственное свойство, которое подходит для сортировки, — **createdDateTime**.</span><span class="sxs-lookup"><span data-stu-id="dd755-124">**Note:** The only property that works for sorting is **createdDateTime**.</span></span> <span data-ttu-id="dd755-125">Фильтр поиска — это поиск с произвольным текстом, который использует несколько свойств при получении результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="dd755-125">The search filter is a free text search that uses multiple properties when retrieving the search results.</span></span>

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
