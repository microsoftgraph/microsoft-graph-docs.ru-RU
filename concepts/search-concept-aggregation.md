---
title: Использование API службы поиска Microsoft в Microsoft Graph для уточнения запросов с помощью агрегатов
description: Вы можете использовать API службы поиска Microsoft для получения аггреатионс
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 6eb537fa8063281073fbdb12edfb4ec09b88bb93
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563431"
---
# <a name="refine-search-results-using-aggregations-preview"></a><span data-ttu-id="e3d91-103">Уточнение результатов поиска с помощью агрегатов (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="e3d91-103">Refine search results using aggregations (preview)</span></span>

<span data-ttu-id="e3d91-104">Уточните результаты поиска и отобразите их распределение в индексе.</span><span class="sxs-lookup"><span data-stu-id="e3d91-104">Refine search results and show their distribution in the index.</span></span>

## <a name="example-1-request-aggregations-by-string-fields"></a><span data-ttu-id="e3d91-105">Пример 1: запрос агрегатов по строковым полям</span><span class="sxs-lookup"><span data-stu-id="e3d91-105">Example 1: Request aggregations by string fields</span></span>

<span data-ttu-id="e3d91-106">В следующем примере выполняется поиск ресурсов **ListItem** и статистические результаты по их типам файлов и классу контента, которые являются строковыми значениями.</span><span class="sxs-lookup"><span data-stu-id="e3d91-106">The following example searches **listItem** resources and aggregates results by their file type and content class, both of which are string values.</span></span>

<span data-ttu-id="e3d91-107">Ответ включает два объекта [сеарчбуккет](/graph/api/resources/searchbucket?view=graph-rest-beta&preserve-view=true) для двух агрегатов:</span><span class="sxs-lookup"><span data-stu-id="e3d91-107">The response includes two [searchBucket](/graph/api/resources/searchbucket?view=graph-rest-beta&preserve-view=true) objects for the two aggregations:</span></span>
- <span data-ttu-id="e3d91-108">Свойство **Key** указывает фактическое значение (by `FileType` или `contentclass` ) для соответствующих объектов **ListItem** , которые объединены в одном сегменте с этим значением.</span><span class="sxs-lookup"><span data-stu-id="e3d91-108">The **key** property specifies the actual value (by `FileType` or `contentclass`) for those matching **listItem** objects that are aggregated in the same bucket by that value.</span></span>
- <span data-ttu-id="e3d91-109">Свойство **Count** указывает количество таких объектов, собранных в том же сегменте.</span><span class="sxs-lookup"><span data-stu-id="e3d91-109">The **count** property specifies the number of such objects aggregated in the same bucket.</span></span> <span data-ttu-id="e3d91-110">Обратите внимание, что это значение является приближением количества совпадений и не обеспечивает точное количество совпадений.</span><span class="sxs-lookup"><span data-stu-id="e3d91-110">Note that this number is an approximation of the number of matches and will not provide an exact number of matches.</span></span>
- <span data-ttu-id="e3d91-111">Сегменты результатов, агрегированные по типу файла, сортируются по количеству в порядке убывания.</span><span class="sxs-lookup"><span data-stu-id="e3d91-111">Buckets of results aggregated by file type are sorted by count in descending order.</span></span> <span data-ttu-id="e3d91-112">В этом примере для трех типов файлов используется 3 сегмента: `docx` , `xlsx` и `pptx` .</span><span class="sxs-lookup"><span data-stu-id="e3d91-112">In this example, there are 3 buckets for 3 file types: `docx`, `xlsx`, and `pptx`.</span></span>
- <span data-ttu-id="e3d91-113">Сегменты результатов, агрегированные по классу контента, сортируются по строковому значению класса контента в порядке убывания.</span><span class="sxs-lookup"><span data-stu-id="e3d91-113">Buckets of results aggregated by content class are sorted by the string value of the content class in descending order.</span></span> <span data-ttu-id="e3d91-114">В этом примере существует только один сегмент со всеми связанными объектами, совместно использующих один и тот же класс контента `STS_ListItem_DocumentLibrary` .</span><span class="sxs-lookup"><span data-stu-id="e3d91-114">In this example, there is only one bucket with all the matching objects sharing the same content class, `STS_ListItem_DocumentLibrary`.</span></span>

