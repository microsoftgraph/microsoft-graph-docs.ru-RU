---
title: Использование API поиска (Майкрософт) для уточнения запросов с помощью агрегатов
description: Вы можете использовать aggregationOption API поиска (Майкрософт) в Microsoft Graph для уточнения результатов поиска и отображения их распределения в индексе.
author: nmoreau
ms.localizationpriority: medium
ms.prod: search
ms.openlocfilehash: c2bdb3121720a880bf2f508e7c43af2e53226dec
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66443363"
---
# <a name="use-the-microsoft-search-api-to-refine-queries-with-aggregations"></a>Использование API поиска (Майкрософт) для уточнения запросов с помощью агрегатов

API поиска (Майкрософт) в Microsoft Graph можно использовать для уточнения результатов поиска и отображения их распределения в индексе.

Чтобы уточнить результаты, в [поисковом запросе](/graph/api/resources/searchRequest) укажите [параметр aggregationOption](/graph/api/resources/aggregationOption). **Каждый объект aggregationOption** указывает свойство, для которого вычисляется агрегирование, и количество элементов [searchBucket](/graph/api/resources/searchBucket), возвращаемых в ответе.

## <a name="example-1-request-aggregations-by-string-fields"></a>Пример 1. Запрос агрегатов по строковым полям

В следующем примере выполняется поиск ресурсов **listItem** и результаты агрегируются по типу файла, классу контента и времени последнего изменения, все из которых являются строковыми значениями.

Ответ включает два [объекта searchBucket](/graph/api/resources/searchbucket) для двух агрегатов:
- Свойство **ключа** указывает фактическое значение (по `fileType``contentclass``lastModifiedTime`или) для соответствующих объектов **listItem**, которые агрегируются в том же контейнере по этому значению.
- Свойство **count** указывает количество таких объектов, агрегированных в одном контейнере. Обратите внимание, что это число является приближением количества совпадений и не будет предоставлять точное число совпадений.
- Сегменты результатов, агрегированных по типу файла, сортируются по счетчику в порядке убывания. В этом примере существует 3 контейнера для 3 типов файлов: `docx`и `xlsx``pptx`.
- Сегменты результатов, агрегированных по классу контента, сортируются по строковому значению класса контента в порядке убывания. В этом примере существует только один контейнер со всеми соответствующими объектами, совместно используя один и тот же класс содержимого. `STS_ListItem_DocumentLibrary`
- Контейнеры результатов, агрегированные по lastModifiedTime, сортируются по строковому значению lastModifiedTime в порядке убывания. Этот пример включает три контейнера: `Before 2021-09-01T09:08:19.6224752Z`и `From 2021-09-01T09:08:19.6224752Z up to 2021-11-09T09:08:19.6224752Z``2021-11-09T09:08:19.6224752Z or later`.

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

## <a name="example-2-apply-an-aggregation-filter-based-on-a-previous-request"></a>Пример 2. Применение фильтра агрегирования на основе предыдущего запроса

В этом примере применяется фильтр агрегирования, основанный на **объекте aggregationFilterToken** `docx` `fileType` `From 2021-09-01T09:08:19.6224752Z up to 2021-11-09T09:08:19.6224752Z` `lastModifiedTime` , возвращаемом в качестве поля, и в качестве поля в примере 1.

Строковое значение, присвоенное свойству **aggregationFilters**, соответствует формату **"{field}:\\"{aggregationFilterToken}\\".** Если для одного фильтра требуется несколько значений, строковое значение, присвоенное свойству **aggregationFilters** , должно иметь следующий формат: **"{field}:or(\\"{aggregationFilterToken1}\\",\\"{aggregationFilterToken2}\\")"**.

Строковое значение форматирования datetime, присвоенное свойству **aggregationFilters** , соответствует формату **"{field}:{aggregationFilterToken}"**.


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

## <a name="example-3-request-aggregation-by-a-numeric-field"></a>Пример 3. Запрос агрегирования по числовому полю

В следующем примере **выполняется поиск ресурсов driveItem** и агрегируются результаты по их размеру, который является числовым значением. Запрос задает статистическую обработку по 3 диапазонам размеров:
- Размер меньше 100
- Размер от 100 до 1000
- Размер 1000 и выше

Ответ включает 3 **объекта searchBucket** , по одному для каждого агрегирования диапазона размеров:
- Два сегмента диапазонов нижнего размера не включают совпадения поиска.
- Все 9 соответствий поиска имеют размер 1000 или более.

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

Агрегаты поддерживаются только для элементов SharePoint или OneDrive. Они не поддерживаются для **сообщений или** **событий**.

## <a name="next-steps"></a>Дальнейшие действия

- [Использование API Поиска (Майкрософт) для запроса данных](/graph/api/resources/search-api-overview)
