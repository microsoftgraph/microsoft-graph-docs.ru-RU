---
author: rahmit
ms.author: rahmit
ms.date: 03/15/2018
title: Получение страницы на сайте
localization_priority: Normal
ms.openlocfilehash: a212dab1c7a15a51d525b332ca5822da8fe28bdd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806673"
---
# <a name="get-a-page-in-the-site-pages-list-of-a-site"></a><span data-ttu-id="e8a0c-102">Получение страницы в списке страниц сайта узла</span><span class="sxs-lookup"><span data-stu-id="e8a0c-102">Get a page in the site pages list of a site</span></span>

> <span data-ttu-id="e8a0c-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e8a0c-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8a0c-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8a0c-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e8a0c-105">Возвращает метаданные для [sitePage][] страниц сайта [списка][] на [сайте][].</span><span class="sxs-lookup"><span data-stu-id="e8a0c-105">Returns the metadata for a [sitePage][] in the site pages [list][] in a [site][].</span></span>

[sitePage]: ../resources/sitepage.md
[list]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="e8a0c-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e8a0c-109">Permissions</span></span>

<span data-ttu-id="e8a0c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8a0c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8a0c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8a0c-112">Permission type</span></span>      | <span data-ttu-id="e8a0c-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8a0c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8a0c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8a0c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e8a0c-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8a0c-115">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e8a0c-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8a0c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8a0c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8a0c-117">Not supported.</span></span>    |
|<span data-ttu-id="e8a0c-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8a0c-118">Application</span></span> | <span data-ttu-id="e8a0c-119">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8a0c-119">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8a0c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8a0c-120">HTTP request</span></span>

```http
GET /sites/{site-id}/pages/{page-id}
```

## <a name="example"></a><span data-ttu-id="e8a0c-121">Пример</span><span class="sxs-lookup"><span data-stu-id="e8a0c-121">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e8a0c-122">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8a0c-122">Request</span></span>

<!-- { "blockType": "request", "name": "get-page", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
GET /sites/{site-id}/pages/{page-id}
```

##### <a name="response"></a><span data-ttu-id="e8a0c-123">Ответ</span><span class="sxs-lookup"><span data-stu-id="e8a0c-123">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.sitePage", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": 2,
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

<!-- {
  "type": "#page.annotation",
  "description": "Get a page in a site",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Pages/Enumerate"
} -->
