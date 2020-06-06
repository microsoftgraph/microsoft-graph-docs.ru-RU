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
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-search-files"></a><span data-ttu-id="3b615-103">Использование API службы поиска Microsoft в Microsoft Graph для поиска файлов</span><span class="sxs-lookup"><span data-stu-id="3b615-103">Use the Microsoft Search API in Microsoft Graph to search files</span></span>

<span data-ttu-id="3b615-104">Вы можете использовать API службы поиска Microsoft для поиска файлов, хранящихся в SharePoint или OneDrive.</span><span class="sxs-lookup"><span data-stu-id="3b615-104">You can use the Microsoft Search API to search files stored in SharePoint or OneDrive.</span></span> <span data-ttu-id="3b615-105">API поиска Microsoft использует модель релевантности, которая использует сигналы из Microsoft Graph о связях и действиях пользователей.</span><span class="sxs-lookup"><span data-stu-id="3b615-105">The Microsoft Search API uses a relevance model that makes use of signals from Microsoft Graph about users' relationships and activities.</span></span> <span data-ttu-id="3b615-106">Это позволяет вернуть и повысить уровень содержимого, которое пользователи волнует, в интерфейсе поиска файлов, который соответствует вкладке **файлы** , в которой отображаются результаты поиска в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3b615-106">This enables you to return and promote the content that users care about, in a file search experience that is consistent with the **Files** tab that lists search results in SharePoint.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

## <a name="search-sharepoint-or-onedrive-files"></a><span data-ttu-id="3b615-107">Поиск файлов SharePoint или OneDrive</span><span class="sxs-lookup"><span data-stu-id="3b615-107">Search SharePoint or OneDrive files</span></span>

<span data-ttu-id="3b615-108">KQL можно использовать в терминах поиска запросов для SharePoint и OneDrive.</span><span class="sxs-lookup"><span data-stu-id="3b615-108">You can use KQL in search terms of queries for SharePoint and OneDrive.</span></span> <span data-ttu-id="3b615-109">Пример.</span><span class="sxs-lookup"><span data-stu-id="3b615-109">For example:</span></span>

- <span data-ttu-id="3b615-110">`"query": "contoso filetype:docx OR filetype:doc"`ограничивает область запроса документами Word.</span><span class="sxs-lookup"><span data-stu-id="3b615-110">`"query": "contoso filetype:docx OR filetype:doc"` scopes the query to Word documents.</span></span>
- <span data-ttu-id="3b615-111">`"query": "test path:\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""`ограничивает область запроса определенной папкой на сайте.</span><span class="sxs-lookup"><span data-stu-id="3b615-111">`"query": "test path:\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""` scopes the query to a particular folder within a site.</span></span>

<span data-ttu-id="3b615-112">Для того чтобы оно было допустимым, ограничение свойств должно указывать допустимое имя управляемого свойства, запрашиваемое в условии.</span><span class="sxs-lookup"><span data-stu-id="3b615-112">In order to be valid, properties restriction should specify a valid, queryable managed property name in the condition.</span></span>

### <a name="example"></a><span data-ttu-id="3b615-113">Пример</span><span class="sxs-lookup"><span data-stu-id="3b615-113">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3b615-114">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b615-114">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="3b615-115">Ответ</span><span class="sxs-lookup"><span data-stu-id="3b615-115">Response</span></span>

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

## <a name="next-steps"></a><span data-ttu-id="3b615-116">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="3b615-116">Next steps</span></span>

- [<span data-ttu-id="3b615-117">Использование API Поиска (Майкрософт) для запроса данных</span><span class="sxs-lookup"><span data-stu-id="3b615-117">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)