### <a name="request"></a><span data-ttu-id="e3d91-115">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3d91-115">Request</span></span>

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
          "queryString": "test"
      },
      "from": 0,
      "size": 25,
      "aggregations": [
          {
              "field": "FileType",
              "size": 20,
              "bucketDefinition": {
                  "sortBy": "count",
                  "isDescending": "true",
                  "minimumCount": 0
              }
          },
          {
              "field": "contentclass",
              "size": 15,
              "bucketDefinition": {
                  "sortBy": "keyAsString",
                  "isDescending": "true",
                  "minimumCount": 0
              }
          }
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="e3d91-116">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3d91-116">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.searchResponse",
    "hitsContainers": [
        {
            "@odata.type": "#microsoft.graph.searchHitsContainer",
            "hits": [
                "..."
            ],
            "total": 9,
            "moreResultsAvailable": false,
            "aggregations": [
                {
                    "@odata.type": "#microsoft.substrateSearch.searchAggregation",
                    "field": "FileType",
                    "buckets": [
                        {
                            "@odata.type": "#microsoft.substrateSearch.searchBucket",
                            "key": "docx",
                            "count": 5,
                            "aggregationFilterToken": "\"ǂǂ646f6378\""
                        },
                        {
                            "@odata.type": "#microsoft.substrateSearch.searchBucket",
                            "key": "xlsx",
                            "count": 3,
                            "aggregationFilterToken": "\"ǂǂ786c7378\""
                        },
                        {
                            "@odata.type": "#microsoft.substrateSearch.searchBucket",
                            "key": "pptx",
                            "count": 1,
                            "aggregationFilterToken": "\"ǂǂ70707478\""
                        }
                    ]
                },
                {
                    "@odata.type": "#microsoft.substrateSearch.searchAggregation",
                    "field": "contentclass",
                    "buckets": [
                        {
                            "@odata.type": "#microsoft.substrateSearch.searchBucket",
                            "key": "STS_ListItem_DocumentLibrary",
                            "count": 9,
                            "aggregationFilterToken": "\"ǂǂ5354535f4c6973744974656d5f446f63756d656e744c696272617279\""
                        }
                    ]
                }
            ]
        }
    ]
}
```

## <a name="example-2-apply-an-aggregation-filter-based-on-a-previous-request"></a><span data-ttu-id="e3d91-117">Пример 2: применение фильтра агрегирования на основе предыдущего запроса</span><span class="sxs-lookup"><span data-stu-id="e3d91-117">Example 2: Apply an aggregation filter based on a previous request</span></span>

<span data-ttu-id="e3d91-118">В этом примере применяется фильтр агрегирования, основанный на **аггрегатионфилтертокен** , возвращенном для `docx` `FileType` поля в примере 1.</span><span class="sxs-lookup"><span data-stu-id="e3d91-118">In this example, we apply an aggregation filter that is based on the **aggregationFilterToken** returned for `docx` as the `FileType` field in example 1.</span></span>

<span data-ttu-id="e3d91-119">Строковое значение, назначенное свойству **аггрегатионфилтерс** , соответствует формату **"{Field}: \\ " {аггрегатионфилтертокен} \\ ""**.</span><span class="sxs-lookup"><span data-stu-id="e3d91-119">The string value assigned to the **aggregationFilters** property follows the format **"{field}:\\"{aggregationFilterToken}\\""**.</span></span>

### <a name="request"></a><span data-ttu-id="e3d91-120">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3d91-120">Request</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
          "driveItem"
      ],
      "query": {
          "queryString": "test"
      },
      "from": 0,
      "size": 20,
      "aggregations": [
          {
              "field": "FileType",
              "size": 10,
              "bucketDefinition": {
                  "sortBy": "count",
                  "isDescending": "true",
                  "minimumCount": 0
              }
          }
      ],
      "aggregationFilters": [
        "FileType:\"ǂǂ68746d6c\""
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="e3d91-121">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3d91-121">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.searchResponse",
    "hitsContainers": [
        {
            "@odata.type": "#microsoft.graph.searchHitsContainer",
            "hits": [
                "..."
            ],
            "total": 69960,
            "moreResultsAvailable": true,
            "aggregations": [
            {
                "@odata.type": "#microsoft.substrateSearch.searchAggregation",
                "field": "FileType",
                "buckets": [
                    {
                        "@odata.type": "#microsoft.substrateSearch.searchBucket",
                        "key": "html",
                        "count": 69960,
                        "aggregationFilterToken": "\"ǂǂ68746d6c\""
                    }
                ]
            }
        ]
        }
    ]
}
```

## <a name="example-3-request-aggregation-by-a-numeric-field"></a><span data-ttu-id="e3d91-122">Пример 3: запрос агрегирования с помощью числового поля</span><span class="sxs-lookup"><span data-stu-id="e3d91-122">Example 3: Request aggregation by a numeric field</span></span>

