---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Получение сайта SharePoint
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: cac9de0dc81813bda482b20e72f8a62e6191f7a1
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481778"
---
# <a name="get-a-site-resource"></a><span data-ttu-id="d6709-102">Получение ресурса site</span><span class="sxs-lookup"><span data-stu-id="d6709-102">Get a site resource</span></span>

<span data-ttu-id="d6709-p101">Получение свойств и отношений ресурса [site][]. Ресурс **site** представляет сайт группы в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d6709-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[site]: ../resources/site.md

<span data-ttu-id="d6709-106">При обращении ресурс **site** рассматривается как уникальный идентификатор, состоящий из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="d6709-106">A **site** is addressed be a unique identifier which is a composite ID of the following values:</span></span>

* <span data-ttu-id="d6709-107">имя узла семейства веб-сайтов (contoso.sharepoint.com);</span><span class="sxs-lookup"><span data-stu-id="d6709-107">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="d6709-108">уникальный идентификатор семейства веб-сайтов (GUID);</span><span class="sxs-lookup"><span data-stu-id="d6709-108">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="d6709-109">уникальный идентификатор сайта (GUID).</span><span class="sxs-lookup"><span data-stu-id="d6709-109">Site unique ID (GUID)</span></span>

<span data-ttu-id="d6709-110">Кроме того, существует зарезервированный идентификатор сайта `root`, который всегда ссылается на корневой сайт указанного целевого объекта, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="d6709-110">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="d6709-111">`/sites/root`. Корневой сайт клиента.</span><span class="sxs-lookup"><span data-stu-id="d6709-111">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="d6709-112">`/groups/{group-id}/sites/root`. Сайт группы для ресурса group.</span><span class="sxs-lookup"><span data-stu-id="d6709-112">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6709-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d6709-113">Permissions</span></span>

<span data-ttu-id="d6709-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6709-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6709-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6709-116">Permission type</span></span>      | <span data-ttu-id="d6709-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6709-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6709-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6709-118">Delegated (work or school account)</span></span> | <span data-ttu-id="d6709-119">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6709-119">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d6709-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6709-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6709-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6709-121">Not supported.</span></span>    |
|<span data-ttu-id="d6709-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6709-122">Application</span></span> | <span data-ttu-id="d6709-123">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6709-123">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-the-tenants-root-site"></a><span data-ttu-id="d6709-124">Получение корневого сайта клиента</span><span class="sxs-lookup"><span data-stu-id="d6709-124">Get the tenant's root site</span></span>

<span data-ttu-id="d6709-125">Чтобы получить доступ к корневому сайту SharePoint внутри клиента, создайте следующие запросы:</span><span class="sxs-lookup"><span data-stu-id="d6709-125">To access the root SharePoint site within a tenant:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a><span data-ttu-id="d6709-126">Использование относительного URL-адреса сервера для доступа к сайту</span><span class="sxs-lookup"><span data-stu-id="d6709-126">Access a site by server-relative URL</span></span>

<span data-ttu-id="d6709-127">Если у вас есть относительный URL-адрес сервера для ресурса **site**, можно создать следующий запрос:</span><span class="sxs-lookup"><span data-stu-id="d6709-127">If you have the server-relative URL for a **site** resource, you can construct a request as follows:</span></span>

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a><span data-ttu-id="d6709-128">Доступ к сайту группы для группы</span><span class="sxs-lookup"><span data-stu-id="d6709-128">Access a group team site</span></span>

<span data-ttu-id="d6709-129">Чтобы получить доступ к сайту группы для группы, создайте следующий запрос:</span><span class="sxs-lookup"><span data-stu-id="d6709-129">To access the team site for a group:</span></span>

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a><span data-ttu-id="d6709-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d6709-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6709-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6709-131">Request</span></span>

<!-- { "blockType": "request", "name": "get-site", "scopes": "sites.read.all" } -->

```http
GET /sites/{site-id}
```

### <a name="response"></a><span data-ttu-id="d6709-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6709-132">Response</span></span>

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
  "tocPath": "Sites/Get by ID"
} -->
