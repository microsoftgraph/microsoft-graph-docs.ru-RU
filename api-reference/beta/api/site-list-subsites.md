---
author: JeremyKelley
description: Вы можете получить коллекцию дочерних сайтов, определенных для сайта.
ms.date: 09/10/2017
title: Создание списка дочерних сайтов для сайта SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 4e69e016f1a83db1b4a2f23e4829ef28d3e3cff0
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475795"
---
# <a name="enumerate-subsites"></a><span data-ttu-id="a43d8-103">Перечисление дочерних сайтов</span><span class="sxs-lookup"><span data-stu-id="a43d8-103">Enumerate subsites</span></span>

<span data-ttu-id="a43d8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a43d8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a43d8-105">Вы можете получить коллекцию дочерних сайтов, определенных для [сайта][].</span><span class="sxs-lookup"><span data-stu-id="a43d8-105">Get a collection of subsites defined for a [site][].</span></span>

[сайта]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="a43d8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a43d8-107">Permissions</span></span>

<span data-ttu-id="a43d8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a43d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a43d8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a43d8-110">Permission type</span></span>      | <span data-ttu-id="a43d8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a43d8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a43d8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a43d8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a43d8-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a43d8-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a43d8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a43d8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a43d8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a43d8-115">Not supported.</span></span>    |
|<span data-ttu-id="a43d8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a43d8-116">Application</span></span> | <span data-ttu-id="a43d8-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a43d8-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a43d8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a43d8-118">HTTP request</span></span>

```http
GET /sites/{site-id}/sites
```

# <a name="http"></a>[<span data-ttu-id="a43d8-119">HTTP</span><span class="sxs-lookup"><span data-stu-id="a43d8-119">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-subsites", "scopes": "service.sharepoint sites.read.all" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{site-id}/sites
```
# <a name="c"></a>[<span data-ttu-id="a43d8-120">C#</span><span class="sxs-lookup"><span data-stu-id="a43d8-120">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-subsites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a43d8-121">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a43d8-121">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-subsites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a43d8-122">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a43d8-122">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-subsites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a43d8-123">Java</span><span class="sxs-lookup"><span data-stu-id="a43d8-123">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-subsites-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="a43d8-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="a43d8-124">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740",
      "name": "Team A Subsite",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/site/subsiteA"
    },
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
      "name": "Team B Subsite",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/site/subsiteB"
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/List subsites",
  "suppressions": [
  ]
}
-->


