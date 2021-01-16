---
title: Использование API Поиска (Майкрософт) в запросах уточнения Microsoft Graph с агрегациями
description: Вы можете использовать API Поиска (Майкрософт) для получения агрегации
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: fad049649172750cf2e362d2558cfc247467a6ed
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883195"
---
# <a name="refine-search-results-using-aggregations-preview"></a><span data-ttu-id="0953e-103">Уточнение результатов поиска с помощью агрегаций (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="0953e-103">Refine search results using aggregations (preview)</span></span>

<span data-ttu-id="0953e-104">Уточнение результатов поиска и их распространение в индексе.</span><span class="sxs-lookup"><span data-stu-id="0953e-104">Refine search results and show their distribution in the index.</span></span>

## <a name="example-1-request-aggregations-by-string-fields"></a><span data-ttu-id="0953e-105">Пример 1. Запрос агрегации по строкам</span><span class="sxs-lookup"><span data-stu-id="0953e-105">Example 1: Request aggregations by string fields</span></span>

<span data-ttu-id="0953e-106">В следующем примере выполняется поиск ресурсов **listItem** и объединяются результаты по типу файла и классу контента, оба из которых являются строками.</span><span class="sxs-lookup"><span data-stu-id="0953e-106">The following example searches **listItem** resources and aggregates results by their file type and content class, both of which are string values.</span></span>

<span data-ttu-id="0953e-107">Ответ включает два [объекта searchBucket](/graph/api/resources/searchbucket?view=graph-rest-beta&preserve-view=true) для двух агрегаций:</span><span class="sxs-lookup"><span data-stu-id="0953e-107">The response includes two [searchBucket](/graph/api/resources/searchbucket?view=graph-rest-beta&preserve-view=true) objects for the two aggregations:</span></span>
- <span data-ttu-id="0953e-108">Свойство **ключа** указывает фактическое значение (по или) для совпадающих объектов `FileType` `contentclass` **listItem,** которые объединяются в одном сегменте по этому значению.</span><span class="sxs-lookup"><span data-stu-id="0953e-108">The **key** property specifies the actual value (by `FileType` or `contentclass`) for those matching **listItem** objects that are aggregated in the same bucket by that value.</span></span>
- <span data-ttu-id="0953e-109">Свойство **count** указывает количество таких объектов, агрегированных в одном сегменте.</span><span class="sxs-lookup"><span data-stu-id="0953e-109">The **count** property specifies the number of such objects aggregated in the same bucket.</span></span> <span data-ttu-id="0953e-110">Обратите внимание, что это число соответствует количеству совпадений и не предоставляет точное количество совпадений.</span><span class="sxs-lookup"><span data-stu-id="0953e-110">Note that this number is an approximation of the number of matches and will not provide an exact number of matches.</span></span>
- <span data-ttu-id="0953e-111">Сегменты результатов, агрегированных по типу файла, сортируются по подсчету в порядке убывания.</span><span class="sxs-lookup"><span data-stu-id="0953e-111">Buckets of results aggregated by file type are sorted by count in descending order.</span></span> <span data-ttu-id="0953e-112">В этом примере имеется 3 сегмента для 3 типов файлов: `docx` `xlsx` , и `pptx` .</span><span class="sxs-lookup"><span data-stu-id="0953e-112">In this example, there are 3 buckets for 3 file types: `docx`, `xlsx`, and `pptx`.</span></span>
- <span data-ttu-id="0953e-113">Сегменты результатов, агрегированных по классу контента, сортируются по строковому значению класса контента в порядке убывания.</span><span class="sxs-lookup"><span data-stu-id="0953e-113">Buckets of results aggregated by content class are sorted by the string value of the content class in descending order.</span></span> <span data-ttu-id="0953e-114">В этом примере имеется только один контейнер со всеми совпадающие объекты, совместно с одним классом `STS_ListItem_DocumentLibrary` контента.</span><span class="sxs-lookup"><span data-stu-id="0953e-114">In this example, there is only one bucket with all the matching objects sharing the same content class, `STS_ListItem_DocumentLibrary`.</span></span>

### <a name="request"></a><span data-ttu-id="0953e-115">Запрос</span><span class="sxs-lookup"><span data-stu-id="0953e-115">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="0953e-116">Отклик</span><span class="sxs-lookup"><span data-stu-id="0953e-116">Response</span></span>

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

## <a name="example-2-apply-an-aggregation-filter-based-on-a-previous-request"></a><span data-ttu-id="0953e-117">Пример 2. Применение фильтра агрегации на основе предыдущего запроса</span><span class="sxs-lookup"><span data-stu-id="0953e-117">Example 2: Apply an aggregation filter based on a previous request</span></span>

