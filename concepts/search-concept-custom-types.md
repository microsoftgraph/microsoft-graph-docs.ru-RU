---
title: Использование API службы поиска Microsoft в Microsoft Graph для поиска пользовательских типов
description: С помощью API Microsoft Search можно импортировать внешние данные через ресурс [екстерналитем](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) и запускать поисковые запросы для этого внешнего контента.
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: b125b8f923e941ad73d5c578e99a67fdd9ea9eea
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192604"
---
# <a name="use-the-microsoft-search-api-to-search-custom-types-imported-using-microsoft-graph-connectors"></a><span data-ttu-id="64086-103">Использование API службы поиска Microsoft для поиска настраиваемых типов, импортированных с помощью Microsoft Graph Connectors</span><span class="sxs-lookup"><span data-stu-id="64086-103">Use the Microsoft Search API to search custom types imported using Microsoft Graph connectors</span></span>

<span data-ttu-id="64086-104">Используйте API Microsoft Search API для поиска контента, полученных и индексируемых через [соединители Microsoft Graph](https://docs.microsoft.com/microsoftsearch/connectors-overview).</span><span class="sxs-lookup"><span data-stu-id="64086-104">Use the Microsoft Search API to search accross content ingested and indexed by [Microsoft Graph connectors](https://docs.microsoft.com/microsoftsearch/connectors-overview).</span></span> <span data-ttu-id="64086-105">Содержимое импортируется либо через [встроенные соединители](https://docs.microsoft.com/microsoftsearch/connectors-gallery) , предоставляемые корпорацией Майкрософт, либо через пользовательские соединители, реализованные с помощью [API приема Microsoft Graph Connectors](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="64086-105">The content is imported either via [built-in connectors](https://docs.microsoft.com/microsoftsearch/connectors-gallery) provided by Microsoft, or via custom connectors implemented using the [Microsoft Graph connectors ingestion API](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true).</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

<span data-ttu-id="64086-106">После импорта и индексирования контента можно использовать API поиска для запроса контента.</span><span class="sxs-lookup"><span data-stu-id="64086-106">Once the content has been imported and indexed, you can use the search API to query the content.</span></span>

<span data-ttu-id="64086-107">Чтобы выполнить поиск пользовательских типов, укажите следующие свойства в теле запроса метода [запроса](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) :</span><span class="sxs-lookup"><span data-stu-id="64086-107">To search for custom types, specify the following properties in the request body of the [query](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) method:</span></span>

- <span data-ttu-id="64086-108">Свойство **контентсаурцес** для включения идентификатора подключения, назначаемого во время установки соединителя.</span><span class="sxs-lookup"><span data-stu-id="64086-108">The **contentSources** property to include the connection ID that is assigned during the connector setup.</span></span> <span data-ttu-id="64086-109">Можно передать несколько идентификаторов подключения для поиска по нескольким подключениям.</span><span class="sxs-lookup"><span data-stu-id="64086-109">You can pass multiple connection IDs to search across multiple connections.</span></span> <span data-ttu-id="64086-110">Результаты возвращаются в виде одного списка, ранжированного по нескольким подключениям.</span><span class="sxs-lookup"><span data-stu-id="64086-110">Results are returned in a single list, ranked accross the multiple connections.</span></span>

<!--
TODOSEARCHAPI - Bug 1653398 
-->

- <span data-ttu-id="64086-111">Свойство **EntityTypes** AS `externalItem` .</span><span class="sxs-lookup"><span data-stu-id="64086-111">The **entityTypes** property as `externalItem`.</span></span>

- <span data-ttu-id="64086-112">Свойство **Fields** для включения полей во внешний элемент для извлечения.</span><span class="sxs-lookup"><span data-stu-id="64086-112">The **fields** property to include the fields in the external item to retrieve.</span></span>

## <a name="example"></a><span data-ttu-id="64086-113">Пример</span><span class="sxs-lookup"><span data-stu-id="64086-113">Example</span></span>

<span data-ttu-id="64086-114">В этом примере содержимое базы данных [AdventureWorks](https://docs.microsoft.com/sql/samples/adventureworks-install-configure) было активировано с помощью встроенного СОЕДИНИТЕЛЯ Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="64086-114">In this example, the content of the [AdventureWorks](https://docs.microsoft.com/sql/samples/adventureworks-install-configure) database has been ingested using the Azure SQL built-in connector.</span></span>

### <a name="request"></a><span data-ttu-id="64086-115">Запрос</span><span class="sxs-lookup"><span data-stu-id="64086-115">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="64086-116">Отклик</span><span class="sxs-lookup"><span data-stu-id="64086-116">Response</span></span>

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

## <a name="known-limitations"></a><span data-ttu-id="64086-117">Известные ограничения</span><span class="sxs-lookup"><span data-stu-id="64086-117">Known limitations</span></span>

- <span data-ttu-id="64086-118">Для получения извлекаемых полей в схеме поиска необходимо указать свойство **Fields** .</span><span class="sxs-lookup"><span data-stu-id="64086-118">You must specify the **fields** property to get retrievable fields in the search schema.</span></span>

## <a name="next-steps"></a><span data-ttu-id="64086-119">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="64086-119">Next steps</span></span>

- [<span data-ttu-id="64086-120">Использование API Поиска (Майкрософт) для запроса данных</span><span class="sxs-lookup"><span data-stu-id="64086-120">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
