---
title: Используйте API Поиск (Майкрософт) в Microsoft Graph для уточнения запросов с помощью агрегаций
description: Вы можете использовать API Поиск (Майкрософт) для получения обострений
author: nmoreau
ms.localizationpriority: medium
ms.prod: search
ms.openlocfilehash: 49e3739985f2a715449ff28c1183d0427543b2c5
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285086"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-refine-queries-with-aggregations"></a>Используйте API Поиск (Майкрософт) в Microsoft Graph для уточнения запросов с помощью агрегаций

Вы можете использовать Поиск (Майкрософт) API в Microsoft Graph для уточнения результатов поиска и демонстрации их распространения в индексе. 

Чтобы уточнить результаты, в [запросе поиска](/graph/api/resources/searchRequest?view=graph-rest-beta&preserve-view=true)укажите [aggregationOption](/graph/api/resources/aggregationOption?view=graph-rest-beta&preserve-view=true). Каждое **aggregationOption** указывает свойство, на котором должна быть вычисляется агрегация, и количество элементов [searchBucket,](/graph/api/resources/searchBucket?view=graph-rest-beta&preserve-view=true) которые будут возвращены в ответе.

## <a name="example-1-request-aggregations-by-string-fields"></a>Пример 1. Запрос агрегации по полям строк

В следующем примере поиск **ресурсов listItem** и агрегируется по типу файла, классу контента и последнему измененным времени, все из которых являются значениями строки.

Ответ включает два [объекта searchBucket](/graph/api/resources/searchbucket?view=graph-rest-beta&preserve-view=true) для двух агрегаций:
- Свойство **key** указывает фактическое значение (по , или) для тех объектов `fileType` `contentclass` `lastModifiedTime` **listItem,** которые агрегируются в одном ведре по этому значению.
- Свойство **count** указывает количество таких объектов, агрегированных в одном ведре. Обратите внимание, что это число является приближением количества совпадений и не будет предоставлять точное число совпадений.
- Ведра результатов, агрегированных по типу файла, сортируются по подсчету в порядке убывания. В этом примере 3 ведра для 3 типов файлов: `docx` `xlsx` и `pptx` .
- Ведра результатов, агрегированных классом контента, сортируются по строковому значению класса контента в порядке убывания. В этом примере имеется только одно ведро со всеми объектами, совпадающие с одним классом контента, `STS_ListItem_DocumentLibrary` .
- Ведерки результатов, агрегированные lastModifiedTime, сортируются по строковому значению lastModifiedTime в порядке убывания. В этом примере содержится три ведра: `Before 2021-09-01T09:08:19.6224752Z` `From 2021-09-01T09:08:19.6224752Z up to 2021-11-09T09:08:19.6224752Z` и `2021-11-09T09:08:19.6224752Z or later` .

### <a name="request"></a>Запрос

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
              "field": "fileType",
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
          },
          {
              "field": "lastModifiedTime",
              "size": 2,
              "bucketDefinition": {
                  "sortBy": "KeyAsString",
                  "isDescending": "true",
                  "minimumCount": 0,
                  "ranges": [
                      {
                          "to": "2021-09-01T09:08:19.6224752Z"
                      },
                      {
                          "from": "2021-09-01T09:08:19.6224752Z",
                          "to": "2021-11-09T09:08:19.6224752Z"
                      },
                      {
                          "from": "2021-11-09T09:08:19.6224752Z"
                      }
                ]
              }
          }
      ]
    }
  ]
}
```

### <a name="response"></a>Отклик

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
                    "field": "fileType",
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
                },
                {
                    "@odata.type": "#microsoft.substrateSearch.searchAggregation",
                    "field": "lastModifiedTime",
                    "buckets": [
                        {
                            "key": "Before 2021-09-01T09:08:19.6224752Z",
                            "count": 5,
                            "aggregationFilterToken": "range(min, 2021-09-01T09:08:19.6224752Z)"
                        },
                        {
                            "key": "From 2021-09-01T09:08:19.6224752Z up to 2021-11-09T09:08:19.6224752Z",
                            "count": 3,
                            "aggregationFilterToken": "range(2021-09-01T09:08:19.6224752Z, 2021-11-09T09:08:19.6224752Z)"
                        },
                        {
                            "key": "2021-11-09T09:08:19.6224752Z or later",
                            "count": 1,
                            "aggregationFilterToken": "range(2021-11-09T09:08:19.6224752Z, max, to=\"le\")"
                        }
                    ]
                }
            ]
        }
    ]
}
```

