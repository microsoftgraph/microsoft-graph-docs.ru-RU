---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Создание списка дочерних сайтов для сайта SharePoint
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: fd0b4c43ae03bd7f09ea095e2f7a73b6fa1dbc13
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481190"
---
# <a name="enumerate-subsites"></a><span data-ttu-id="bd46e-102">Перечисление дочерних сайтов</span><span class="sxs-lookup"><span data-stu-id="bd46e-102">Enumerate subsites</span></span>

<span data-ttu-id="bd46e-103">Вы можете получить коллекцию дочерних сайтов, определенных для [сайта][].</span><span class="sxs-lookup"><span data-stu-id="bd46e-103">Get a collection of subsites defined for a [site][].</span></span>

[сайта]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="bd46e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bd46e-105">Permissions</span></span>

<span data-ttu-id="bd46e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd46e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd46e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd46e-108">Permission type</span></span>      | <span data-ttu-id="bd46e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd46e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd46e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd46e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bd46e-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd46e-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="bd46e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd46e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd46e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd46e-113">Not supported.</span></span>    |
|<span data-ttu-id="bd46e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd46e-114">Application</span></span> | <span data-ttu-id="bd46e-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd46e-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd46e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd46e-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "list-subsites", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/sites
```

## <a name="response"></a><span data-ttu-id="bd46e-117">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd46e-117">Response</span></span>

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
  "tocPath": "Sites/List subsites"
} -->
