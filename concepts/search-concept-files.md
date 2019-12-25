---
title: Использование API службы поиска Microsoft в Microsoft Graph для поиска файлов
description: Вы можете использовать API службы поиска Microsoft для поиска файлов, хранящихся в SharePoint или OneDrive.
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 0b8db24a8b9ccd63ac3d3be800b209a64eb3aa9d
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866919"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-search-files"></a><span data-ttu-id="c3a07-103">Использование API службы поиска Microsoft в Microsoft Graph для поиска файлов</span><span class="sxs-lookup"><span data-stu-id="c3a07-103">Use the Microsoft Search API in Microsoft Graph to search files</span></span>

<span data-ttu-id="c3a07-104">Вы можете использовать API службы поиска Microsoft для поиска файлов, хранящихся в SharePoint или OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c3a07-104">You can use the Microsoft Search API to search files stored in SharePoint or OneDrive.</span></span> <span data-ttu-id="c3a07-105">API поиска Microsoft использует модель релевантности, которая использует сигналы из Microsoft Graph о связях и действиях пользователей.</span><span class="sxs-lookup"><span data-stu-id="c3a07-105">The Microsoft Search API uses a relevance model that makes use of signals from Microsoft Graph about users' relationships and activities.</span></span> <span data-ttu-id="c3a07-106">Это позволяет вернуть и повысить уровень содержимого, которое пользователи волнует, в интерфейсе поиска файлов, который соответствует вкладке **файлы** , в которой отображаются результаты поиска в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c3a07-106">This enables you to return and promote the content that users care about, in a file search experience that is consistent with the **Files** tab that lists search results in SharePoint.</span></span> 

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<span data-ttu-id="c3a07-107">API также может подавать внешние файлы, предоставляемые через ресурс [екстерналфиле](/graph/api/resources/externalfile?view=graph-rest-beta) .</span><span class="sxs-lookup"><span data-stu-id="c3a07-107">The API can also surface external files exposed via the [externalFile](/graph/api/resources/externalfile?view=graph-rest-beta) resource.</span></span>

## <a name="search-sharepoint-or-onedrive-files"></a><span data-ttu-id="c3a07-108">Поиск файлов SharePoint или OneDrive</span><span class="sxs-lookup"><span data-stu-id="c3a07-108">Search SharePoint or OneDrive files</span></span>

<span data-ttu-id="c3a07-109">KQL можно использовать в терминах поиска запросов для SharePoint и OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c3a07-109">You can use KQL in search terms of queries for SharePoint and OneDrive.</span></span> <span data-ttu-id="c3a07-110">Пример:</span><span class="sxs-lookup"><span data-stu-id="c3a07-110">For example:</span></span>

- <span data-ttu-id="c3a07-111">`"query": "contoso filetype:docx OR filetype:doc"`ограничивает область запроса документами Word.</span><span class="sxs-lookup"><span data-stu-id="c3a07-111">`"query": "contoso filetype:docx OR filetype:doc"` scopes the query to Word documents.</span></span>
- <span data-ttu-id="c3a07-112">`"query": "test path:\\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""`ограничивает область запроса определенной папкой на сайте.</span><span class="sxs-lookup"><span data-stu-id="c3a07-112">`"query": "test path:\\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""` scopes the query to a particular folder within a site.</span></span>

<span data-ttu-id="c3a07-113">Для того чтобы оно было допустимым, ограничение свойств должно указывать допустимое имя управляемого свойства, запрашиваемое в условии.</span><span class="sxs-lookup"><span data-stu-id="c3a07-113">In order to be valid, properties restriction should specify a valid, queryable managed property name in the condition.</span></span>

### <a name="example"></a><span data-ttu-id="c3a07-114">Пример</span><span class="sxs-lookup"><span data-stu-id="c3a07-114">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c3a07-115">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3a07-115">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="c3a07-116">Ответ</span><span class="sxs-lookup"><span data-stu-id="c3a07-116">Response</span></span>

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

## <a name="search-external-files-well-known-types"></a><span data-ttu-id="c3a07-117">Поиск внешних файлов (известных типов)</span><span class="sxs-lookup"><span data-stu-id="c3a07-117">Search external files (well-known types)</span></span>

