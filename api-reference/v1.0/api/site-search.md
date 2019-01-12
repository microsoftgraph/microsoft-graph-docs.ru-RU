---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Поиск сайтов SharePoint по ключевому слову
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: c73b1e5650d14e55842aba83069f27cb98e6a1ff
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917379"
---
# <a name="search-for-sites"></a><span data-ttu-id="b95f0-102">Поиск сайтов</span><span class="sxs-lookup"><span data-stu-id="b95f0-102">Search for sites</span></span>

<span data-ttu-id="b95f0-103">Поиск [сайтов][], соответствующих указанным ключевым словам, в клиенте SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b95f0-103">Search across a SharePoint tenant for [sites][] that match provided keywords.</span></span>

[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="b95f0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b95f0-105">Permissions</span></span>

<span data-ttu-id="b95f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b95f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b95f0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b95f0-108">Permission type</span></span>                        | <span data-ttu-id="b95f0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b95f0-109">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="b95f0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b95f0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b95f0-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b95f0-111">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="b95f0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b95f0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b95f0-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b95f0-113">Not supported.</span></span>
|<span data-ttu-id="b95f0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b95f0-114">Application</span></span>                            | <span data-ttu-id="b95f0-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b95f0-115">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="b95f0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b95f0-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "search-sites", "scopes": "sites.readwrite.all", "tags": "service.sharepoint" } -->

```http
GET /sites?search={query}
```

## <a name="response"></a><span data-ttu-id="b95f0-117">Ответ</span><span class="sxs-lookup"><span data-stu-id="b95f0-117">Response</span></span>

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
