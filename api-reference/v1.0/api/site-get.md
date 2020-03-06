---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Получение сайта SharePoint
localization_priority: Priority
ms.prod: sharepoint
description: Получение свойств и отношений ресурса site.
doc_type: apiPageType
ms.openlocfilehash: af50b2eae0287ad31e75c6373b6dedb4c67bd42b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509803"
---
# <a name="get-a-site-resource"></a><span data-ttu-id="e163f-103">Получение ресурса site</span><span class="sxs-lookup"><span data-stu-id="e163f-103">Get a site resource</span></span>

<span data-ttu-id="e163f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e163f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e163f-p101">Получение свойств и отношений ресурса [site][]. Ресурс **site** представляет сайт группы в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e163f-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[сайта]: ../resources/site.md
[site]: ../resources/site.md

<span data-ttu-id="e163f-108">Для обращения к ресурсу **site** используется уникальный идентификатор, при создании которого используются указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="e163f-108">A **site** is addressed by a unique identifier which is a composite ID of the following values:</span></span>

* <span data-ttu-id="e163f-109">имя узла семейства веб-сайтов (contoso.sharepoint.com);</span><span class="sxs-lookup"><span data-stu-id="e163f-109">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="e163f-110">уникальный идентификатор семейства веб-сайтов (GUID);</span><span class="sxs-lookup"><span data-stu-id="e163f-110">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="e163f-111">уникальный идентификатор сайта (GUID).</span><span class="sxs-lookup"><span data-stu-id="e163f-111">Site unique ID (GUID)</span></span>

<span data-ttu-id="e163f-112">Кроме того, существует зарезервированный идентификатор сайта `root`, который всегда ссылается на корневой сайт указанного целевого объекта, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="e163f-112">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="e163f-113">`/sites/root`. Корневой сайт клиента.</span><span class="sxs-lookup"><span data-stu-id="e163f-113">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="e163f-114">`/groups/{group-id}/sites/root`. Сайт группы для ресурса group.</span><span class="sxs-lookup"><span data-stu-id="e163f-114">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="e163f-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e163f-115">Permissions</span></span>

<span data-ttu-id="e163f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e163f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e163f-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e163f-118">Permission type</span></span>      | <span data-ttu-id="e163f-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e163f-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e163f-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e163f-120">Delegated (work or school account)</span></span> | <span data-ttu-id="e163f-121">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e163f-121">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e163f-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e163f-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e163f-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e163f-123">Not supported.</span></span>    |
|<span data-ttu-id="e163f-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e163f-124">Application</span></span> | <span data-ttu-id="e163f-125">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e163f-125">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-the-tenants-root-site"></a><span data-ttu-id="e163f-126">Получение корневого сайта клиента</span><span class="sxs-lookup"><span data-stu-id="e163f-126">Get the tenant's root site</span></span>

<span data-ttu-id="e163f-127">Чтобы получить доступ к корневому сайту SharePoint внутри клиента, создайте следующие запросы:</span><span class="sxs-lookup"><span data-stu-id="e163f-127">To access the root SharePoint site within a tenant:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a><span data-ttu-id="e163f-128">Использование относительного URL-адреса сервера для доступа к сайту</span><span class="sxs-lookup"><span data-stu-id="e163f-128">Access a site by server-relative URL</span></span>

<span data-ttu-id="e163f-129">Если у вас есть относительный URL-адрес сервера для ресурса **site**, можно создать следующий запрос:</span><span class="sxs-lookup"><span data-stu-id="e163f-129">If you have the server-relative URL for a **site** resource, you can construct a request as follows:</span></span>

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a><span data-ttu-id="e163f-130">Доступ к сайту группы для группы</span><span class="sxs-lookup"><span data-stu-id="e163f-130">Access a group team site</span></span>

<span data-ttu-id="e163f-131">Чтобы получить доступ к сайту группы для группы, создайте следующий запрос:</span><span class="sxs-lookup"><span data-stu-id="e163f-131">To access the team site for a group:</span></span>

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a><span data-ttu-id="e163f-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e163f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e163f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e163f-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e163f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e163f-134">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-site", "scopes": "sites.read.all" } -->

```msgraph-interactive
GET /sites/{site-id}
```
# <a name="c"></a>[<span data-ttu-id="e163f-135">C#</span><span class="sxs-lookup"><span data-stu-id="e163f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e163f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e163f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e163f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e163f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e163f-138">Java</span><span class="sxs-lookup"><span data-stu-id="e163f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e163f-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="e163f-139">Response</span></span>

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
