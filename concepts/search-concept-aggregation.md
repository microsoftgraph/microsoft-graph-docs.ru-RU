---
title: Использование API службы поиска Microsoft в Microsoft Graph для уточнения запросов с помощью агрегатов
description: Вы можете использовать API службы поиска Microsoft для получения аггреатионс
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: b414c0beb26280ef90d0a6bd5c807ee9904a5a7e
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193807"
---
# <a name="refine-search-results-using-aggregations"></a>Уточнение результатов поиска с помощью агрегатов

Уточните результаты поиска и отобразите их распределение в индексе. 

## <a name="example-1-request-aggregations-by-string-fields"></a>Пример 1: запрос агрегатов по строковым полям

В следующем примере выполняется поиск ресурсов **ListItem** и статистические результаты по их типам файлов и классу контента, которые являются строковыми значениями.

Ответ включает два объекта [сеарчбуккет](/graph/api/resources/searchbucket?view=graph-rest-beta&preserve-view=true) для двух агрегатов:
- Свойство **Key** указывает фактическое значение (by `FileType` или `contentclass` ) для соответствующих объектов **ListItem** , которые объединены в одном сегменте с этим значением.
- Свойство **Count** указывает количество таких объектов, собранных в том же сегменте.
- Сегменты результатов, агрегированные по типу файла, сортируются по количеству в порядке убывания. В этом примере для трех типов файлов используется 3 сегмента: `docx` , `xlsx` и `pptx` .
- Сегменты результатов, агрегированные по классу контента, сортируются по строковому значению класса контента в порядке убывания. В этом примере существует только один сегмент со всеми связанными объектами, совместно использующих один и тот же класс контента `STS_ListItem_DocumentLibrary` .

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

## <a name="example-2-apply-an-aggregation-filter-based-on-a-previous-request"></a>Пример 2: применение фильтра агрегирования на основе предыдущего запроса

В этом примере применяется фильтр агрегирования, основанный на **аггрегатионфилтертокен** , возвращенном для `docx` `FileType` поля в примере 1.

Строковое значение, назначенное свойству **аггрегатионфилтерс** , соответствует формату **"{Field}: \\ " {аггрегатионфилтертокен} \\ ""**.

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

## <a name="example-3-request-aggregation-by-a-numeric-field"></a>Пример 3: запрос агрегирования с помощью числового поля

В следующем примере выполняется поиск ресурсов **driveItem** и статистические результаты по их размеру — числовому значению. В запросе задается объединение по 3 диапазонам размера:
- Размер менее 100
- Размер между 100 и 1000
- Размер 1000 и выше

Ответ включает 3 объекта **сеарчбуккет** , по одному для каждого объединения диапазонов размеров:
- 2 сегмента из диапазонов меньшего размера не содержат совпадений поиска.
- Все 9 совпадений поиска имеют размеры 1000 или выше.

### <a name="request"></a>Запрос

```HTTP
POST /search/query
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

Агрегаты поддерживаются только для элементов SharePoint или OneDrive. Они не поддерживаются для **сообщений**, **событий**и **екстерналитем**.

## <a name="next-steps"></a>Дальнейшие действия

- [Использование API Поиска (Майкрософт) для запроса данных](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