<span data-ttu-id="0953e-118">В этом примере применяется фильтр агрегации, основанный на **возвращаемом в** качестве поля в примере `docx` `FileType` 1.</span><span class="sxs-lookup"><span data-stu-id="0953e-118">In this example, we apply an aggregation filter that is based on the **aggregationFilterToken** returned for `docx` as the `FileType` field in example 1.</span></span>

<span data-ttu-id="0953e-119">Строка, назначенная свойству **aggregationFilters,** имеет формат **"{field}: \\ "{aggregationFilterToken} \\ ""**.</span><span class="sxs-lookup"><span data-stu-id="0953e-119">The string value assigned to the **aggregationFilters** property follows the format **"{field}:\\"{aggregationFilterToken}\\""**.</span></span> <span data-ttu-id="0953e-120">Если для одного фильтра требуется несколько значений, строка, назначенная свойству **aggregationFilters,** должна иметь такой формат: **"{field}:or( \\ "{aggregationFilterToken1} \\ ", \\ "{aggregationFilterToken2} \\ ")"**.</span><span class="sxs-lookup"><span data-stu-id="0953e-120">If multiple values for the same filter are required, the string value assigned to the **aggregationFilters** property should follow this format : **"{field}:or(\\"{aggregationFilterToken1}\\",\\"{aggregationFilterToken2}\\")"**.</span></span>

### <a name="request"></a><span data-ttu-id="0953e-121">Запрос</span><span class="sxs-lookup"><span data-stu-id="0953e-121">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="0953e-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="0953e-122">Response</span></span>

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

## <a name="example-3-request-aggregation-by-a-numeric-field"></a><span data-ttu-id="0953e-123">Пример 3. Запрос агрегации по числовому полю</span><span class="sxs-lookup"><span data-stu-id="0953e-123">Example 3: Request aggregation by a numeric field</span></span>

<span data-ttu-id="0953e-124">В следующем примере выполняется поиск ресурсов **driveItem** и объединяются результаты по их размеру, который является числом.</span><span class="sxs-lookup"><span data-stu-id="0953e-124">The following example searches **driveItem** resources and aggregates results by their size which is a numeric value.</span></span> <span data-ttu-id="0953e-125">Запрос определяет агрегацию на 3 диапазона размеров:</span><span class="sxs-lookup"><span data-stu-id="0953e-125">The request specifies aggregation by 3 size ranges:</span></span>
- <span data-ttu-id="0953e-126">Размер меньше 100</span><span class="sxs-lookup"><span data-stu-id="0953e-126">Size less than 100</span></span>
- <span data-ttu-id="0953e-127">Размер от 100 до 1000</span><span class="sxs-lookup"><span data-stu-id="0953e-127">Size between 100 and 1000</span></span>
- <span data-ttu-id="0953e-128">Размер 1000 и выше</span><span class="sxs-lookup"><span data-stu-id="0953e-128">Size 1000 and higher</span></span>

<span data-ttu-id="0953e-129">Ответ включает 3 **объекта searchBucket,** по одному для каждого агрегирования диапазона размеров:</span><span class="sxs-lookup"><span data-stu-id="0953e-129">The response includes 3 **searchBucket** objects, one for each size range aggregation:</span></span>
- <span data-ttu-id="0953e-130">2 сегмента диапазонов меньшего размера не включают совпадения поиска.</span><span class="sxs-lookup"><span data-stu-id="0953e-130">The 2 buckets of the lower size ranges don't include any search matches.</span></span>
- <span data-ttu-id="0953e-131">Размер всех 9 совпадений поиска не превышает 1000.</span><span class="sxs-lookup"><span data-stu-id="0953e-131">All 9 search matches have sizes 1000 or higher.</span></span>

### <a name="request"></a><span data-ttu-id="0953e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0953e-132">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="0953e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="0953e-133">Response</span></span>

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

## <a name="known-limitations"></a><span data-ttu-id="0953e-134">Известные ограничения</span><span class="sxs-lookup"><span data-stu-id="0953e-134">Known limitations</span></span>

<span data-ttu-id="0953e-135">Агрегации поддерживаются только для элементов SharePoint или OneDrive.</span><span class="sxs-lookup"><span data-stu-id="0953e-135">Aggregations are supported only for SharePoint or OneDrive items.</span></span> <span data-ttu-id="0953e-136">Они не поддерживаются для **сообщения или** **события.**</span><span class="sxs-lookup"><span data-stu-id="0953e-136">They are not supported for **message** or **event**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="0953e-137">Следующие шаги</span><span class="sxs-lookup"><span data-stu-id="0953e-137">Next steps</span></span>

- [<span data-ttu-id="0953e-138">Использование API Поиска (Майкрософт) для запроса данных</span><span class="sxs-lookup"><span data-stu-id="0953e-138">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
