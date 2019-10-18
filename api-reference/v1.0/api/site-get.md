---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Получение сайта SharePoint
localization_priority: Priority
ms.prod: sharepoint
description: Получение свойств и отношений ресурса site.
doc_type: apiPageType
ms.openlocfilehash: 102295c12ca5278b40c9540049282db360f7701b
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36727721"
---
# <a name="get-a-site-resource"></a><span data-ttu-id="95674-103">Получение ресурса site</span><span class="sxs-lookup"><span data-stu-id="95674-103">Get a site resource</span></span>

<span data-ttu-id="95674-p101">Получение свойств и отношений ресурса [site][]. Ресурс **site** представляет сайт группы в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="95674-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[сайта]: ../resources/site.md
[site]: ../resources/site.md

<span data-ttu-id="95674-107">Для обращения к ресурсу **site** используется уникальный идентификатор, при создании которого используются указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="95674-107">A **site** is addressed by a unique identifier which is a composite ID of the following values:</span></span>

* <span data-ttu-id="95674-108">имя узла семейства веб-сайтов (contoso.sharepoint.com);</span><span class="sxs-lookup"><span data-stu-id="95674-108">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="95674-109">уникальный идентификатор семейства веб-сайтов (GUID);</span><span class="sxs-lookup"><span data-stu-id="95674-109">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="95674-110">уникальный идентификатор сайта (GUID).</span><span class="sxs-lookup"><span data-stu-id="95674-110">Site unique ID (GUID)</span></span>

<span data-ttu-id="95674-111">Кроме того, существует зарезервированный идентификатор сайта `root`, который всегда ссылается на корневой сайт указанного целевого объекта, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="95674-111">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="95674-112">`/sites/root`. Корневой сайт клиента.</span><span class="sxs-lookup"><span data-stu-id="95674-112">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="95674-113">`/groups/{group-id}/sites/root`. Сайт группы для ресурса group.</span><span class="sxs-lookup"><span data-stu-id="95674-113">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="95674-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="95674-114">Permissions</span></span>

<span data-ttu-id="95674-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95674-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95674-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95674-117">Permission type</span></span>      | <span data-ttu-id="95674-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="95674-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95674-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95674-119">Delegated (work or school account)</span></span> | <span data-ttu-id="95674-120">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95674-120">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="95674-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95674-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95674-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95674-122">Not supported.</span></span>    |
|<span data-ttu-id="95674-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="95674-123">Application</span></span> | <span data-ttu-id="95674-124">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95674-124">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-the-tenants-root-site"></a><span data-ttu-id="95674-125">Получение корневого сайта клиента</span><span class="sxs-lookup"><span data-stu-id="95674-125">Get the tenant's root site</span></span>

<span data-ttu-id="95674-126">Чтобы получить доступ к корневому сайту SharePoint внутри клиента, создайте следующие запросы:</span><span class="sxs-lookup"><span data-stu-id="95674-126">To access the root SharePoint site within a tenant:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a><span data-ttu-id="95674-127">Использование относительного URL-адреса сервера для доступа к сайту</span><span class="sxs-lookup"><span data-stu-id="95674-127">Access a site by server-relative URL</span></span>

<span data-ttu-id="95674-128">Если у вас есть относительный URL-адрес сервера для ресурса **site**, можно создать следующий запрос:</span><span class="sxs-lookup"><span data-stu-id="95674-128">If you have the server-relative URL for a **site** resource, you can construct a request as follows:</span></span>

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a><span data-ttu-id="95674-129">Доступ к сайту группы для группы</span><span class="sxs-lookup"><span data-stu-id="95674-129">Access a group team site</span></span>

<span data-ttu-id="95674-130">Чтобы получить доступ к сайту группы для группы, создайте следующий запрос:</span><span class="sxs-lookup"><span data-stu-id="95674-130">To access the team site for a group:</span></span>

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a><span data-ttu-id="95674-131">Пример</span><span class="sxs-lookup"><span data-stu-id="95674-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="95674-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="95674-132">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="95674-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="95674-133">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-site", "scopes": "sites.read.all" } -->

```msgraph-interactive
GET /sites/{site-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="95674-134">C#</span><span class="sxs-lookup"><span data-stu-id="95674-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="95674-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95674-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="95674-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95674-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="95674-137">Java</span><span class="sxs-lookup"><span data-stu-id="95674-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="95674-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="95674-138">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE",
  "displayName": "OneDrive Team Site",
  "name": "1drvteam",
  "createdDateTime": "2017-05-09T20:56:00Z",
  "lastModifiedDateTime": "2017-05-09T20:56:01Z",
  "webUrl": "https://contoso.sharepoint.com/teams/1drvteam"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Get by ID",
  "suppressions": [
  ]
} -->
