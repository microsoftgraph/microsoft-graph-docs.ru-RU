---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Поиск сайтов
description: Поиск сайтов, соответствующих указанным ключевым словам, в клиенте SharePoint.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: a0238bfd462d33aa63f3b9f68be94ae9365a3b90
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509775"
---
# <a name="search-for-sites"></a><span data-ttu-id="6bb1c-103">Поиск сайтов</span><span class="sxs-lookup"><span data-stu-id="6bb1c-103">Search for sites</span></span>

<span data-ttu-id="6bb1c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6bb1c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6bb1c-105">Выполните поиск в клиенте SharePoint для [сайтов][] , которые совпадают с предоставленными ключевыми словами.</span><span class="sxs-lookup"><span data-stu-id="6bb1c-105">Search across a SharePoint tenant for [sites][] that match keywords provided.</span></span>

[сайтов]: ../resources/site.md
[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="6bb1c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6bb1c-107">Permissions</span></span>

<span data-ttu-id="6bb1c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bb1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bb1c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6bb1c-110">Permission type</span></span>                        | <span data-ttu-id="6bb1c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6bb1c-111">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="6bb1c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6bb1c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6bb1c-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bb1c-113">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="6bb1c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6bb1c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6bb1c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6bb1c-115">Not supported.</span></span>
|<span data-ttu-id="6bb1c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6bb1c-116">Application</span></span>                            | <span data-ttu-id="6bb1c-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bb1c-117">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="6bb1c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6bb1c-118">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="6bb1c-119">HTTP</span><span class="sxs-lookup"><span data-stu-id="6bb1c-119">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "search-sites", "scopes": "sites.readwrite.all", "tags": "service.sharepoint" } -->

```msgraph-interactive
GET /sites?search={query}
```
# <a name="c"></a>[<span data-ttu-id="6bb1c-120">C#</span><span class="sxs-lookup"><span data-stu-id="6bb1c-120">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/search-sites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6bb1c-121">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6bb1c-121">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/search-sites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6bb1c-122">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6bb1c-122">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/search-sites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6bb1c-123">Java</span><span class="sxs-lookup"><span data-stu-id="6bb1c-123">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/search-sites-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="6bb1c-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="6bb1c-124">Response</span></span>

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
><span data-ttu-id="6bb1c-125">**Примечание:** Единственное свойство, которое подходит для сортировки, — **createdDateTime**.</span><span class="sxs-lookup"><span data-stu-id="6bb1c-125">**Note:** The only property that works for sorting is **createdDateTime**.</span></span> <span data-ttu-id="6bb1c-126">Фильтр поиска — это поиск с произвольным текстом, который использует несколько свойств при получении результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="6bb1c-126">The search filter is a free text search that uses multiple properties when retrieving the search results.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Search",
  "suppressions": [
  ]
} -->
