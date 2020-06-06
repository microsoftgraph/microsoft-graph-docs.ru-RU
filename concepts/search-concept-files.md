---
title: Использование API службы поиска Microsoft в Microsoft Graph для поиска файлов
description: Вы можете использовать API службы поиска Microsoft для поиска файлов, хранящихся в SharePoint или OneDrive.
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 52b2d5b54577bfb744bff5f3dacf4ad77da3761a
ms.sourcegitcommit: 093d89c7583bb6880c8395e9498a1f33cdd938b4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44568812"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-search-files"></a>Использование API службы поиска Microsoft в Microsoft Graph для поиска файлов

Вы можете использовать API службы поиска Microsoft для поиска файлов, хранящихся в SharePoint или OneDrive. API поиска Microsoft использует модель релевантности, которая использует сигналы из Microsoft Graph о связях и действиях пользователей. Это позволяет вернуть и повысить уровень содержимого, которое пользователи волнует, в интерфейсе поиска файлов, который соответствует вкладке **файлы** , в которой отображаются результаты поиска в SharePoint.

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

## <a name="search-sharepoint-or-onedrive-files"></a>Поиск файлов SharePoint или OneDrive

KQL можно использовать в терминах поиска запросов для SharePoint и OneDrive. Пример.

- `"query": "contoso filetype:docx OR filetype:doc"`ограничивает область запроса документами Word.
- `"query": "test path:\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""`ограничивает область запроса определенной папкой на сайте.

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
        "driveItem"
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

## <a name="next-steps"></a>Дальнейшие действия

- [Использование API Поиска (Майкрософт) для запроса данных](/graph/api/resources/search-api-overview?view=graph-rest-beta)
