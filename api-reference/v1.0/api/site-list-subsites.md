---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Создание списка дочерних сайтов для сайта SharePoint
localization_priority: Priority
ms.prod: sharepoint
description: Вы можете получить коллекцию дочерних сайтов, определенных для сайта.
doc_type: apiPageType
ms.openlocfilehash: 8ea4afee4289037e118efad49ef01926c3a76189
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36727686"
---
# <a name="enumerate-subsites"></a><span data-ttu-id="6b2a0-103">Перечисление дочерних сайтов</span><span class="sxs-lookup"><span data-stu-id="6b2a0-103">Enumerate subsites</span></span>

<span data-ttu-id="6b2a0-104">Вы можете получить коллекцию дочерних сайтов, определенных для [сайта][].</span><span class="sxs-lookup"><span data-stu-id="6b2a0-104">Get a collection of subsites defined for a [site][].</span></span>

[сайта]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="6b2a0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6b2a0-106">Permissions</span></span>

<span data-ttu-id="6b2a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b2a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b2a0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b2a0-109">Permission type</span></span>      | <span data-ttu-id="6b2a0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b2a0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b2a0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b2a0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6b2a0-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b2a0-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="6b2a0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b2a0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b2a0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b2a0-114">Not supported.</span></span>    |
|<span data-ttu-id="6b2a0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b2a0-115">Application</span></span> | <span data-ttu-id="6b2a0-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b2a0-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b2a0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b2a0-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6b2a0-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b2a0-118">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-subsites", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/sites/{site-id}/sites
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6b2a0-119">C#</span><span class="sxs-lookup"><span data-stu-id="6b2a0-119">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-subsites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6b2a0-120">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b2a0-120">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-subsites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6b2a0-121">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b2a0-121">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-subsites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6b2a0-122">Java</span><span class="sxs-lookup"><span data-stu-id="6b2a0-122">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-subsites-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="6b2a0-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b2a0-123">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/List subsites",
  "suppressions": [
  ]
} -->
