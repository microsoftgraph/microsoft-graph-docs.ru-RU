---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Поиск сайтов SharePoint по ключевому слову
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a5594eb71fd4193756d3d07af82bbd7bbe4a7ea3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335838"
---
# <a name="search-for-sites"></a><span data-ttu-id="1880d-102">Поиск сайтов</span><span class="sxs-lookup"><span data-stu-id="1880d-102">Search for sites</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1880d-103">Выполните поиск в клиенте SharePoint для [сайтов][] , которые совпадают с предоставленными ключевыми словами.</span><span class="sxs-lookup"><span data-stu-id="1880d-103">Search across a SharePoint tenant for [sites][] that match keywords provided.</span></span>

[сайтов]: ../resources/site.md
[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="1880d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1880d-105">Permissions</span></span>

<span data-ttu-id="1880d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1880d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1880d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1880d-108">Permission type</span></span>                        | <span data-ttu-id="1880d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1880d-109">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="1880d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1880d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1880d-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1880d-111">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="1880d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1880d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1880d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1880d-113">Not supported.</span></span>
|<span data-ttu-id="1880d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1880d-114">Application</span></span>                            | <span data-ttu-id="1880d-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1880d-115">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="1880d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1880d-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "search-sites", "scopes": "service.sharepoint sites.readwrite.all" } -->

```http
GET https://graph.microsoft.com/beta/sites?search={query}
```

## <a name="response"></a><span data-ttu-id="1880d-117">Отклик</span><span class="sxs-lookup"><span data-stu-id="1880d-117">Response</span></span>

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
><span data-ttu-id="1880d-118">**Примечание:** Единственное свойство, которое подходит для сортировки, — **createdDateTime**.</span><span class="sxs-lookup"><span data-stu-id="1880d-118">**Note:** The only property that works for sorting is **createdDateTime**.</span></span> <span data-ttu-id="1880d-119">Фильтр поиска — это поиск с произвольным текстом, который использует несколько свойств при получении результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="1880d-119">The search filter is a free text search that uses multiple properties when retrieving the search results.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Search",
  "suppressions": []
}
-->
