---
author: rahmit
description: Создайте новый Ситепаже в списке страниц сайта на сайте.
ms.date: 05/07/2018
title: Создание новой страницы на сайте SharePoint
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 5ddedd4932e0c2061bcfe3bfac6a52879a3f2b73
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870891"
---
# <a name="create-a-page-in-the-site-pages-list-of-a-site"></a><span data-ttu-id="7be1f-103">Создание страницы в списке страниц сайта</span><span class="sxs-lookup"><span data-stu-id="7be1f-103">Create a page in the site pages list of a site</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7be1f-104">Создайте новый [ситепаже][] в [списке][] страниц сайта на [сайте][].</span><span class="sxs-lookup"><span data-stu-id="7be1f-104">Create a new [sitePage][] in the site pages [list][] in a [site][].</span></span>

## <a name="permissions"></a><span data-ttu-id="7be1f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7be1f-105">Permissions</span></span>

<span data-ttu-id="7be1f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7be1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7be1f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7be1f-108">Permission type</span></span>      | <span data-ttu-id="7be1f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7be1f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7be1f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7be1f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7be1f-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7be1f-111">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7be1f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7be1f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7be1f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7be1f-113">Not supported.</span></span>    |
|<span data-ttu-id="7be1f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7be1f-114">Application</span></span> | <span data-ttu-id="7be1f-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7be1f-115">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7be1f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7be1f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/pages
```

## <a name="request-body"></a><span data-ttu-id="7be1f-117">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7be1f-117">Request body</span></span>

<span data-ttu-id="7be1f-118">В теле запроса добавьте представление ресурса [ситепаже][] , который требуется создать, в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7be1f-118">In the request body, supply a JSON representation of the [sitePage][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="7be1f-119">Пример</span><span class="sxs-lookup"><span data-stu-id="7be1f-119">Example</span></span>

<span data-ttu-id="7be1f-120">В приведенном ниже примере показано, как создать новую страницу.</span><span class="sxs-lookup"><span data-stu-id="7be1f-120">The following example shows how to create a new page.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7be1f-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="7be1f-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-page", "scopes": "sites.readwrite.all" } -->

```json
POST /sites/{site-id}/pages
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7be1f-122">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7be1f-122">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-page-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="7be1f-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="7be1f-123">Response</span></span>

<span data-ttu-id="7be1f-124">В случае успешного выполнения этот метод возвращает объект [ситепаже][] в тексте отклика для созданной страницы.</span><span class="sxs-lookup"><span data-stu-id="7be1f-124">If successful, this method returns a [sitePage][] in the response body for the created page.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.sitePage", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "2",
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

<span data-ttu-id="7be1f-125">**Примечание.** Ответ усечен для наглядности.</span><span class="sxs-lookup"><span data-stu-id="7be1f-125">**Note:** The response object is truncated for clarity.</span></span> <span data-ttu-id="7be1f-126">При фактическом вызове будут возвращены свойства, используемые по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7be1f-126">Default properties will be returned from the actual call.</span></span>

[list]: ../resources/list.md
[listItem]: ../resources/listitem.md
[site]: ../resources/site.md
[sitePage]: ../resources/sitepage.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a sitePage in the SitePages list in a site.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Pages/Create",
  "suppressions": []
}
-->
