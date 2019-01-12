---
author: rahmit
ms.author: rahmit
ms.date: 05/07/2018
title: Создание новой страницы на сайте SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 112c9f564c549bbae06430d4c2353c26abbac908
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921740"
---
# <a name="create-a-page-in-the-site-pages-list-of-a-site"></a><span data-ttu-id="fccb0-102">Создайте страницу в списке страниц сайта узла</span><span class="sxs-lookup"><span data-stu-id="fccb0-102">Create a page in the site pages list of a site</span></span>

> <span data-ttu-id="fccb0-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fccb0-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fccb0-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fccb0-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fccb0-105">Создание нового [sitePage][] в страниц сайта [списка][] на [сайте][].</span><span class="sxs-lookup"><span data-stu-id="fccb0-105">Create a new [sitePage][] in the site pages [list][] in a [site][].</span></span>

## <a name="permissions"></a><span data-ttu-id="fccb0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fccb0-106">Permissions</span></span>

<span data-ttu-id="fccb0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fccb0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fccb0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fccb0-109">Permission type</span></span>      | <span data-ttu-id="fccb0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fccb0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fccb0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fccb0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fccb0-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fccb0-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="fccb0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fccb0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fccb0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fccb0-114">Not supported.</span></span>    |
|<span data-ttu-id="fccb0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fccb0-115">Application</span></span> | <span data-ttu-id="fccb0-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fccb0-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fccb0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fccb0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/pages
```

## <a name="request-body"></a><span data-ttu-id="fccb0-118">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fccb0-118">Request body</span></span>

<span data-ttu-id="fccb0-119">В тексте запроса укажите представление JSON [sitePage][] ресурсов для создания.</span><span class="sxs-lookup"><span data-stu-id="fccb0-119">In the request body, supply a JSON representation of the [sitePage][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="fccb0-120">Пример</span><span class="sxs-lookup"><span data-stu-id="fccb0-120">Example</span></span>

<span data-ttu-id="fccb0-121">Следующем примере показано, как создать новую страницу.</span><span class="sxs-lookup"><span data-stu-id="fccb0-121">The following example shows how to create a new page.</span></span>

<!-- { "blockType": "request", "name": "create-page", "scopes": "sites.readwrite.all" } -->

```json
POST /sites/{site-id}/page
Content-Type: application/json

{
    "name": "Events.aspx",
    "title": "Team Events",
    "publishingState": {
        "level": "checkedOut",
        "versionId": "0.1"
    },
    "webParts": [
        {
            "type": "rte",
            "innerHTML": "<p>Here are the team's upcoming events:</p>"
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

## <a name="response"></a><span data-ttu-id="fccb0-122">Ответ</span><span class="sxs-lookup"><span data-stu-id="fccb0-122">Response</span></span>

<span data-ttu-id="fccb0-123">Если успешно завершена, этот метод возвращает [sitePage][] в теле ответа для созданного страницы.</span><span class="sxs-lookup"><span data-stu-id="fccb0-123">If successful, this method returns a [sitePage][] in the response body for the created page.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.sitePage", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": 2,
    "eTag": "75bc70e2-6587-45be-8493-c99a956b2e05,7",
    "createdDateTime": "2016-12-06T20:04:40Z",
    "lastModifiedDateTime": "2016-12-06T20:05:09Z",
    "webUrl": "https://www.contoso.com/sites/Engineering/SitePages/Events.aspx",
    "createdBy": {
        "user": {
            "email": "rahmit",
            "id": "1b37d2e1-5000-4648-b431-7dfa509b5660",
            "displayName": "Rahul Mittal"
        }
    },
    "lastModifiedBy": {
        "user": {
            "email": "rahmit",
            "id": "1b37d2e1-5000-4648-b431-7dfa509b5660",
            "displayName": "Rahul Mittal"
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
    "title": "Team Events",
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
                        "baseUrl": "https://www.contoso.com/teams/Engineering"
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

<span data-ttu-id="fccb0-124">**Примечание.** Ответ усечен для наглядности.</span><span class="sxs-lookup"><span data-stu-id="fccb0-124">**Note:** The response object is truncated for clarity.</span></span> <span data-ttu-id="fccb0-125">При фактическом вызове будут возвращены свойства, используемые по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fccb0-125">Default properties will be returned from the actual call.</span></span>

[list]: ../resources/list.md
[listItem]: ../resources/listitem.md
[site]: ../resources/site.md
[sitePage]: ../resources/sitepage.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a sitePage in the SitePages list in a site.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Pages/Create"
} -->
