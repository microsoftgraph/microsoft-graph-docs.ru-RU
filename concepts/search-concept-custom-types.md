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
# <a name="search-custom-types-externalitem"></a><span data-ttu-id="15f1a-103">Настраиваемые типы поиска (Екстерналитем)</span><span class="sxs-lookup"><span data-stu-id="15f1a-103">Search custom types (externalItem)</span></span>

<span data-ttu-id="15f1a-104">API Microsoft Search позволяет импортировать внешние данные через ресурс [екстерналитем](/graph/api/resources/externalitem?view=graph-rest-beta) и запускать поисковые запросы для этого внешнего контента.</span><span class="sxs-lookup"><span data-stu-id="15f1a-104">The Microsoft Search API lets you import external data via the [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) resource, and run search queries on this external content.</span></span>

<span data-ttu-id="15f1a-105">Чтобы выполнить поиск пользовательских типов, укажите следующие данные в тексте запроса метода [запроса](/graph/api/search-query?view=graph-rest-beta) :</span><span class="sxs-lookup"><span data-stu-id="15f1a-105">To search for custom types, specify the following in the [query](/graph/api/search-query?view=graph-rest-beta) method request body:</span></span>

- <span data-ttu-id="15f1a-106">Свойство **контентсаурцес** для включения идентификатора подключения, назначаемого во время установки соединителя.</span><span class="sxs-lookup"><span data-stu-id="15f1a-106">The **contentSources** property to include the connection ID which is assigned during the connector setup</span></span>

- <span data-ttu-id="15f1a-107">Свойство **EntityType** в качестве`externalItem`</span><span class="sxs-lookup"><span data-stu-id="15f1a-107">The **entityType** property as `externalItem`</span></span>

- <span data-ttu-id="15f1a-108">Свойство **stored_fields** для включения полей во внешний элемент, который требуется получить</span><span class="sxs-lookup"><span data-stu-id="15f1a-108">The **stored_fields** property to include the fields in the external item you want to retrieve</span></span>

## <a name="example"></a><span data-ttu-id="15f1a-109">Пример</span><span class="sxs-lookup"><span data-stu-id="15f1a-109">Example</span></span>

### <a name="request"></a><span data-ttu-id="15f1a-110">Запрос</span><span class="sxs-lookup"><span data-stu-id="15f1a-110">Request</span></span>

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
### <a name="response"></a><span data-ttu-id="15f1a-111">Отклик</span><span class="sxs-lookup"><span data-stu-id="15f1a-111">Response</span></span>

<span data-ttu-id="15f1a-112">Отклик</span><span class="sxs-lookup"><span data-stu-id="15f1a-112">Response</span></span>

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


## <a name="known-limitations"></a><span data-ttu-id="15f1a-113">Известные ограничения</span><span class="sxs-lookup"><span data-stu-id="15f1a-113">Known limitations</span></span>

- <span data-ttu-id="15f1a-114">Пользовательские типы не поддерживают поиск в нескольких источниках (указывается в **контентсаурцес**).</span><span class="sxs-lookup"><span data-stu-id="15f1a-114">Custom types don’t support searching across multiple sources (specified in **contentSources**).</span></span> <span data-ttu-id="15f1a-115">Одновременно можно выполнять поиск только по одному подключению.</span><span class="sxs-lookup"><span data-stu-id="15f1a-115">You can search only one connection at a time.</span></span>

- <span data-ttu-id="15f1a-116">Необходимо указать свойство **stored_fields** , иначе результаты поиска не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="15f1a-116">You must specify the **stored_fields** property, otherwise search results are not returned.</span></span>

## <a name="next-steps"></a><span data-ttu-id="15f1a-117">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="15f1a-117">Next steps</span></span>

<span data-ttu-id="15f1a-118">Дополнительные сведения:</span><span class="sxs-lookup"><span data-stu-id="15f1a-118">Find out more about:</span></span>

- [<span data-ttu-id="15f1a-119">Использование API поиска</span><span class="sxs-lookup"><span data-stu-id="15f1a-119">Use the search API</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)