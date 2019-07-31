---
author: rahmit
description: Возвращает метаданные для объекта Ситепаже в списке страниц сайта на сайте.
ms.date: 03/15/2018
title: Получение страницы на сайте
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 384436bbae1318eb66e6edc345c2949b9c1d0aba
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991221"
---
# <a name="get-a-page-in-the-site-pages-list-of-a-site"></a><span data-ttu-id="afe36-103">Получение страницы в списке страниц сайта</span><span class="sxs-lookup"><span data-stu-id="afe36-103">Get a page in the site pages list of a site</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="afe36-104">Возвращает метаданные для объекта [ситепаже][] в [списке][] страниц сайта на [сайте][].</span><span class="sxs-lookup"><span data-stu-id="afe36-104">Returns the metadata for a [sitePage][] in the site pages [list][] in a [site][].</span></span>

[sitePage]: ../resources/sitepage.md
[list]: ../resources/list.md
[сайта]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="afe36-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="afe36-108">Permissions</span></span>

<span data-ttu-id="afe36-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afe36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afe36-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="afe36-111">Permission type</span></span>      | <span data-ttu-id="afe36-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="afe36-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="afe36-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="afe36-113">Delegated (work or school account)</span></span> | <span data-ttu-id="afe36-114">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afe36-114">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="afe36-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="afe36-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afe36-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="afe36-116">Not supported.</span></span>    |
|<span data-ttu-id="afe36-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="afe36-117">Application</span></span> | <span data-ttu-id="afe36-118">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afe36-118">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="afe36-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="afe36-119">HTTP request</span></span>

```http
GET /sites/{site-id}/pages/{page-id}
```

## <a name="example"></a><span data-ttu-id="afe36-120">Пример</span><span class="sxs-lookup"><span data-stu-id="afe36-120">Example</span></span>

##### <a name="request"></a><span data-ttu-id="afe36-121">Запрос</span><span class="sxs-lookup"><span data-stu-id="afe36-121">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="afe36-122">HTTP</span><span class="sxs-lookup"><span data-stu-id="afe36-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-page", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
GET /sites/{site-id}/pages/{page-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="afe36-123">C#</span><span class="sxs-lookup"><span data-stu-id="afe36-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-page-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="afe36-124">Javascript</span><span class="sxs-lookup"><span data-stu-id="afe36-124">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-page-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="afe36-125">Цель — C</span><span class="sxs-lookup"><span data-stu-id="afe36-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-page-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="afe36-126">Java</span><span class="sxs-lookup"><span data-stu-id="afe36-126">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-page-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="afe36-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="afe36-127">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.sitePage", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "2",
    "eTag": "75bc70e2-6587-45be-8493-c99a956b2e05,7",
    "createdDateTime": "2016-12-06T20:04:40Z",
    "lastModifiedDateTime": "2016-12-06T20:05:09Z",
    "webUrl": "https://www.contoso.com/sites/Engineering/SitePages/Events.aspx",
    "createdBy": {
        "user": {
            "email": "rahmit@microsoft.com",
            "id": "1b37d2e1-5000-4648-b431-7dfa509b5660",
            "displayName": "Rahul Mittal (ODSP)"
        }
    },
    "lastModifiedBy": {
        "user": {
            "email": "rahmit@microsoft.com",
            "id": "1b37d2e1-5000-4648-b431-7dfa509b5660",
            "displayName": "Rahul Mittal (ODSP)"
        }
    },
    "parentReference": {
        "id": "eb3bfd48-56f8-4c1e-8312-e58588b22e7c"
    },
    "contentType": {
        "id": "0x0101009D1CB255DA76424F860D91F20E6C411800C9E7033636784C4B88A284B1823C45FD",
        "name": "Site Page"
    },
    "description": "",
    "title": "Upcoming Events",
    "publishingState": {
        "level": "published",
        "versionId": "1.0"
    },
    "webParts": [
        {
            "type": "rte",
            "data": {
                "innerHTML": "<p>Here are the team's upcoming events:</p>"
            }
        },
        {
            "type": "d1d91016-032f-456d-98a4-721247c305e8",
            "data": {
                "title": "Events",
                "description": "Display upcoming events",
                "serverProcessedContent": {
                    "htmlStrings": {},
                    "searchablePlainTexts": {
                        "title": ""
                    },
                    "imageSources": {},
                    "links": {
                        "baseUrl": "https://www.contoso.com/sites/Engineering"
                    },
                    "componentDependencies": {
                        "layoutComponentId": "8ac0c53c-e8d0-4e3e-87d0-7449eb0d4027"
                    }
                },
                "dataVersion": "1.0",
                "properties": {
                    "selectedListId": "032e08ab-89b0-4d8f-bc10-73094233615c",
                    "selectedCategory": "",
                    "dateRangeOption": 0,
                    "startDate": "",
                    "endDate": "",
                    "isOnSeeAllPage": false,
                    "layoutId": "FilmStrip",
                    "dataProviderId": "Event",
                    "webId": "0764c419-1ecc-4126-ba32-0c25ae0fffe8",
                    "siteId": "6b4ffc7a-cfc2-4a76-903a-1cc3686dee23"
                }
            }
        }
    ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Get a page in a site",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Pages/Enumerate",
  "suppressions": [
  ]
}
-->
