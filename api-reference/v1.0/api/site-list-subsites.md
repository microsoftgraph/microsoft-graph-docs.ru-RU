---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Создание списка дочерних сайтов для сайта SharePoint
localization_priority: Priority
ms.prod: sharepoint
description: Вы можете получить коллекцию дочерних сайтов, определенных для сайта.
doc_type: apiPageType
ms.openlocfilehash: 853170cb82f5874d322bd5122f74396813ad3153
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038174"
---
# <a name="enumerate-subsites"></a><span data-ttu-id="befe6-103">Перечисление дочерних сайтов</span><span class="sxs-lookup"><span data-stu-id="befe6-103">Enumerate subsites</span></span>

<span data-ttu-id="befe6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="befe6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="befe6-105">Вы можете получить коллекцию дочерних сайтов, определенных для [сайта][].</span><span class="sxs-lookup"><span data-stu-id="befe6-105">Get a collection of subsites defined for a [site][].</span></span>

[сайта]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="befe6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="befe6-107">Permissions</span></span>

<span data-ttu-id="befe6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="befe6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="befe6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="befe6-110">Permission type</span></span>      | <span data-ttu-id="befe6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="befe6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="befe6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="befe6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="befe6-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="befe6-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="befe6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="befe6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="befe6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="befe6-115">Not supported.</span></span>    |
|<span data-ttu-id="befe6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="befe6-116">Application</span></span> | <span data-ttu-id="befe6-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="befe6-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="befe6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="befe6-118">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="befe6-119">HTTP</span><span class="sxs-lookup"><span data-stu-id="befe6-119">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-subsites", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/sites/{site-id}/sites
```
# <a name="c"></a>[<span data-ttu-id="befe6-120">C#</span><span class="sxs-lookup"><span data-stu-id="befe6-120">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-subsites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="befe6-121">JavaScript</span><span class="sxs-lookup"><span data-stu-id="befe6-121">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-subsites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="befe6-122">Objective-C</span><span class="sxs-lookup"><span data-stu-id="befe6-122">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-subsites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="befe6-123">Java</span><span class="sxs-lookup"><span data-stu-id="befe6-123">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-subsites-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="befe6-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="befe6-124">Response</span></span>

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

