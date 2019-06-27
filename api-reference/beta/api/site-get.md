---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Получение сайта SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: adf20d242dec40dd2981b90f725fb18980e1a60d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271584"
---
# <a name="get-a-site-resource"></a><span data-ttu-id="05a20-102">Получение ресурса site</span><span class="sxs-lookup"><span data-stu-id="05a20-102">Get a site resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05a20-p101">Получение свойств и отношений ресурса [site][]. Ресурс **site** представляет сайт группы в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="05a20-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="05a20-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="05a20-106">Permissions</span></span>

<span data-ttu-id="05a20-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05a20-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05a20-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05a20-109">Permission type</span></span>      | <span data-ttu-id="05a20-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="05a20-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05a20-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05a20-111">Delegated (work or school account)</span></span> | <span data-ttu-id="05a20-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05a20-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="05a20-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05a20-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05a20-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05a20-114">Not supported.</span></span>    |
|<span data-ttu-id="05a20-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05a20-115">Application</span></span> | <span data-ttu-id="05a20-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05a20-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-the-tenants-root-site"></a><span data-ttu-id="05a20-117">Получение корневого сайта клиента</span><span class="sxs-lookup"><span data-stu-id="05a20-117">Get the tenant's root site</span></span>

<span data-ttu-id="05a20-118">Чтобы получить доступ к корневому сайту SharePoint внутри клиента, создайте следующие запросы:</span><span class="sxs-lookup"><span data-stu-id="05a20-118">To access the root SharePoint site within a tenant:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a><span data-ttu-id="05a20-119">Использование относительного URL-адреса сервера для доступа к сайту</span><span class="sxs-lookup"><span data-stu-id="05a20-119">Access a site by server-relative URL</span></span>

<span data-ttu-id="05a20-120">Если у вас есть относительный URL-адрес сервера для ресурса **site**, можно создать следующий запрос:</span><span class="sxs-lookup"><span data-stu-id="05a20-120">If you have the server-relative URL for a **site** resource, you can construct a request as follows:</span></span>

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a><span data-ttu-id="05a20-121">Доступ к сайту группы для группы</span><span class="sxs-lookup"><span data-stu-id="05a20-121">Access a group team site</span></span>

<span data-ttu-id="05a20-122">Чтобы получить доступ к сайту группы для группы, создайте следующий запрос:</span><span class="sxs-lookup"><span data-stu-id="05a20-122">To access the team site for a group:</span></span>

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a><span data-ttu-id="05a20-123">Пример</span><span class="sxs-lookup"><span data-stu-id="05a20-123">Example</span></span>

### <a name="request"></a><span data-ttu-id="05a20-124">Запрос</span><span class="sxs-lookup"><span data-stu-id="05a20-124">Request</span></span>

<!-- { "blockType": "request", "name": "get-site" } -->

```http
GET /sites/{site-id}
```

### <a name="response"></a><span data-ttu-id="05a20-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="05a20-125">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE",
  "owner": {
    "user": {
      "displayName": "Daron Spektor",
      "id": "5280E7FE-DC7A-4486-9490-E790D81DFEB3"
    }
  },
  "displayName": "OneDrive Team Site",
  "name": "1drvteam",
  "createdDateTime": "2017-05-09T20:56:00Z",
  "lastModifiedDateTime": "2017-05-09T20:56:01Z",
  "webUrl": "https://contoso.sharepoint.com/teams/1drvteam"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="05a20-126">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="05a20-126">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="05a20-127">C#</span><span class="sxs-lookup"><span data-stu-id="05a20-127">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-site-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="05a20-128">Javascript</span><span class="sxs-lookup"><span data-stu-id="05a20-128">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-site-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="05a20-129">Цель — C</span><span class="sxs-lookup"><span data-stu-id="05a20-129">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-site-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Get by ID",
  "suppressions": [
    "Error: /api-reference/beta/api/site-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/site-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/site-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
