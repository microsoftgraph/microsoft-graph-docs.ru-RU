---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "Поиск сайтов SharePoint по ключевому слову"
ms.openlocfilehash: 53c9d735ad791bd42fb8b0e1c9b9f412ef469dd8
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="search-for-sites"></a><span data-ttu-id="6d7a5-102">Поиск сайтов</span><span class="sxs-lookup"><span data-stu-id="6d7a5-102">Search for sites</span></span>

<span data-ttu-id="6d7a5-103">Поиск [сайтов][], соответствующих указанным ключевым словам, в клиенте SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6d7a5-103">Search across a SharePoint tenant for [sites][] that match provided keywords.</span></span>

[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="6d7a5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6d7a5-105">Permissions</span></span>

<span data-ttu-id="6d7a5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6d7a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6d7a5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d7a5-108">Permission type</span></span>                        | <span data-ttu-id="6d7a5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d7a5-109">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="6d7a5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d7a5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6d7a5-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d7a5-111">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="6d7a5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d7a5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d7a5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d7a5-113">Not supported.</span></span>
|<span data-ttu-id="6d7a5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d7a5-114">Application</span></span>                            | <span data-ttu-id="6d7a5-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d7a5-115">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="6d7a5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d7a5-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "search-sites", "scopes": "service.sharepoint sites.readwrite.all" } -->

```http
GET /sites?search={query}
```

## <a name="response"></a><span data-ttu-id="6d7a5-117">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d7a5-117">Response</span></span>

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
