---
title: Поиск файлов (включая externalFile)
description: API запросов позволяет выполнять поиск по файлам (DriveItem или внешним файлам).
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 95a8b99b9970ec239935ee2c35afeec581a1b35f
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703949"
---
# <a name="search-files-including-externalfile"></a><span data-ttu-id="5de8a-103">Поиск файлов (включая externalFile)</span><span class="sxs-lookup"><span data-stu-id="5de8a-103">Search files (including externalFile)</span></span>

<span data-ttu-id="5de8a-104">API службы поиска Microsoft позволяет искать файлы, хранящиеся в SharePoint или OneDrive.</span><span class="sxs-lookup"><span data-stu-id="5de8a-104">The Microsoft Search API lets you search files stored in SharePoint or OneDrive.</span></span> <span data-ttu-id="5de8a-105">Он использует модель релевантности, которая использует сигналы из Microsoft Graph о связи и действиях пользователей.</span><span class="sxs-lookup"><span data-stu-id="5de8a-105">It uses a relevance model which makes use of signals from Microsoft Graph about users' relations and activities.</span></span> <span data-ttu-id="5de8a-106">Это позволяет вернуть и повысить контент, который пользователи волнует, в процессе поиска файлов, который соответствует вкладке **файлы** , в которой отображаются результаты поиска в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5de8a-106">This allows returning and promoting content that users care about, in a file search experience that is consistent with the **Files** tab that lists search results in SharePoint.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<span data-ttu-id="5de8a-107">Кроме того, API может подавать внешние файлы, предоставляемые через ресурс [екстерналфиле](/graph/api/resources/externalfile?view=graph-rest-beta) .</span><span class="sxs-lookup"><span data-stu-id="5de8a-107">In addition, the API can surface external files exposed via the [externalFile](/graph/api/resources/externalfile?view=graph-rest-beta) resource.</span></span>

## <a name="search-sharepoint-or-onedrive-files"></a><span data-ttu-id="5de8a-108">Поиск файлов SharePoint или OneDrive</span><span class="sxs-lookup"><span data-stu-id="5de8a-108">Search SharePoint or OneDrive files</span></span>

<span data-ttu-id="5de8a-109">KQL можно использовать в терминах поиска запросов для SharePoint и OneDrive.</span><span class="sxs-lookup"><span data-stu-id="5de8a-109">You can use KQL in search terms of queries for SharePoint and OneDrive.</span></span> <span data-ttu-id="5de8a-110">Пример:</span><span class="sxs-lookup"><span data-stu-id="5de8a-110">For example:</span></span>

- <span data-ttu-id="5de8a-111">`"query" : "contoso filetype:docx OR filetype:doc"`области запрашивает документы Word</span><span class="sxs-lookup"><span data-stu-id="5de8a-111">`"query" : "contoso filetype:docx OR filetype:doc"` scopes queries to Word documents</span></span>
- <span data-ttu-id="5de8a-112">`"query": "test path:\\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""`ограничивает область запроса определенной папкой на сайте.</span><span class="sxs-lookup"><span data-stu-id="5de8a-112">`"query": "test path:\\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""` scopes the query to a particular folder within a site.</span></span>

<span data-ttu-id="5de8a-113">Чтобы быть допустимым, ограничение свойств должно указывать допустимое имя управляемого свойства, поддерживающего запросы, в условии.</span><span class="sxs-lookup"><span data-stu-id="5de8a-113">In order to be valid, properties restriction should specify a valid Queryable managed property name in the condition.</span></span>

### <a name="example"></a><span data-ttu-id="5de8a-114">Пример</span><span class="sxs-lookup"><span data-stu-id="5de8a-114">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5de8a-115">Запрос</span><span class="sxs-lookup"><span data-stu-id="5de8a-115">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="5de8a-116">Отклик</span><span class="sxs-lookup"><span data-stu-id="5de8a-116">Response</span></span>

<span data-ttu-id="5de8a-117">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5de8a-117">Here is an example of the response.</span></span>

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

## <a name="search-external-files-well-known-types"></a><span data-ttu-id="5de8a-118">Поиск внешних файлов (известных типов)</span><span class="sxs-lookup"><span data-stu-id="5de8a-118">Search external files (well-known types)</span></span>

