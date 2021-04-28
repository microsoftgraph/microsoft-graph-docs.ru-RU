---
title: Используйте API поиска Майкрософт в Microsoft Graph для запроса исправлений орфографии
description: API поиска Майкрософт можно использовать для получения предложения орфографии или изменения орфографии для поиска.
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 9d7f935f2de7e0777679266fc479b302fcfaf2a9
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067755"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-request-spelling-correction-preview"></a><span data-ttu-id="9823d-103">Используйте API поиска Майкрософт в Microsoft Graph, чтобы запросить исправление орфографии (предварительный просмотр)</span><span class="sxs-lookup"><span data-stu-id="9823d-103">Use the Microsoft Search API in Microsoft Graph to request spelling correction (preview)</span></span>

<span data-ttu-id="9823d-104">API поиска Майкрософт можно использовать для запроса исправлений орфографии для обработки несоответствий между опечатками в запросах пользователей и правильными словами в содержимом.</span><span class="sxs-lookup"><span data-stu-id="9823d-104">You can use the Microsoft Search API to request spelling corrections to handle mismatches between typos in user queries and correct words in matched contents.</span></span> <span data-ttu-id="9823d-105">Чтобы запросить исправления орфографии, укажите следующие свойства в **свойстве requestAlterationOptions** тела запроса [метода](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) запроса:</span><span class="sxs-lookup"><span data-stu-id="9823d-105">To request spelling corrections, specify the following properties in the **queryAlterationOptions** property of request body of the [query](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) method:</span></span>

- <span data-ttu-id="9823d-106">**enableSuggestion** для включения и отключения предложений орфографии для запроса пользователя.</span><span class="sxs-lookup"><span data-stu-id="9823d-106">**enableSuggestion** to enable/disable spelling suggestions for the user query.</span></span> <span data-ttu-id="9823d-107">Вы можете передать, чтобы получить рекомендуемые сведения об исправлении орфографии для `true` опечаток в запросе пользователя.</span><span class="sxs-lookup"><span data-stu-id="9823d-107">You can pass `true` to get the suggested spelling correction information for typos in the user query.</span></span>

- <span data-ttu-id="9823d-108">**enableModification,** чтобы включить/отключить изменения орфографии для пользовательского запроса.</span><span class="sxs-lookup"><span data-stu-id="9823d-108">**enableModification** to enable/disable spelling modifications for the user query.</span></span> <span data-ttu-id="9823d-109">Вы можете передать, чтобы получить результаты поиска для исправленного запроса, если нет результатов для исходного запроса с опечатки, и получить соответствующие `true` сведения о  исправлении.</span><span class="sxs-lookup"><span data-stu-id="9823d-109">You can pass `true` to get the search results for the corrected query *when there are no results* for the original query with typos, and get the corresponding correction information.</span></span>

<span data-ttu-id="9823d-110">Приоритет изменения орфографии выше, чем предложение орфографии, если они включены.</span><span class="sxs-lookup"><span data-stu-id="9823d-110">The priority of spelling modification is higher than spelling suggestion if they are both enabled.</span></span>

<span data-ttu-id="9823d-111">Все строки запросов пользователей должны быть одинаковыми, чтобы включить исправления орфографии для поиска нескольких сущностями.</span><span class="sxs-lookup"><span data-stu-id="9823d-111">All the user query strings should be the same to enable spelling corrections for searches of multiple entities.</span></span>

## <a name="example-1-request-spelling-suggestions"></a><span data-ttu-id="9823d-112">Пример 1. Запрос предложений по написанию</span><span class="sxs-lookup"><span data-stu-id="9823d-112">Example 1: Request spelling suggestions</span></span>

<span data-ttu-id="9823d-113">В следующем примере запрашиваются **ресурсы listItem,** содержащие строку "учетная запись", и запрашивается предложение орфографии для запроса.</span><span class="sxs-lookup"><span data-stu-id="9823d-113">The following example queries **listItem** resources that contain the string "accountt" and requests a spelling suggestion for the query.</span></span>

<span data-ttu-id="9823d-114">Ответ содержит [объекты alterationResponse](/graph/api/resources/alterationResponse?view=graph-rest-beta&preserve-view=true) для предложения орфографии.</span><span class="sxs-lookup"><span data-stu-id="9823d-114">The response contains [alterationResponse](/graph/api/resources/alterationResponse?view=graph-rest-beta&preserve-view=true) objects for the spelling suggestion.</span></span>

### <a name="request"></a><span data-ttu-id="9823d-115">Запрос</span><span class="sxs-lookup"><span data-stu-id="9823d-115">Request</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json

{
    "requests": [
        {
            "entityTypes": [
                "listItem"
            ],
            "query": {
                "queryString": "accountt"
            },
            "from": 0,
            "size": 25
        }
    ],
    "queryAlterationOptions": {
        "enableSuggestion": true,
        "enableModification": false
    }
}
```

### <a name="response"></a><span data-ttu-id="9823d-116">Отклик</span><span class="sxs-lookup"><span data-stu-id="9823d-116">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.searchResponse)",
    "value": [
        {
            "searchTerms": [
                "accountt"
            ],
            "hitsContainers": [
                {
                    "total": 0,
                    "moreResultsAvailable": false
                }
            ]
        }
    ],
    "queryAlterationResponse": {
        "@odata.type": "#microsoft.substrateSearch.alterationResponse",
        "originalQueryString": "accountt",
        "queryAlteration": {
            "@odata.type": "#microsoft.substrateSearch.searchAlteration",
            "alteredQueryString": "account",
            "alteredHighlightedQueryString": "account",
            "alteredQueryTokens": [
                {
                    "offset": 0,
                    "length": 8,
                    "suggestion": "account"
                }
            ]
        },
        "queryAlterationType": "Suggestion"
    }
}
```