<span data-ttu-id="c3a07-118">По умолчанию в Microsoft Search есть доступ [к файловому ресурсному соединителю](/MicrosoftSearch/file-share-connector) .</span><span class="sxs-lookup"><span data-stu-id="c3a07-118">The [file share connector](/MicrosoftSearch/file-share-connector) is available in Microsoft Search by default.</span></span> <span data-ttu-id="c3a07-119">Его можно использовать для индексации файлов, доступных в общей папке.</span><span class="sxs-lookup"><span data-stu-id="c3a07-119">You can use it to index files available on a file share.</span></span> <span data-ttu-id="c3a07-120">Вы можете использовать API запросов для запроса всех внешних файлов.</span><span class="sxs-lookup"><span data-stu-id="c3a07-120">You can use the query API to query all external files.</span></span>

<!-- markdownlint-disable MD024 -->
### <a name="example"></a><span data-ttu-id="c3a07-121">Пример</span><span class="sxs-lookup"><span data-stu-id="c3a07-121">Example</span></span>

<span data-ttu-id="c3a07-122">В следующем примере возвращаются все настроенные внешние файлы для клиента, а результаты сортируются по релевантности.</span><span class="sxs-lookup"><span data-stu-id="c3a07-122">The following example returns all configured external files for the tenant, and sorts the results by relevance.</span></span>

#### <a name="request"></a><span data-ttu-id="c3a07-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3a07-123">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="c3a07-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="c3a07-124">Response</span></span>

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

## <a name="search-all-files-including-externalfile-instances"></a><span data-ttu-id="c3a07-125">Поиск во всех файлах (в том числе экземплярах Екстерналфиле)</span><span class="sxs-lookup"><span data-stu-id="c3a07-125">Search all files (including externalFile instances)</span></span>

<span data-ttu-id="c3a07-126">Можно выполнять поиск по всем файлам в клиенте, включая файлы, хранящиеся в [элементов driveitem](/graph/api/resources/driveitem?view=graph-rest-beta) и внешние файлы, указывая два типа сущностей в запросе поиска.</span><span class="sxs-lookup"><span data-stu-id="c3a07-126">You can search all the files in a tenant, including files stored in [driveItems](/graph/api/resources/driveitem?view=graph-rest-beta) and external files, by specifying two entity types in the search request.</span></span>

<span data-ttu-id="c3a07-127">Ответ содержит экземпляры **driveItem** и **екстерналитем** в `_sources` поле каждого объекта [сеарчхит](/graph/api/resources/searchhit?view=graph-rest-beta) .</span><span class="sxs-lookup"><span data-stu-id="c3a07-127">The response includes **driveItem** and **externalItem** instances in the `_sources` field of each [searchHit](/graph/api/resources/searchhit?view=graph-rest-beta) object.</span></span>

### <a name="example"></a><span data-ttu-id="c3a07-128">Пример</span><span class="sxs-lookup"><span data-stu-id="c3a07-128">Example</span></span>

<span data-ttu-id="c3a07-129">В следующем примере возвращаются все настроенные объекты **екстерналфиле** и **driveItem** в клиенте, которые удовлетворяют условиям поиска.</span><span class="sxs-lookup"><span data-stu-id="c3a07-129">The following example returns all configured **externalFile** and **driveItem** objects in the tenant that satisfy the search terms.</span></span> <span data-ttu-id="c3a07-130">Результаты сортируются по релевантности.</span><span class="sxs-lookup"><span data-stu-id="c3a07-130">It sorts the results by relevance.</span></span>

### <a name="request"></a><span data-ttu-id="c3a07-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3a07-131">Request</span></span>

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

## <a name="known-limitations"></a><span data-ttu-id="c3a07-132">Известные ограничения</span><span class="sxs-lookup"><span data-stu-id="c3a07-132">Known limitations</span></span>

<span data-ttu-id="c3a07-133">Вы не можете ограничить запрос определенным ИДЕНТИФИКАТОРом подключения.</span><span class="sxs-lookup"><span data-stu-id="c3a07-133">You cannot scope a query to a particular connection ID.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c3a07-134">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="c3a07-134">Next steps</span></span>

- [<span data-ttu-id="c3a07-135">Использование API Поиска (Майкрософт) для запроса данных</span><span class="sxs-lookup"><span data-stu-id="c3a07-135">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)