<span data-ttu-id="5de8a-119">[Соединитель файлов общего доступа](/MicrosoftSearch/file-share-connector) — это соединитель "из поля", доступный в Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="5de8a-119">[File share connector](/MicrosoftSearch/file-share-connector) is an "out of the box" connector available in Microsoft Search.</span></span> <span data-ttu-id="5de8a-120">Он позволяет индексировать файлы, доступные в общей папке.</span><span class="sxs-lookup"><span data-stu-id="5de8a-120">It enables you to index files available on a file share.</span></span> <span data-ttu-id="5de8a-121">Вы можете использовать API запросов для запроса всех внешних файлов.</span><span class="sxs-lookup"><span data-stu-id="5de8a-121">You can use the query API to query all external files.</span></span>

<!-- markdownlint-disable MD024 -->
### <a name="example"></a><span data-ttu-id="5de8a-122">Пример</span><span class="sxs-lookup"><span data-stu-id="5de8a-122">Example</span></span>

<span data-ttu-id="5de8a-123">Следующий пример возвращает все настроенные соединители Екстерналфиле для клиента и сортирует результаты по релевантности.</span><span class="sxs-lookup"><span data-stu-id="5de8a-123">The following example returns all configured externalFile connector for the tenant, and sorts the results by relevance.</span></span>

#### <a name="request"></a><span data-ttu-id="5de8a-124">Запрос</span><span class="sxs-lookup"><span data-stu-id="5de8a-124">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="5de8a-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="5de8a-125">Response</span></span>

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

## <a name="search-all-files-including-externalfile-instances"></a><span data-ttu-id="5de8a-126">Поиск во всех файлах (в том числе экземплярах Екстерналфиле)</span><span class="sxs-lookup"><span data-stu-id="5de8a-126">Search all files (including externalFile instances)</span></span>

<span data-ttu-id="5de8a-127">Можно выполнять поиск во всех файлах клиента, включая [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) и все внешние файлы, указывая в запросе поиска два типа сущности.</span><span class="sxs-lookup"><span data-stu-id="5de8a-127">You can search all the files in a tenant, including [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) and all external files, by specifying two entity types in the search request.</span></span>

<span data-ttu-id="5de8a-128">Ответ предоставляет сочетание экземпляров **driveItem** и екстерналитем в `_sources` поле каждого объекта [сеарчхит](/graph/api/resources/searchhit?view=graph-rest-beta) .</span><span class="sxs-lookup"><span data-stu-id="5de8a-128">The response provide a mix of **driveItem** and externalItem instances in the `_sources` field of each [searchHit](/graph/api/resources/searchhit?view=graph-rest-beta) object.</span></span>

### <a name="example"></a><span data-ttu-id="5de8a-129">Пример</span><span class="sxs-lookup"><span data-stu-id="5de8a-129">Example</span></span>

<span data-ttu-id="5de8a-130">В следующем примере возвращаются все настроенные соединители **екстерналфиле** и объекты **driveItem** клиента, которые удовлетворяют условиям поиска.</span><span class="sxs-lookup"><span data-stu-id="5de8a-130">The following example returns all configured **externalFile** connector and **driveItem** objects of the tenant's that satisfy the search terms.</span></span> <span data-ttu-id="5de8a-131">Результаты сортируются по релевантности.</span><span class="sxs-lookup"><span data-stu-id="5de8a-131">It sorts the results by relevance.</span></span>

### <a name="request"></a><span data-ttu-id="5de8a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5de8a-132">Request</span></span>

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

## <a name="known-limitations"></a><span data-ttu-id="5de8a-133">Известные ограничения</span><span class="sxs-lookup"><span data-stu-id="5de8a-133">Known limitations</span></span>

<span data-ttu-id="5de8a-134">Невозможно выполнить запрос к определенному Коннектионид.</span><span class="sxs-lookup"><span data-stu-id="5de8a-134">You cannot scope a query to a particular connectionId.</span></span>

## <a name="next-steps"></a><span data-ttu-id="5de8a-135">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="5de8a-135">Next steps</span></span>

<span data-ttu-id="5de8a-136">Дополнительные сведения:</span><span class="sxs-lookup"><span data-stu-id="5de8a-136">Find out more about:</span></span>

- [<span data-ttu-id="5de8a-137">Использование API поиска</span><span class="sxs-lookup"><span data-stu-id="5de8a-137">Use the search API</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)
