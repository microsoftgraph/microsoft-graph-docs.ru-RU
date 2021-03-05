---
ms.author: yiwenwang
title: Используйте API поиска Майкрософт в Microsoft Graph для поиска пользовательских типов
description: API поиска Майкрософт можно использовать для импорта внешних данных с помощью [ресурса externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) и запуска поисковых запросов по этому внешнему контенту.
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: c4e0b158356d3f26d8a0f36a7d7e86faeba96649
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471840"
---
# <a name="use-the-microsoft-search-api-to-search-custom-types-imported-using-microsoft-graph-connectors-preview"></a><span data-ttu-id="933c7-103">Используйте API поиска Майкрософт для поиска пользовательских типов, импортируемых с помощью соединителов Microsoft Graph (предварительный просмотр)</span><span class="sxs-lookup"><span data-stu-id="933c7-103">Use the Microsoft Search API to search custom types imported using Microsoft Graph connectors (preview)</span></span> 

<span data-ttu-id="933c7-104">Используйте API поиска Майкрософт для поиска по контенту, который будет проиндексироваться [соединиттелями Microsoft Graph.](/microsoftsearch/connectors-overview)</span><span class="sxs-lookup"><span data-stu-id="933c7-104">Use the Microsoft Search API to search accross content ingested and indexed by [Microsoft Graph connectors](/microsoftsearch/connectors-overview).</span></span> <span data-ttu-id="933c7-105">Содержимое импортируется либо [](/microsoftsearch/connectors-gallery) через встроенные соединители, предоставляемые Корпорацией Майкрософт, либо через настраиваемые соединители, реализованные с помощью [API ingestion](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true)соединителов Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="933c7-105">The content is imported either via [built-in connectors](/microsoftsearch/connectors-gallery) provided by Microsoft, or via custom connectors implemented using the [Microsoft Graph connectors ingestion API](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true).</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

<span data-ttu-id="933c7-106">После импорта и индексации контента можно использовать API поиска для запроса контента.</span><span class="sxs-lookup"><span data-stu-id="933c7-106">Once the content has been imported and indexed, you can use the search API to query the content.</span></span>

