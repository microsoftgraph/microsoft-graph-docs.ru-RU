---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Получение сайта SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: cac9de0dc81813bda482b20e72f8a62e6191f7a1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32520799"
---
# <a name="get-a-site-resource"></a><span data-ttu-id="56f00-102">Получение ресурса site</span><span class="sxs-lookup"><span data-stu-id="56f00-102">Get a site resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56f00-p101">Получение свойств и отношений ресурса [site][]. Ресурс **site** представляет сайт группы в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="56f00-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[site]: ../resources/site.md

<span data-ttu-id="56f00-106">При обращении ресурс **site** рассматривается как уникальный идентификатор, состоящий из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="56f00-106">A **site** is addressed be a unique identifier which is a composite ID of the following values:</span></span>

* <span data-ttu-id="56f00-107">имя узла семейства веб-сайтов (contoso.sharepoint.com);</span><span class="sxs-lookup"><span data-stu-id="56f00-107">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="56f00-108">уникальный идентификатор семейства веб-сайтов (GUID);</span><span class="sxs-lookup"><span data-stu-id="56f00-108">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="56f00-109">уникальный идентификатор сайта (GUID).</span><span class="sxs-lookup"><span data-stu-id="56f00-109">Site unique ID (GUID)</span></span>

<span data-ttu-id="56f00-110">Кроме того, существует зарезервированный идентификатор сайта `root`, который всегда ссылается на корневой сайт указанного целевого объекта, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="56f00-110">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="56f00-111">`/sites/root`. Корневой сайт клиента.</span><span class="sxs-lookup"><span data-stu-id="56f00-111">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="56f00-112">`/groups/{group-id}/sites/root`. Сайт группы для ресурса group.</span><span class="sxs-lookup"><span data-stu-id="56f00-112">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="56f00-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="56f00-113">Permissions</span></span>

<span data-ttu-id="56f00-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56f00-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56f00-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56f00-116">Permission type</span></span>      | <span data-ttu-id="56f00-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="56f00-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56f00-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56f00-118">Delegated (work or school account)</span></span> | <span data-ttu-id="56f00-119">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56f00-119">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="56f00-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56f00-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56f00-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56f00-121">Not supported.</span></span>    |
|<span data-ttu-id="56f00-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="56f00-122">Application</span></span> | <span data-ttu-id="56f00-123">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56f00-123">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-the-tenants-root-site"></a><span data-ttu-id="56f00-124">Получение корневого сайта клиента</span><span class="sxs-lookup"><span data-stu-id="56f00-124">Get the tenant's root site</span></span>

<span data-ttu-id="56f00-125">Чтобы получить доступ к корневому сайту SharePoint внутри клиента, создайте следующие запросы:</span><span class="sxs-lookup"><span data-stu-id="56f00-125">To access the root SharePoint site within a tenant:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a><span data-ttu-id="56f00-126">Использование относительного URL-адреса сервера для доступа к сайту</span><span class="sxs-lookup"><span data-stu-id="56f00-126">Access a site by server-relative URL</span></span>

<span data-ttu-id="56f00-127">Если у вас есть относительный URL-адрес сервера для ресурса **site**, можно создать следующий запрос:</span><span class="sxs-lookup"><span data-stu-id="56f00-127">If you have the server-relative URL for a **site** resource, you can construct a request as follows:</span></span>

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a><span data-ttu-id="56f00-128">Доступ к сайту группы для группы</span><span class="sxs-lookup"><span data-stu-id="56f00-128">Access a group team site</span></span>

<span data-ttu-id="56f00-129">Чтобы получить доступ к сайту группы для группы, создайте следующий запрос:</span><span class="sxs-lookup"><span data-stu-id="56f00-129">To access the team site for a group:</span></span>

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a><span data-ttu-id="56f00-130">Пример</span><span class="sxs-lookup"><span data-stu-id="56f00-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="56f00-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="56f00-131">Request</span></span>

<!-- { "blockType": "request", "name": "get-site" } -->

```http
GET /sites/{site-id}
```

### <a name="response"></a><span data-ttu-id="56f00-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="56f00-132">Response</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Get by ID",
  "suppressions": [
    "Error: /api-reference/beta/api/site-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
