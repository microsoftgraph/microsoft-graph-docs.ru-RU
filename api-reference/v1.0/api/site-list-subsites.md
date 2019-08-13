---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Создание списка дочерних сайтов для сайта SharePoint
localization_priority: Priority
ms.prod: sharepoint
description: Вы можете получить коллекцию дочерних сайтов, определенных для сайта.
doc_type: apiPageType
ms.openlocfilehash: 11642a80dbcd6aa53dd21a4666b0d0298d53a3b6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372657"
---
# <a name="enumerate-subsites"></a><span data-ttu-id="33e7e-103">Перечисление дочерних сайтов</span><span class="sxs-lookup"><span data-stu-id="33e7e-103">Enumerate subsites</span></span>

<span data-ttu-id="33e7e-104">Вы можете получить коллекцию дочерних сайтов, определенных для [сайта][].</span><span class="sxs-lookup"><span data-stu-id="33e7e-104">Get a collection of subsites defined for a [site][].</span></span>

[сайта]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="33e7e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="33e7e-106">Permissions</span></span>

<span data-ttu-id="33e7e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33e7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33e7e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33e7e-109">Permission type</span></span>      | <span data-ttu-id="33e7e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="33e7e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33e7e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33e7e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="33e7e-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33e7e-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="33e7e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33e7e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33e7e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33e7e-114">Not supported.</span></span>    |
|<span data-ttu-id="33e7e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="33e7e-115">Application</span></span> | <span data-ttu-id="33e7e-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33e7e-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="33e7e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33e7e-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="33e7e-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="33e7e-118">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-subsites", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/sites
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="33e7e-119">C#</span><span class="sxs-lookup"><span data-stu-id="33e7e-119">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-subsites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="33e7e-120">JavaScript</span><span class="sxs-lookup"><span data-stu-id="33e7e-120">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-subsites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="33e7e-121">Objective-C</span><span class="sxs-lookup"><span data-stu-id="33e7e-121">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-subsites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="33e7e-122">Java</span><span class="sxs-lookup"><span data-stu-id="33e7e-122">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-subsites-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="33e7e-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="33e7e-123">Response</span></span>

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