<span data-ttu-id="933c7-107">Чтобы найти настраиваемые типы, укажите следующие свойства в теле запроса метода [запроса:](/graph/api/search-query?view=graph-rest-beta&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="933c7-107">To search for custom types, specify the following properties in the request body of the [query](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) method:</span></span>

- <span data-ttu-id="933c7-108">Свойство **contentSources,** чтобы включить ID подключения, задаваемое во время установки соединиттеля.</span><span class="sxs-lookup"><span data-stu-id="933c7-108">The **contentSources** property to include the connection ID that is assigned during the connector setup.</span></span> <span data-ttu-id="933c7-109">Вы можете передать несколько ID-подключений для поиска по нескольким подключениям.</span><span class="sxs-lookup"><span data-stu-id="933c7-109">You can pass multiple connection IDs to search across multiple connections.</span></span> <span data-ttu-id="933c7-110">Результаты возвращаются в одном списке, ранжировали по нескольким подключениям.</span><span class="sxs-lookup"><span data-stu-id="933c7-110">Results are returned in a single list, ranked accross the multiple connections.</span></span>

<!--
TODOSEARCHAPI - Bug 1653398 
-->

- <span data-ttu-id="933c7-111">Свойство **entityTypes** как `externalItem` .</span><span class="sxs-lookup"><span data-stu-id="933c7-111">The **entityTypes** property as `externalItem`.</span></span>

- <span data-ttu-id="933c7-112">Свойство **полей,** чтобы включить поля во внешний элемент для получения.</span><span class="sxs-lookup"><span data-stu-id="933c7-112">The **fields** property to include the fields in the external item to retrieve.</span></span> <span data-ttu-id="933c7-113">Обратите внимание, что если  в запрос не включены какие-либо поля, ответ будет содержать все поля, отмеченные в схеме данных, указанной для указанных подключений в свойстве **contentSources.** </span><span class="sxs-lookup"><span data-stu-id="933c7-113">Note that if you do not include any **fields** in the request, the response will contain all the fields marked as *retrievable* in the data schema specified for the specified connections in the **contentSources** property.</span></span>

<span data-ttu-id="933c7-114">Кроме того, можно агрегировать результаты поиска на основе свойств [в externalItem,](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) которые числимы или типа строки, и которые должны быть уточнены в [схеме](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="933c7-114">In addition, you can aggregate search results based on properties in an [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) that are numeric or string type, and that are set to be refinable in the [schema](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true).</span></span> <span data-ttu-id="933c7-115">Дополнительные сведения см. в дополнительных сведениях об уточнении результатов поиска с помощью [агрегаций.](search-concept-aggregation.md)</span><span class="sxs-lookup"><span data-stu-id="933c7-115">For more information, see [Refine search results using aggregations](search-concept-aggregation.md).</span></span>

## <a name="example-1-retrieve-items-using-azure-sql-built-in-connector"></a><span data-ttu-id="933c7-116">Пример 1. Извлечение элементов с помощью встроенного соединиттеля Azure SQL Azure</span><span class="sxs-lookup"><span data-stu-id="933c7-116">Example 1: Retrieve items using Azure SQL built-in connector</span></span>

<span data-ttu-id="933c7-117">В этом примере содержимое базы данных [AdventureWorks](/sql/samples/adventureworks-install-configure) было въехано с помощью встроенного соединиттеля Azure SQL Azure.</span><span class="sxs-lookup"><span data-stu-id="933c7-117">In this example, the content of the [AdventureWorks](/sql/samples/adventureworks-install-configure) database has been ingested using the Azure SQL built-in connector.</span></span>

### <a name="request"></a><span data-ttu-id="933c7-118">Запрос</span><span class="sxs-lookup"><span data-stu-id="933c7-118">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="933c7-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="933c7-119">Response</span></span>

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
                  "shortDescription": "Contoso maintenance guidelines",
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

## <a name="example-2-retrieve-items-using-semantic-labels"></a><span data-ttu-id="933c7-120">Пример 2. Извлечение элементов с помощью семантических меток</span><span class="sxs-lookup"><span data-stu-id="933c7-120">Example 2: Retrieve items using semantic labels</span></span>

### <a name="request"></a><span data-ttu-id="933c7-121">Запрос</span><span class="sxs-lookup"><span data-stu-id="933c7-121">Request</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json

{
    "requests": [
      {
        "entityTypes": [
          "microsoft.graph.externalItem"
        ],
        "contentSources": [
          "/external/connections/FileAsUdt"
        ],
        "query": {
          "query_string": {
            "query": "test"
          }
        },
        "stored_fields": [
          "label_Title",
          "label_URL",
          "label_LastModifiedBy",
          "label_LastModifiedDateTime"
        ],
        "from": 0,
        "size": 25
      }
    ]
}
```

### <a name="response"></a><span data-ttu-id="933c7-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="933c7-122">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.searchResponse)",
"value": [
      {
        "searchTerms": [
          "test"
        ],
        "hitsContainers": [
          {
            "hits": [
              {
                "_id": "AQMkAGRjZWJjZTFkLTkzYWItNDhlOC1iODA2LTgwMTNjNjEzYzI2YwBGAAADOx0/YV2JckefuDmJtUO7mwcAHNjGq33S50uXSFeU/U9mogAAAgEWAAAAHNjGq33S50uXSFeU/U9mogAAAgleAAAA",
                "_contentSource": "FileAsUdt",
                "_score": 1,
                "_summary": "<c0>Test</c0> component to move data files and messages between the gateway and internal <ddd/>",
                "_source": {
                  "@odata.type": "#microsoft.graph.externalItem",
                  "properties": {
                    "label_Title": "SONIC Operations support and test Guide for the month of March",
                    "label_URL": "D:\\\\ConnectorsEcho\\\\New\\\\MSW06SecondSet\\\\teams\\\\Enterprise_Platforms\\\\CCO\\\\Projects\\\\BTSi Modernization\\\\SONIC Retirement\\\\SONIC_Operations_Support_Guide.docx",
                    "label_LastModifiedBy": [
                      "Bob",
                      "Scott"
                    ],
                    "label_LastModifiedDateTime": "2020-01-30T12:44:19Z"
                  }
                }
              },
              {
                "_id": "AQMkAGRjZWJjZTFkLTkzYWItNDhlOC1iODA2LTgwMTNjNjEzYzI2YwBGAAADOx0/YV2JckefuDmJtUO7mwcAHNjGq33S50uXSFeU/U9mogAAAgEWAAAAHNjGq33S50uXSFeU/U9mogAAAgldAAAA",
                "_contentSource": "FileAsUdt",
                "_score": 2,
                "_summary": "File Transfer Workbench A <c0>test</c0> File transfer Management Solution File Transfer the number <ddd/>",
                "_source": {
                  "@odata.type": "#microsoft.graph.externalItem",
                  "properties": {
                    "label_Title": "Test File Transfer Workbench for the month of January",
                    "label_URL": "D:\\\\ConnectorsEcho\\\\New\\\\MSW06SecondSet\\\\teams\\\\IssueLog\\\\FCAGA Organisation\\\\NSN CO CCA Infra YBCFTPAR entry\\\\File Transfer Workbench.ppt",
                    "label_LastModifiedBy": [
                      "Alice",
                      "Scott"
                    ],
                    "label_LastModifiedDateTime": "2020-01-31T11:44:19Z"
                  }
                }
              },
              {
                "_id": "AQMkAGRjZWJjZTFkLTkzYWItNDhlOC1iODA2LTgwMTNjNjEzYzI2YwBGAAADOx0/YV2JckefuDmJtUO7mwcAHNjGq33S50uXSFeU/U9mogAAAgEWAAAAHNjGq33S50uXSFeU/U9mogAAAglgAAAA",
                "_contentSource": "FileAsUdt",
                "_score": 3,
                "_summary": "document and the associated <c0>test</c0> software are the sole property of Express Logic.<ddd/>",
                "_source": {
                  "@odata.type": "#microsoft.graph.externalItem",
                  "properties": {
                    "label_Title": "System User Guide Express Logic 858.613.6640",
                    "label_URL": "D:\\\\ConnectorsEcho\\\\New\\\\MSW06FirstSet\\\\teams\\\\AzureIoTMarketing\\\\Shared Documents\\\\Whitepapers\\\\RTOS Whitepapers\\\\User Guides\\\\Azure_RTOS_FileX_User_Guide.pdf",
                    "label_LastModifiedBy": [
                      "Alice",
                      "Bob"
                    ],
                    "label_LastModifiedDateTime": "2020-05-25T10:20:19Z"
                  }
                }
              }
            ],
            "total": 3,
            "moreResultsAvailable": false
          }
        ]
      }
    ]
}
```

<span data-ttu-id="933c7-123">Дополнительные сведения см. в [материале Назначение меток свойств.](/microsoftsearch/configure-connector#step-5-assign-property-labels)</span><span class="sxs-lookup"><span data-stu-id="933c7-123">For more details, see [Assign property labels](/microsoftsearch/configure-connector#step-5-assign-property-labels).</span></span>

## <a name="next-steps"></a><span data-ttu-id="933c7-124">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="933c7-124">Next steps</span></span>

- [<span data-ttu-id="933c7-125">Использование API Поиска (Майкрософт) для запроса данных</span><span class="sxs-lookup"><span data-stu-id="933c7-125">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
