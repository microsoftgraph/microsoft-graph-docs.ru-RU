---
author: JeremyKelley
description: Вы можете получить свойства и связи ресурса site.
ms.date: 09/10/2017
title: Получение сайта SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: d39c9532a267dae36a7c0f1718402d25f6ce00f2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36363762"
---
# <a name="get-a-site-resource"></a><span data-ttu-id="f237b-103">Получение ресурса site</span><span class="sxs-lookup"><span data-stu-id="f237b-103">Get a site resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f237b-p101">Получение свойств и отношений ресурса [site][]. Ресурс **site** представляет сайт группы в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f237b-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[сайта]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="f237b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f237b-107">Permissions</span></span>

<span data-ttu-id="f237b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f237b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f237b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f237b-110">Permission type</span></span>      | <span data-ttu-id="f237b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f237b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f237b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f237b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f237b-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f237b-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f237b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f237b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f237b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f237b-115">Not supported.</span></span>    |
|<span data-ttu-id="f237b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f237b-116">Application</span></span> | <span data-ttu-id="f237b-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f237b-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-the-tenants-root-site"></a><span data-ttu-id="f237b-118">Получение корневого сайта клиента</span><span class="sxs-lookup"><span data-stu-id="f237b-118">Get the tenant's root site</span></span>

<span data-ttu-id="f237b-119">Чтобы получить доступ к корневому сайту SharePoint внутри клиента, создайте следующие запросы:</span><span class="sxs-lookup"><span data-stu-id="f237b-119">To access the root SharePoint site within a tenant:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a><span data-ttu-id="f237b-120">Использование относительного URL-адреса сервера для доступа к сайту</span><span class="sxs-lookup"><span data-stu-id="f237b-120">Access a site by server-relative URL</span></span>

<span data-ttu-id="f237b-121">Если у вас есть относительный URL-адрес сервера для ресурса **site**, можно создать следующий запрос:</span><span class="sxs-lookup"><span data-stu-id="f237b-121">If you have the server-relative URL for a **site** resource, you can construct a request as follows:</span></span>

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a><span data-ttu-id="f237b-122">Доступ к сайту группы для группы</span><span class="sxs-lookup"><span data-stu-id="f237b-122">Access a group team site</span></span>

<span data-ttu-id="f237b-123">Чтобы получить доступ к сайту группы для группы, создайте следующий запрос:</span><span class="sxs-lookup"><span data-stu-id="f237b-123">To access the team site for a group:</span></span>

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a><span data-ttu-id="f237b-124">Пример</span><span class="sxs-lookup"><span data-stu-id="f237b-124">Example</span></span>

### <a name="request"></a><span data-ttu-id="f237b-125">Запрос</span><span class="sxs-lookup"><span data-stu-id="f237b-125">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f237b-126">HTTP</span><span class="sxs-lookup"><span data-stu-id="f237b-126">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-site" } -->

```http
GET /sites/{site-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f237b-127">C#</span><span class="sxs-lookup"><span data-stu-id="f237b-127">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f237b-128">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f237b-128">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f237b-129">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f237b-129">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f237b-130">Java</span><span class="sxs-lookup"><span data-stu-id="f237b-130">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f237b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f237b-131">Response</span></span>

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
  ]
}
-->
