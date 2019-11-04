---
title: Поиск файлов (в том числе Екстерналфиле)
description: API запросов позволяет выполнять поиск по файлам (DriveItem или внешним файлам).
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: e34816e56872830cdb3b8ac524293d21588a5d9f
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939553"
---
# <a name="search-files-including-externalfile"></a>Поиск файлов (в том числе Екстерналфиле)

API службы поиска Microsoft позволяет искать файлы, хранящиеся в SharePoint или OneDrive. Он использует модель релевантности, которая использует сигналы из Microsoft Graph о связи и действиях пользователей. Это позволяет вернуть и повысить контент, который пользователи волнует, в процессе поиска файлов, который соответствует вкладке **файлы** , в которой отображаются результаты поиска в SharePoint. 

Кроме того, API может подавать внешние файлы, предоставляемые через ресурс [екстерналфиле](/graph/api/resources/externalfile?view=graph-rest-beta) .


## <a name="search-sharepoint-or-onedrive-files"></a>Поиск файлов SharePoint или OneDrive

KQL можно использовать в терминах поиска запросов для SharePoint и OneDrive. Пример:

- "запрос": "области" Contoso тип_файла: docx и filetype: doc "— запросы к документам Word
- "запрос": "путь к\\тестуhttps://contoso.sharepoint.com/sites/Team :" site/Documents/Project\\"" область запроса в определенной папке на сайте.

Чтобы быть допустимым, ограничение свойств должно указывать допустимое имя управляемого свойства, поддерживающего запросы, в условии.

### <a name="example"></a>Пример

#### <a name="request"></a>Запрос

```HTTP
POST /search/query
Content-Type: application/json
```

```Json
{
  "requests": [
    {
       "entityTypes": ["microsoft.graph.driveItem"],
       "query": {
        "query_string": {
          "query": "contoso"
        }
      },
      "from": 0,
      "size": 25,
    }
  ]
}
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

<!---TODO nmoreau team Include one example of externalItem response.-->
```Json
{

  "@odata.context": "https://graph.microsoft.com/beta/$metadata#search",
  "value": [
      {
          "searchTerms": [
              "test"
          ],
          "hitsContainers": [
              {
                  "total": 350,
                  "moreResultsAvailable": true,
                  "hits": [
                      {
                          "_id": "FlULeN/ui/1GjLx1rUfio5UAAEl",
                          "_score": 1,
                          "_sortField": "Relevance",
                          "_summary": "<c0>Contoso</c0> Detailed Design <ddd/>",
                          "_source": {
                              "@odata.type": "#microsoft.graph.driveItem",
                              "createdDateTime": "2019-06-10T06:37:43Z",
                              "lastModifiedDateTime": "2019-06-10T06:37:43Z",
                              "name": "web_part_test_long Notebook",
                              "webUrl": "https://contoso.sharepoint.com/sites/contoso-team/contoso-designs.docx",
                              "lastModifiedBy": {
                                  "user": {
                                      "displayName": "Richard Mayer"
                                  }
                              },
                              "fileSystemInfo": {
                                  "createdDateTime": "2019-06-10T06:37:43Z",
                                  "lastModifiedDateTime": "2019-06-10T06:37:43Z"
                              }
                          }
                      },
                      {
                      }
                  ]
              }
          ]
      }
  ]
}
```

## <a name="search-external-files-well-known-types"></a>Поиск внешних файлов (известных типов)

[Соединитель файлов общего доступа](/MicrosoftSearch/file-share-connector) — это соединитель "из поля", доступный в Microsoft Search. Он позволяет индексировать файлы, доступные в общей папке. Вы можете использовать API запросов для запроса всех внешних файлов.

### <a name="example"></a>Пример
Следующий пример возвращает все настроенные соединители Екстерналфиле для клиента и сортирует результаты по релевантности.

#### <a name="request"></a>Запрос

```HTTP
POST /search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
       "entityTypes": ["microsoft.graph.externalFile"],
       "query": {
        "query_string": {
          "query": "contoso"
        }
      },
      "from": 0,
      "size": 25,
    }
  ]
}
```

#### <a name="response"></a>Отклик

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#search",
    "value": [{
        "searchTerms": [
            "contoso"
        ],
        "hitsContainers": [{
            "total": 4,
            "moreResultsAvailable": true,
            // Hits represent the search results
            "hits": [
                     {
                     "_id": "FsHvoeTuRRVLnuEZLEVBfSQAAWTp",
                     "_score": 1,
                     "_sortField": "Relevance",
                     "_source": {
                            "@odata.type": "#microsoft.graph.externalFile",
                            "id": "FsHvoeTuRRVLnuEZLEVBfSQAAWTp",
                            "extension": "pptx",
                            "name": "Contoso-Overview.pptx",
                            "lastModifiedTime": "2018-05-09T04:01:14Z",
                            "modifiedBy": "Baala Vedantam",
                            "title": "Contoso Overview 2018",
                            "url": "file://fileshare01/External Presentations/Contoso-Overview.pptx",
                            }
                     }
                     ,
                     {
                            ///Another searchHit
                     }
            ]
        }]
    }]
}
```

## <a name="search-all-files-including-externalfile-instances"></a>Поиск во всех файлах (в том числе экземплярах Екстерналфиле)

Можно выполнять поиск во всех файлах клиента, включая [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) и все внешние файлы, указывая в запросе поиска два типа сущности.

Ответ предоставляет сочетание экземпляров **driveItem** и екстерналитем в `_sources` поле каждого объекта [сеарчхит](/graph/api/resources/searchhit?view=graph-rest-beta) .

### <a name="example"></a>Пример

В следующем примере возвращаются все настроенные соединители **екстерналфиле** и объекты **driveItem** клиента, которые удовлетворяют условиям поиска. Результаты сортируются по релевантности.

### <a name="request"></a>Запрос

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
       "entityTypes": ["microsoft.graph.driveItem","microsoft.graph.externalFile"],
       "query": {
        "query_string": {
          "query": "contoso"
        }
      },
      "from": 0,
      "size": 25,
    }
  ]
}
```

## <a name="known-limitations"></a>Известные ограничения

Невозможно выполнить запрос к определенному Коннектионид.

## <a name="next-steps"></a>Дальнейшие действия

Дополнительные сведения:

- [Использование API поиска](/graph/api/resources/search-api-overview?view=graph-rest-beta)