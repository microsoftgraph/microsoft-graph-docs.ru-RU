---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Создание списка дочерних сайтов для сайта SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5a2c16b53dd6b89588932d0f562f91a2deba348a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271577"
---
# <a name="enumerate-subsites"></a><span data-ttu-id="14425-102">Перечисление дочерних сайтов</span><span class="sxs-lookup"><span data-stu-id="14425-102">Enumerate subsites</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14425-103">Вы можете получить коллекцию дочерних сайтов, определенных для [сайта][].</span><span class="sxs-lookup"><span data-stu-id="14425-103">Get a collection of subsites defined for a [site][].</span></span>

[сайта]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="14425-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="14425-105">Permissions</span></span>

<span data-ttu-id="14425-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14425-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14425-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14425-108">Permission type</span></span>      | <span data-ttu-id="14425-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="14425-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14425-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14425-110">Delegated (work or school account)</span></span> | <span data-ttu-id="14425-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14425-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="14425-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14425-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14425-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14425-113">Not supported.</span></span>    |
|<span data-ttu-id="14425-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14425-114">Application</span></span> | <span data-ttu-id="14425-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14425-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="14425-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14425-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "list-subsites", "scopes": "service.sharepoint sites.read.all" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/sites
```

## <a name="response"></a><span data-ttu-id="14425-117">Отклик</span><span class="sxs-lookup"><span data-stu-id="14425-117">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="14425-118">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="14425-118">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="14425-119">C#</span><span class="sxs-lookup"><span data-stu-id="14425-119">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/list-subsites-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="14425-120">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14425-120">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/list-subsites-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="14425-121">Цель — C</span><span class="sxs-lookup"><span data-stu-id="14425-121">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/list-subsites-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/List subsites",
  "suppressions": [
    "Error: /api-reference/beta/api/site-list-subsites.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/site-list-subsites.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/site-list-subsites.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