## <a name="example-2-apply-an-aggregation-filter-based-on-a-previous-request"></a>Пример 2. Применение фильтра агрегации на основе предыдущего запроса

В этом примере применяется фильтр агрегации, основанный на **aggregationFilterToken,** возвращаемом в качестве поля и поля в примере `docx` `fileType` `From 2021-09-01T09:08:19.6224752Z up to 2021-11-09T09:08:19.6224752Z` `lastModifiedTime` 1.

Значение строки, назначенное свойству **aggregationFilters,** следует **формату "{field}: \\ "{aggregationFilterToken} \\ """**. Если для одного фильтра требуется несколько значений, строковая величина, назначенная свойству **aggregationFilters,** должна следовать этому формату: **"{field}:or( \\ "{aggregationFilterToken1} \\ ", \\ {aggregationFilterToken2} \\ ") ".**

Значение строки форматирования дат, назначенное свойству **aggregationFilters,** следует **формату "{field}:{aggregationFilterToken}".**


### <a name="request"></a>Запрос

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
              "field": "fileType",
              "size": 10,
              "bucketDefinition": {
                  "sortBy": "count",
                  "isDescending": "true",
                  "minimumCount": 0
              }
          }
      ],
      "aggregationFilters": [
        "fileType:\"ǂǂ68746d6c\"",
        "lastModifiedTime:range(2021-09-01T09:08:19.6224752Z, 2021-11-09T09:08:19.6224752Z)"
      ]
    }
  ]
}
```

### <a name="response"></a>Отклик

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
                    "field": "fileType",
                    "buckets": [
                        {
                            "@odata.type": "#microsoft.substrateSearch.searchBucket",
                            "key": "html",
                            "count": 69960,
                            "aggregationFilterToken": "\"ǂǂ68746d6c\""
                        }
                    ]
                },
                {
                    "@odata.type": "#microsoft.substrateSearch.searchAggregation",
                    "field": "lastModifiedTime",
                    "buckets": [
                        {
                            "key": "Before 2021-09-01T09:08:19.6224752Z",
                            "count": 0,
                            "aggregationFilterToken": "range(min, 2021-09-01T09:08:19.6224752Z)"
                        },
                        {
                            "key": "From 2021-09-01T09:08:19.6224752Z up to 2021-11-09T09:08:19.6224752Z",
                            "count": 69960,
                            "aggregationFilterToken": "range(2021-09-01T09:08:19.6224752Z, 2021-11-09T09:08:19.6224752Z)"
                        },
                        {
                            "key": "2021-11-09T09:08:19.6224752Z or later",
                            "count": 0,
                            "aggregationFilterToken": "range(2021-11-09T09:08:19.6224752Z, max, to=\"le\")"
                        }
                    ]
                }
            ]
        }
    ]
}
```

## <a name="example-3-request-aggregation-by-a-numeric-field"></a>Пример 3. Агрегация запроса по числовому полю

В следующем примере **выполняется поиск ресурсов driveItem** и агрегируется результат по их размеру, который является числимым значением. Запрос указывает агрегацию на 3 диапазона размеров:
- Размер менее 100
- Размер от 100 до 1000
- Размер 1000 и выше

Ответ включает 3 **объекта searchBucket,** по одному для каждого агрегирования диапазона размеров:
- 2 ведра нижних диапазонов размеров не содержат совпадений поиска.
- Все 9 совпадений поиска имеют размер 1000 или более.

### <a name="request"></a>Запрос

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

### <a name="response"></a>Отклик

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

## <a name="known-limitations"></a>Известные ограничения

Агрегации поддерживаются только для SharePoint или OneDrive элементов. Они не поддерживаются для **сообщения или** **события.**

## <a name="next-steps"></a>Дальнейшие действия

- [Использование API Поиска (Майкрософт) для запроса данных](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