<span data-ttu-id="e3d91-123">В следующем примере выполняется поиск ресурсов **driveItem** и статистические результаты по их размеру — числовому значению.</span><span class="sxs-lookup"><span data-stu-id="e3d91-123">The following example searches **driveItem** resources and aggregates results by their size which is a numeric value.</span></span> <span data-ttu-id="e3d91-124">В запросе задается объединение по 3 диапазонам размера:</span><span class="sxs-lookup"><span data-stu-id="e3d91-124">The request specifies aggregation by 3 size ranges:</span></span>
- <span data-ttu-id="e3d91-125">Размер менее 100</span><span class="sxs-lookup"><span data-stu-id="e3d91-125">Size less than 100</span></span>
- <span data-ttu-id="e3d91-126">Размер между 100 и 1000</span><span class="sxs-lookup"><span data-stu-id="e3d91-126">Size between 100 and 1000</span></span>
- <span data-ttu-id="e3d91-127">Размер 1000 и выше</span><span class="sxs-lookup"><span data-stu-id="e3d91-127">Size 1000 and higher</span></span>

<span data-ttu-id="e3d91-128">Ответ включает 3 объекта **сеарчбуккет** , по одному для каждого объединения диапазонов размеров:</span><span class="sxs-lookup"><span data-stu-id="e3d91-128">The response includes 3 **searchBucket** objects, one for each size range aggregation:</span></span>
- <span data-ttu-id="e3d91-129">2 сегмента из диапазонов меньшего размера не содержат совпадений поиска.</span><span class="sxs-lookup"><span data-stu-id="e3d91-129">The 2 buckets of the lower size ranges don't include any search matches.</span></span>
- <span data-ttu-id="e3d91-130">Все 9 совпадений поиска имеют размеры 1000 или выше.</span><span class="sxs-lookup"><span data-stu-id="e3d91-130">All 9 search matches have sizes 1000 or higher.</span></span>

### <a name="request"></a><span data-ttu-id="e3d91-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3d91-131">Request</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json

{
    "requests": [
        {
            "entityTypes": [
                "driveItem"
            ],
            "query": {
                "queryString": "test"
            },
            "from": 0,
            "size": 10,
            "aggregations": [
                {
                    "field": "Size",
                    "size": 5,
                    "bucketDefinition": {
                        "sortBy": "keyAsNumber",
                        "isDescending": "true",
                        "minimumCount": 0,
                        "ranges": [
                            {
                                "to": "100"
                            },
                            {
                                "from": "100",
                                "to": "1000"
                            },
                            {
                                "from": "1000"
                            }
                        ]
                    }
                }
            ]
        }
    ]
}
```

### <a name="response"></a><span data-ttu-id="e3d91-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3d91-132">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.searchResponse",
    "hitsContainers": [
        {
            "@odata.type": "#microsoft.graph.searchHitsContainer",
            "hits": [
                "..."
                    ],
            "total": 9,
            "moreResultsAvailable": false,
            "aggregations": [
                {
                    "@odata.type": "#microsoft.substrateSearch.searchAggregation",
                    "field": "Size",
                    "buckets": [
                        {
                            "@odata.type": "#microsoft.substrateSearch.searchBucket",
                            "key": "Less than 100",
                            "count": 0,
                            "aggregationFilterToken": "range(min, 100)"
                        },
                        {
                            "@odata.type": "#microsoft.substrateSearch.searchBucket",
                            "key": "100 up to 1000",
                            "count": 0,
                            "aggregationFilterToken": "range(100, 1000)"
                        },
                        {
                            "@odata.type": "#microsoft.substrateSearch.searchBucket",
                            "key": "1000 and up",
                            "count": 9,
                            "aggregationFilterToken": "range(1000, max, to=\"le\")"
                        }
                    ]
                }
            ]
        }
    ]
}
```

## <a name="known-limitations"></a><span data-ttu-id="e3d91-133">Известные ограничения</span><span class="sxs-lookup"><span data-stu-id="e3d91-133">Known limitations</span></span>

<span data-ttu-id="e3d91-134">Агрегаты поддерживаются только для элементов SharePoint или OneDrive.</span><span class="sxs-lookup"><span data-stu-id="e3d91-134">Aggregations are supported only for SharePoint or OneDrive items.</span></span> <span data-ttu-id="e3d91-135">Они не поддерживаются для **сообщений** или **событий**.</span><span class="sxs-lookup"><span data-stu-id="e3d91-135">They are not supported for **message** or **event**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e3d91-136">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="e3d91-136">Next steps</span></span>

- [<span data-ttu-id="e3d91-137">Использование API Поиска (Майкрософт) для запроса данных</span><span class="sxs-lookup"><span data-stu-id="e3d91-137">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
