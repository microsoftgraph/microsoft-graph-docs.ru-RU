---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Создание списка дочерних сайтов для сайта SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: bdbe1b70be15cac8acfd55a4735acd6185408545
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638563"
---
# <a name="enumerate-subsites"></a><span data-ttu-id="60703-102">Перечисление дочерних сайтов</span><span class="sxs-lookup"><span data-stu-id="60703-102">Enumerate subsites</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60703-103">Вы можете получить коллекцию дочерних сайтов, определенных для [сайта][].</span><span class="sxs-lookup"><span data-stu-id="60703-103">Get a collection of subsites defined for a [site][].</span></span>

[сайта]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="60703-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="60703-105">Permissions</span></span>

<span data-ttu-id="60703-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60703-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60703-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60703-108">Permission type</span></span>      | <span data-ttu-id="60703-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="60703-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60703-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60703-110">Delegated (work or school account)</span></span> | <span data-ttu-id="60703-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60703-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="60703-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60703-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60703-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60703-113">Not supported.</span></span>    |
|<span data-ttu-id="60703-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="60703-114">Application</span></span> | <span data-ttu-id="60703-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60703-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="60703-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60703-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "list-subsites", "scopes": "service.sharepoint sites.read.all" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/sites
```

## <a name="response"></a><span data-ttu-id="60703-117">Отклик</span><span class="sxs-lookup"><span data-stu-id="60703-117">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="60703-118">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="60703-118">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="60703-119">Языках</span><span class="sxs-lookup"><span data-stu-id="60703-119">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/list-subsites-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="60703-120">Язык</span><span class="sxs-lookup"><span data-stu-id="60703-120">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/list-subsites-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/site-list-subsites.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/site-list-subsites.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