## <a name="example-2-request-spelling-modifications"></a><span data-ttu-id="9823d-117">Пример 2. Запрос на изменения орфографии</span><span class="sxs-lookup"><span data-stu-id="9823d-117">Example 2: Request spelling modifications</span></span>

<span data-ttu-id="9823d-118">В следующем примере запрашиваются **ресурсы listItem,** содержащие строку "учетная запись", и запрашивается изменение орфографии для запроса.</span><span class="sxs-lookup"><span data-stu-id="9823d-118">The following example queries **listItem** resources that contain the string "accountt" and requests a spelling modification for the query.</span></span>

<span data-ttu-id="9823d-119">В этом примере нет результатов для исходного запроса с помощью опечатки "учетная запись".</span><span class="sxs-lookup"><span data-stu-id="9823d-119">In this example, there are no results for original query with typo "accountt".</span></span> <span data-ttu-id="9823d-120">Ответ содержит результаты, связанные с исправленными объектами строки "учетная запись" и [объектами alterationResponse](/graph/api/resources/alterationResponse?view=graph-rest-beta&preserve-view=true) для изменения орфографии.</span><span class="sxs-lookup"><span data-stu-id="9823d-120">The response contains results related to corrected string "account" and [alterationResponse](/graph/api/resources/alterationResponse?view=graph-rest-beta&preserve-view=true) objects for the spelling modification.</span></span>

### <a name="request"></a><span data-ttu-id="9823d-121">Запрос</span><span class="sxs-lookup"><span data-stu-id="9823d-121">Request</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json

{
    "requests": [
        {
            "entityTypes": [
                "listItem"
            ],
            "query": {
                "queryString": "accountt"
            },
            "from": 0,
            "size": 25
        }
    ],
    "queryAlterationOptions": {
        "enableSuggestion": true,
        "enableModification": true
    }
}
```

### <a name="response"></a><span data-ttu-id="9823d-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="9823d-122">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.searchResponse)",
    "value": [
        {
            "searchTerms": [
                "account"
            ],
            "hitsContainers": [
                {
                    "total": 1,
                    "moreResultsAvailable": false,
                    "hits": [
                        {
                            "hitId": "FlULeN/ui/1GjLx1rUfio5UAAEl",
                            "rank": 1,
                            "summary": "",
                            "resource": {
                                "@odata.type": "#microsoft.graph.listItem",
                                "createdDateTime": "2019-06-10T06:37:43Z",
                                "lastModifiedDateTime": "2019-06-10T06:37:43Z",
                                "name": "web_part_test_long Notebook",
                                "webUrl": "https://contoso.sharepoint.com/sites/contoso-team/Lists/Issue tracker list/DispForm.aspx?ID=1",
                                "sharepointIds": {
                                    "listId": "33498de0-d695-4d23-ac26-e1bf95a3206e",
                                    "listItemId": "13"
                                },
                                "createdBy": {
                                    "user": {
                                        "displayName": "System Account"
                                    }
                                },
                                "lastModifiedBy": {
                                    "user": {
                                        "displayName": "System Account"
                                    }
                                },
                                "parentReference": {
                                    "sharepointIds": {
                                        "listId": "da61a2b0-4120-4a3f-812b-0fc0d79bf16b"
                                    },
                                    "siteId": "m365x231305.sharepoint.com,5724d91f-650c-4810-83cc-61a8818917d6,c3ba25dc-2c9f-48cb-83be-74cdf68ea5a0"
                                }
                            }
                        }
                    ]
                }
            ]
        }
    ],
    "queryAlterationResponse": {
        "@odata.type": "#microsoft.substrateSearch.alterationResponse",
        "originalQueryString": "accountt",
        "queryAlteration": {
            "@odata.type": "#microsoft.substrateSearch.searchAlteration",
            "alteredQueryString": "account",
            "alteredHighlightedQueryString": "account",
            "alteredQueryTokens": [
                {
                    "offset": 0,
                    "length": 8,
                    "suggestion": "account"
                }
            ]
        },
        "queryAlterationType": "Modification"
    }
}
```

## <a name="known-limitations"></a><span data-ttu-id="9823d-123">Известные ограничения</span><span class="sxs-lookup"><span data-stu-id="9823d-123">Known limitations</span></span>

<span data-ttu-id="9823d-124">Исправление орфографии поддерживается только для следующих ресурсов: **сообщение,** **событие,** **сайт,** **диск**, **driveItem**, **список**, **listItem** и **externalItem**.</span><span class="sxs-lookup"><span data-stu-id="9823d-124">Spelling correction is only supported for the following resources: **message**, **event**, **site**, **drive**, **driveItem**, **list**, **listItem** and **externalItem**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="9823d-125">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="9823d-125">Next steps</span></span>

- [<span data-ttu-id="9823d-126">Использование API Поиска (Майкрософт) для запроса данных</span><span class="sxs-lookup"><span data-stu-id="9823d-126">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
