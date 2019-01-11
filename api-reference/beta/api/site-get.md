---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Получение сайта SharePoint
localization_priority: Normal
ms.openlocfilehash: 72a99b1768486da792a401cea4b8dfde5a25a153
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872858"
---
# <a name="get-a-site-resource"></a><span data-ttu-id="7dcdc-102">Получение ресурса site</span><span class="sxs-lookup"><span data-stu-id="7dcdc-102">Get a site resource</span></span>

> <span data-ttu-id="7dcdc-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7dcdc-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7dcdc-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7dcdc-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7dcdc-p102">Получение свойств и отношений ресурса [site][]. Ресурс **site** представляет сайт группы в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7dcdc-p102">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[site]: ../resources/site.md

<span data-ttu-id="7dcdc-108">При обращении ресурс **site** рассматривается как уникальный идентификатор, состоящий из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="7dcdc-108">A **site** is addressed be a unique identifier which is a composite ID of the following values:</span></span>

* <span data-ttu-id="7dcdc-109">имя узла семейства веб-сайтов (contoso.sharepoint.com);</span><span class="sxs-lookup"><span data-stu-id="7dcdc-109">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="7dcdc-110">уникальный идентификатор семейства веб-сайтов (GUID);</span><span class="sxs-lookup"><span data-stu-id="7dcdc-110">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="7dcdc-111">уникальный идентификатор сайта (GUID).</span><span class="sxs-lookup"><span data-stu-id="7dcdc-111">Site unique ID (GUID)</span></span>

<span data-ttu-id="7dcdc-112">Кроме того, существует зарезервированный идентификатор сайта `root`, который всегда ссылается на корневой сайт указанного целевого объекта, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="7dcdc-112">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="7dcdc-113">`/sites/root`. Корневой сайт клиента.</span><span class="sxs-lookup"><span data-stu-id="7dcdc-113">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="7dcdc-114">`/groups/{group-id}/sites/root`. Сайт группы для ресурса group.</span><span class="sxs-lookup"><span data-stu-id="7dcdc-114">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="7dcdc-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7dcdc-115">Permissions</span></span>

<span data-ttu-id="7dcdc-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7dcdc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dcdc-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7dcdc-118">Permission type</span></span>      | <span data-ttu-id="7dcdc-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7dcdc-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7dcdc-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7dcdc-120">Delegated (work or school account)</span></span> | <span data-ttu-id="7dcdc-121">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dcdc-121">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7dcdc-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7dcdc-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7dcdc-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7dcdc-123">Not supported.</span></span>    |
|<span data-ttu-id="7dcdc-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7dcdc-124">Application</span></span> | <span data-ttu-id="7dcdc-125">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dcdc-125">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-the-tenants-root-site"></a><span data-ttu-id="7dcdc-126">Получение корневого сайта клиента</span><span class="sxs-lookup"><span data-stu-id="7dcdc-126">Get the tenant's root site</span></span>

<span data-ttu-id="7dcdc-127">Чтобы получить доступ к корневому сайту SharePoint внутри клиента, создайте следующие запросы:</span><span class="sxs-lookup"><span data-stu-id="7dcdc-127">To access the root SharePoint site within a tenant:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a><span data-ttu-id="7dcdc-128">Использование относительного URL-адреса сервера для доступа к сайту</span><span class="sxs-lookup"><span data-stu-id="7dcdc-128">Access a site by server-relative URL</span></span>

<span data-ttu-id="7dcdc-129">Если у вас есть относительный URL-адрес сервера для ресурса **site**, можно создать следующий запрос:</span><span class="sxs-lookup"><span data-stu-id="7dcdc-129">If you have the server-relative URL for a **site** resource, you can construct a request as follows:</span></span>

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a><span data-ttu-id="7dcdc-130">Доступ к сайту группы для ресурса group</span><span class="sxs-lookup"><span data-stu-id="7dcdc-130">Access a group team site</span></span>

<span data-ttu-id="7dcdc-131">Чтобы получить доступ к сайту группы для ресурса group, создайте следующий запрос:</span><span class="sxs-lookup"><span data-stu-id="7dcdc-131">To access the team site for a group:</span></span>

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a><span data-ttu-id="7dcdc-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7dcdc-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7dcdc-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7dcdc-133">Request</span></span>

<!-- { "blockType": "request", "name": "get-site" } -->

```http
GET /sites/{site-id}
```

### <a name="response"></a><span data-ttu-id="7dcdc-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="7dcdc-134">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Get by ID"
} -->
