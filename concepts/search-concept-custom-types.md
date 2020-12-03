---
title: Использование API службы поиска Microsoft в Microsoft Graph для поиска пользовательских типов
description: С помощью API Microsoft Search можно импортировать внешние данные через ресурс [екстерналитем](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) и запускать поисковые запросы для этого внешнего контента.
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: ba08eeb2aeaf4aa13e6b5bc686143e9b4293c0d8
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49523765"
---
# <a name="use-the-microsoft-search-api-to-search-custom-types-imported-using-microsoft-graph-connectors-preview"></a>Использование API службы поиска Microsoft для поиска настраиваемых типов, импортированных с помощью Microsoft Graph Connectors (Предварительная версия) 

Используйте API Microsoft Search API для поиска контента, полученных и индексируемых через [соединители Microsoft Graph](/microsoftsearch/connectors-overview). Содержимое импортируется либо через [встроенные соединители](/microsoftsearch/connectors-gallery) , предоставляемые корпорацией Майкрософт, либо через пользовательские соединители, реализованные с помощью [API приема Microsoft Graph Connectors](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true).

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

После импорта и индексирования контента можно использовать API поиска для запроса контента.

Чтобы выполнить поиск пользовательских типов, укажите следующие свойства в теле запроса метода [запроса](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) :

- Свойство **контентсаурцес** для включения идентификатора подключения, назначаемого во время установки соединителя. Можно передать несколько идентификаторов подключения для поиска по нескольким подключениям. Результаты возвращаются в виде одного списка, ранжированного по нескольким подключениям.

<!--
TODOSEARCHAPI - Bug 1653398 
-->

- Свойство **EntityTypes** AS `externalItem` .

- Свойство **Fields** для включения полей во внешний элемент для извлечения. Обратите внимание, что если вы не включаете какие бы то ни было **поля** в запрос, ответ будет содержать все поля, помеченные как *извлекаемые* в схеме данных, указанной для заданных подключений в свойстве **контентсаурцес** .

Кроме того, можно агрегировать результаты поиска на основе свойств в [екстерналитем](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) , которые представляют собой числовые или строковые типы, и которые настроены для уточнения в [схеме](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true). Более подробную информацию можно узнать [в статье уточнение результатов поиска с помощью агрегатов](search-concept-aggregation.md).

## <a name="example"></a>Пример

В этом примере содержимое базы данных [AdventureWorks](/sql/samples/adventureworks-install-configure) было активировано с помощью встроенного СОЕДИНИТЕЛЯ Azure SQL.

### <a name="request"></a>Запрос

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "externalItem"
      ],
      "contentSources": [
          "/external/connections/azuresqlconnector",
          "/external/connections/azuresqlconnector2"
      ],
      "query": {
        "queryString": "yang"
      },
      "from": 0,
      "size": 25,
      "fields": [
        "BusinessEntityID",
        "firstName",
        "lastName"
      ]
    }
  ]
}
```

### <a name="response"></a>Ответ

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.searchResponse)",
  "value": [
    {
      "searchTerms": ["ya"],
      "hitsContainers": [
        {
          "total": 2,
          "moreResultsAvailable": false,
          "hits": [
            {
              "hitId": "AAMkADc0NDNlNTE0",
              "rank": 1,
              "summary": "<ddd/>",
              "contentSource": "/external/connections/azuresqlconnector",
              "resource": {
                "@odata.type": "#microsoft.graph.externalItem",
                "properties": {
                  "businessEntityID": 20704,
                  "firstName": "Amy",
                  "lastName": "Yang"
                }
              }
            },
           {
              "hitId": "AQMkADg3M2I3YWMyLTEwZ",
              "rank": 2,
              "summary": "<ddd/>",
              "contentSource": "/external/connections/azuresqlconnector2",
              "resource": {
                "@odata.type": "#microsoft.graph.externalItem",
                "properties": {
                  "businessEntityID": 20704,
                  "shortdescription": "Contoso maintenance guidelines",
                  "firstName": "Amy",
                  "lastName": "Yang"
                }
              }
            },
          ]
        }
      ]
    }
  ]
}
```

## <a name="next-steps"></a>Дальнейшие действия

- [Использование API Поиска (Майкрософт) для запроса данных](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)