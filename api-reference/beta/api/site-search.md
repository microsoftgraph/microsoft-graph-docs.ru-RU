---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Поиск сайтов SharePoint по ключевому слову
localization_priority: Normal
ms.openlocfilehash: e811dc54f37a55331e0b6c4f25c95f4ce89be142
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821443"
---
# <a name="search-for-sites"></a><span data-ttu-id="c7679-102">Поиск сайтов</span><span class="sxs-lookup"><span data-stu-id="c7679-102">Search for sites</span></span>

> <span data-ttu-id="c7679-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c7679-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7679-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7679-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c7679-105">Поиск [сайтов][], соответствующих указанным ключевым словам, в клиенте SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c7679-105">Search across a SharePoint tenant for [sites][] that match provided keywords.</span></span>

[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="c7679-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c7679-107">Permissions</span></span>

<span data-ttu-id="c7679-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7679-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7679-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7679-110">Permission type</span></span>                        | <span data-ttu-id="c7679-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7679-111">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="c7679-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7679-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c7679-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7679-113">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="c7679-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7679-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7679-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7679-115">Not supported.</span></span>
|<span data-ttu-id="c7679-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7679-116">Application</span></span>                            | <span data-ttu-id="c7679-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7679-117">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="c7679-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7679-118">HTTP request</span></span>

<!-- { "blockType": "request", "name": "search-sites", "scopes": "service.sharepoint sites.readwrite.all" } -->

```http
GET https://graph.microsoft.com/beta/sites?search={query}
```

## <a name="response"></a><span data-ttu-id="c7679-119">Ответ</span><span class="sxs-lookup"><span data-stu-id="c7679-119">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Search"
} -->
