---
title: Использование API службы поиска Microsoft в Microsoft Graph для поиска пользовательских типов
description: С помощью API Microsoft Search можно импортировать внешние данные через ресурс [екстерналитем](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) и запускать поисковые запросы для этого внешнего контента.
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: ef245e88e635e888c3a5e2eeafb61497e804072f
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288184"
---
# <a name="use-the-microsoft-search-api-to-search-custom-types-imported-using-microsoft-graph-connectors"></a>Использование API службы поиска Microsoft для поиска настраиваемых типов, импортированных с помощью Microsoft Graph Connectors

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

- Свойство **Fields** для включения полей во внешний элемент для извлечения.

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

### <a name="response"></a>Отклик

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

## <a name="known-limitations"></a>Известные ограничения

- Для получения извлекаемых полей в схеме поиска необходимо указать свойство **Fields** .

## <a name="next-steps"></a>Дальнейшие действия

- [Использование API Поиска (Майкрософт) для запроса данных](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)