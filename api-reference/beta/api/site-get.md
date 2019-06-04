---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Получение сайта SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f189a28d9b4853492c68e581fc9790253ce6de89
ms.sourcegitcommit: 895a03cb2706a9b3a2236b30d6a7e9f5cbc6a89e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2019
ms.locfileid: "34683554"
---
# <a name="get-a-site-resource"></a><span data-ttu-id="a75b9-102">Получение ресурса site</span><span class="sxs-lookup"><span data-stu-id="a75b9-102">Get a site resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a75b9-p101">Получение свойств и отношений ресурса [site][]. Ресурс **site** представляет сайт группы в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a75b9-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="a75b9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a75b9-106">Permissions</span></span>

<span data-ttu-id="a75b9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a75b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a75b9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a75b9-109">Permission type</span></span>      | <span data-ttu-id="a75b9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a75b9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a75b9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a75b9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a75b9-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a75b9-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a75b9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a75b9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a75b9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a75b9-114">Not supported.</span></span>    |
|<span data-ttu-id="a75b9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a75b9-115">Application</span></span> | <span data-ttu-id="a75b9-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a75b9-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-the-tenants-root-site"></a><span data-ttu-id="a75b9-117">Получение корневого сайта клиента</span><span class="sxs-lookup"><span data-stu-id="a75b9-117">Get the tenant's root site</span></span>

<span data-ttu-id="a75b9-118">Чтобы получить доступ к корневому сайту SharePoint внутри клиента, создайте следующие запросы:</span><span class="sxs-lookup"><span data-stu-id="a75b9-118">To access the root SharePoint site within a tenant:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a><span data-ttu-id="a75b9-119">Использование относительного URL-адреса сервера для доступа к сайту</span><span class="sxs-lookup"><span data-stu-id="a75b9-119">Access a site by server-relative URL</span></span>

<span data-ttu-id="a75b9-120">Если у вас есть относительный URL-адрес сервера для ресурса **site**, можно создать следующий запрос:</span><span class="sxs-lookup"><span data-stu-id="a75b9-120">If you have the server-relative URL for a **site** resource, you can construct a request as follows:</span></span>

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a><span data-ttu-id="a75b9-121">Доступ к сайту группы для группы</span><span class="sxs-lookup"><span data-stu-id="a75b9-121">Access a group team site</span></span>

<span data-ttu-id="a75b9-122">Чтобы получить доступ к сайту группы для группы, создайте следующий запрос:</span><span class="sxs-lookup"><span data-stu-id="a75b9-122">To access the team site for a group:</span></span>

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a><span data-ttu-id="a75b9-123">Пример</span><span class="sxs-lookup"><span data-stu-id="a75b9-123">Example</span></span>

### <a name="request"></a><span data-ttu-id="a75b9-124">Запрос</span><span class="sxs-lookup"><span data-stu-id="a75b9-124">Request</span></span>

<!-- { "blockType": "request", "name": "get-site" } -->

```http
GET /sites/{site-id}
```

### <a name="response"></a><span data-ttu-id="a75b9-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="a75b9-125">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a75b9-126">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="a75b9-126">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a75b9-127">C#</span><span class="sxs-lookup"><span data-stu-id="a75b9-127">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-site-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a75b9-128">Javascript</span><span class="sxs-lookup"><span data-stu-id="a75b9-128">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-site-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/site-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/site-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
