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
# <a name="use-the-microsoft-search-api-to-search-custom-types-imported-using-microsoft-graph-connectors-preview"></a><span data-ttu-id="152b7-103">Использование API службы поиска Microsoft для поиска настраиваемых типов, импортированных с помощью Microsoft Graph Connectors (Предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="152b7-103">Use the Microsoft Search API to search custom types imported using Microsoft Graph connectors (preview)</span></span> 

<span data-ttu-id="152b7-104">Используйте API Microsoft Search API для поиска контента, полученных и индексируемых через [соединители Microsoft Graph](/microsoftsearch/connectors-overview).</span><span class="sxs-lookup"><span data-stu-id="152b7-104">Use the Microsoft Search API to search accross content ingested and indexed by [Microsoft Graph connectors](/microsoftsearch/connectors-overview).</span></span> <span data-ttu-id="152b7-105">Содержимое импортируется либо через [встроенные соединители](/microsoftsearch/connectors-gallery) , предоставляемые корпорацией Майкрософт, либо через пользовательские соединители, реализованные с помощью [API приема Microsoft Graph Connectors](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="152b7-105">The content is imported either via [built-in connectors](/microsoftsearch/connectors-gallery) provided by Microsoft, or via custom connectors implemented using the [Microsoft Graph connectors ingestion API](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true).</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

<span data-ttu-id="152b7-106">После импорта и индексирования контента можно использовать API поиска для запроса контента.</span><span class="sxs-lookup"><span data-stu-id="152b7-106">Once the content has been imported and indexed, you can use the search API to query the content.</span></span>

<span data-ttu-id="152b7-107">Чтобы выполнить поиск пользовательских типов, укажите следующие свойства в теле запроса метода [запроса](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) :</span><span class="sxs-lookup"><span data-stu-id="152b7-107">To search for custom types, specify the following properties in the request body of the [query](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) method:</span></span>

- <span data-ttu-id="152b7-108">Свойство **контентсаурцес** для включения идентификатора подключения, назначаемого во время установки соединителя.</span><span class="sxs-lookup"><span data-stu-id="152b7-108">The **contentSources** property to include the connection ID that is assigned during the connector setup.</span></span> <span data-ttu-id="152b7-109">Можно передать несколько идентификаторов подключения для поиска по нескольким подключениям.</span><span class="sxs-lookup"><span data-stu-id="152b7-109">You can pass multiple connection IDs to search across multiple connections.</span></span> <span data-ttu-id="152b7-110">Результаты возвращаются в виде одного списка, ранжированного по нескольким подключениям.</span><span class="sxs-lookup"><span data-stu-id="152b7-110">Results are returned in a single list, ranked accross the multiple connections.</span></span>

<!--
TODOSEARCHAPI - Bug 1653398 
-->

- <span data-ttu-id="152b7-111">Свойство **EntityTypes** AS `externalItem` .</span><span class="sxs-lookup"><span data-stu-id="152b7-111">The **entityTypes** property as `externalItem`.</span></span>

- <span data-ttu-id="152b7-112">Свойство **Fields** для включения полей во внешний элемент для извлечения.</span><span class="sxs-lookup"><span data-stu-id="152b7-112">The **fields** property to include the fields in the external item to retrieve.</span></span> <span data-ttu-id="152b7-113">Обратите внимание, что если вы не включаете какие бы то ни было **поля** в запрос, ответ будет содержать все поля, помеченные как *извлекаемые* в схеме данных, указанной для заданных подключений в свойстве **контентсаурцес** .</span><span class="sxs-lookup"><span data-stu-id="152b7-113">Note that if you do not include any **fields** in the request, the response will contain all the fields marked as *retrievable* in the data schema specified for the specified connections in the **contentSources** property.</span></span>

<span data-ttu-id="152b7-114">Кроме того, можно агрегировать результаты поиска на основе свойств в [екстерналитем](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) , которые представляют собой числовые или строковые типы, и которые настроены для уточнения в [схеме](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="152b7-114">In addition, you can aggregate search results based on properties in an [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) that are numeric or string type, and that are set to be refinable in the [schema](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true).</span></span> <span data-ttu-id="152b7-115">Более подробную информацию можно узнать [в статье уточнение результатов поиска с помощью агрегатов](search-concept-aggregation.md).</span><span class="sxs-lookup"><span data-stu-id="152b7-115">For more information, see [Refine search results using aggregations](search-concept-aggregation.md).</span></span>

## <a name="example"></a><span data-ttu-id="152b7-116">Пример</span><span class="sxs-lookup"><span data-stu-id="152b7-116">Example</span></span>

<span data-ttu-id="152b7-117">В этом примере содержимое базы данных [AdventureWorks](/sql/samples/adventureworks-install-configure) было активировано с помощью встроенного СОЕДИНИТЕЛЯ Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="152b7-117">In this example, the content of the [AdventureWorks](/sql/samples/adventureworks-install-configure) database has been ingested using the Azure SQL built-in connector.</span></span>

### <a name="request"></a><span data-ttu-id="152b7-118">Запрос</span><span class="sxs-lookup"><span data-stu-id="152b7-118">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="152b7-119">Ответ</span><span class="sxs-lookup"><span data-stu-id="152b7-119">Response</span></span>

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

## <a name="next-steps"></a><span data-ttu-id="152b7-120">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="152b7-120">Next steps</span></span>

- [<span data-ttu-id="152b7-121">Использование API Поиска (Майкрософт) для запроса данных</span><span class="sxs-lookup"><span data-stu-id="152b7-121">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)