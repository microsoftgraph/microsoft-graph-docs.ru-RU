---
title: Настраиваемые типы поиска
description: API запросов позволяет выполнять поиск по пользовательским типам, которые применялись с помощью API индексирования.
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: d4381529d66eaae19d9866eeb594201cec115735
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939567"
---
# <a name="search-custom-types-externalitem"></a>Настраиваемые типы поиска (Екстерналитем)

API Microsoft Search позволяет импортировать внешние данные через ресурс [екстерналитем](/graph/api/resources/externalitem?view=graph-rest-beta) и запускать поисковые запросы для этого внешнего контента.

Чтобы выполнить поиск пользовательских типов, укажите следующие данные в тексте запроса метода [запроса](/graph/api/search-query?view=graph-rest-beta) :

- Свойство **контентсаурцес** для включения идентификатора подключения, назначаемого во время установки соединителя.

- Свойство **EntityType** в качестве`externalItem`

- Свойство **stored_fields** для включения полей во внешний элемент, который требуется получить

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
       "entityTypes": ["microsoft.graph.externalItem"],
       "contentSources": ["/external/connections/servicenow-connector-contoso"],
       "query": {
        "query_string": {
          "query": "contoso tickets"
        }
      },
      "from": 0,
      "size": 25,
    "stored_fields": [
        "title",
        "priority",
        "description"
       ]
    }
  ]
}
```
### <a name="response"></a>Отклик

Отклик

```Json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.searchResponse)",
    "value": [
        {
            "hitsContainers": [
                {
                    "total": 2,
                    "moreResultsAvailable": false,
                    "hits": [
                        {
                            "_id": "AAMkADc0NDNlNTE0",
                            "_score": 1,
                            "_sortField": "Relevance",
                            "_source": {
                                "@odata.type": "#microsoft.graph.externalItem",
                                "properties": {
                                    "number": "KB0010025",
                                    "shortdescription": "Contoso maintenance guidelines",
                                    "syscreatedon": "2019-10-14T22:45:02Z",
                                    "accessurl": "https://contoso.service-now.com/kb_view.do?sys_kb_id=6b5465781ba000104793877ddc4bcb81",
                                    "previewContent": "Contoso maintenance guidelines"
                                }
                            }
                        },
                        {
                            "_id": "MG+1glPAAAAAAl3AAA=",
                            "_score": 2,
                            "_sortField": "Relevance",
                            "_source": {
                                "@odata.type": "#microsoft.graph.externalItem",
                                "properties": {
                                    "number": "KB0054396",
                                    "shortdescription": "Contoso : Setting Office for the first time.",
                                    "syscreatedon": "2019-08-09T01:53:26Z",
                                    "accessurl": "https://contoso.service-now.com/kb_view.do?sys_kb_id=004d8d931b0733004793877ddc4bcb29",
                                    "previewContent": "Description:  Setting Office for the first time.  Resolution:    To setup any Office app for the first time, tap any Office app like Word to launch it.    Tap Sign in if you already have a Microsoft Account or an Office 365 work or school account."
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


## <a name="known-limitations"></a>Известные ограничения

- Пользовательские типы не поддерживают поиск в нескольких источниках (указывается в **контентсаурцес**). Одновременно можно выполнять поиск только по одному подключению.

- Необходимо указать свойство **stored_fields** , иначе результаты поиска не возвращаются.

## <a name="next-steps"></a>Дальнейшие действия

Дополнительные сведения:

- [Использование API поиска](/graph/api/resources/search-api-overview?view=graph-rest-beta)