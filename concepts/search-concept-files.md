---
title: Использование API службы поиска Microsoft в Microsoft Graph для поиска файлов
description: Вы можете использовать API службы поиска Microsoft для поиска файлов, хранящихся в SharePoint или OneDrive.
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 0b8db24a8b9ccd63ac3d3be800b209a64eb3aa9d
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866919"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-search-files"></a>Использование API службы поиска Microsoft в Microsoft Graph для поиска файлов

Вы можете использовать API службы поиска Microsoft для поиска файлов, хранящихся в SharePoint или OneDrive. API поиска Microsoft использует модель релевантности, которая использует сигналы из Microsoft Graph о связях и действиях пользователей. Это позволяет вернуть и повысить уровень содержимого, которое пользователи волнует, в интерфейсе поиска файлов, который соответствует вкладке **файлы** , в которой отображаются результаты поиска в SharePoint. 

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

API также может подавать внешние файлы, предоставляемые через ресурс [екстерналфиле](/graph/api/resources/externalfile?view=graph-rest-beta) .

## <a name="search-sharepoint-or-onedrive-files"></a>Поиск файлов SharePoint или OneDrive

KQL можно использовать в терминах поиска запросов для SharePoint и OneDrive. Пример:

- `"query": "contoso filetype:docx OR filetype:doc"`ограничивает область запроса документами Word.
- `"query": "test path:\\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""`ограничивает область запроса определенной папкой на сайте.

Для того чтобы оно было допустимым, ограничение свойств должно указывать допустимое имя управляемого свойства, запрашиваемое в условии.

### <a name="example"></a>Пример

#### <a name="request"></a>Запрос

```HTTP
POST /search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "entityTypes": [
        "microsoft.graph.driveItem"
      ],
      "query": {
        "query_string": {
          "query": "contoso"
        }
      },
      "from": 0,
      "size": 25
    }
  ]
}
```

#### <a name="response"></a>Ответ

<!---TODO nmoreau team Include one example of externalItem response.-->
```json
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
            }
          ]
        }
      ]
    }
  ]
}
```

## <a name="search-external-files-well-known-types"></a>Поиск внешних файлов (известных типов)

По умолчанию в Microsoft Search есть доступ [к файловому ресурсному соединителю](/MicrosoftSearch/file-share-connector) . Его можно использовать для индексации файлов, доступных в общей папке. Вы можете использовать API запросов для запроса всех внешних файлов.

<!-- markdownlint-disable MD024 -->
### <a name="example"></a>Пример

В следующем примере возвращаются все настроенные внешние файлы для клиента, а результаты сортируются по релевантности.

#### <a name="request"></a>Запрос

```HTTP
POST /search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "entityTypes": [
        "microsoft.graph.externalFile"
      ],
      "query": {
        "query_string": {
          "query": "contoso"
        }
      },
      "from": 0,
      "size": 25
    }
  ]
}
```

#### <a name="response"></a>Ответ

```json
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#search",
  "value": [
    {
      "searchTerms": [
        "contoso"
      ],
      "hitsContainers": [
        {
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
                "url": "file://fileshare01/External Presentations/Contoso-Overview.pptx"
              }
            },
            {
              //Another searchHit
            }
          ]
        }
      ]
    }
  ]
}
```

## <a name="search-all-files-including-externalfile-instances"></a>Поиск во всех файлах (в том числе экземплярах Екстерналфиле)

Можно выполнять поиск по всем файлам в клиенте, включая файлы, хранящиеся в [элементов driveitem](/graph/api/resources/driveitem?view=graph-rest-beta) и внешние файлы, указывая два типа сущностей в запросе поиска.

Ответ содержит экземпляры **driveItem** и **екстерналитем** в `_sources` поле каждого объекта [сеарчхит](/graph/api/resources/searchhit?view=graph-rest-beta) .

### <a name="example"></a>Пример

В следующем примере возвращаются все настроенные объекты **екстерналфиле** и **driveItem** в клиенте, которые удовлетворяют условиям поиска. Результаты сортируются по релевантности.

### <a name="request"></a>Запрос

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "entityTypes": [
        "microsoft.graph.driveItem",
        "microsoft.graph.externalFile"
      ],
      "query": {
        "query_string": {
          "query": "contoso"
        }
      },
      "from": 0,
      "size": 25
    }
  ]
}
```

## <a name="known-limitations"></a>Известные ограничения

Вы не можете ограничить запрос определенным ИДЕНТИФИКАТОРом подключения.

## <a name="next-steps"></a>Дальнейшие действия

- [Использование API Поиска (Майкрософт) для запроса данных](/graph/api/resources/search-api-overview?view=graph-rest-beta)

