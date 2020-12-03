---
title: Использование API службы поиска Microsoft в Microsoft Graph для поиска файлов
description: Вы можете использовать API службы поиска Microsoft для поиска файлов, хранящихся в OneDrive или SharePoint.
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 604fb0cac6a79f78cadf31df057dceb2524e3cbb
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523695"
---
# <a name="use-the-microsoft-search-api-to-search-content-in-onedrive-and-sharepoint"></a><span data-ttu-id="1fc0b-103">Использование API службы поиска Microsoft для поиска содержимого в OneDrive и SharePoint</span><span class="sxs-lookup"><span data-stu-id="1fc0b-103">Use the Microsoft Search API to search content in OneDrive and SharePoint</span></span>

<span data-ttu-id="1fc0b-104">Используйте API службы поиска Microsoft для поиска контента, хранящегося в OneDrive или SharePoint: файлы, папки, списки, элементы списков или сайты.</span><span class="sxs-lookup"><span data-stu-id="1fc0b-104">Use the Microsoft Search API to search content stored in OneDrive or SharePoint: files, folders, lists, list items, or sites.</span></span>

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

<span data-ttu-id="1fc0b-105">API поиска позволяет ограничить типы контента, извлекаемого в OneDrive или SharePoint, путем указания свойства **EntityTypes** в [сеарчрекуест](/graph/api/resources/searchRequest).</span><span class="sxs-lookup"><span data-stu-id="1fc0b-105">The Search API lets you scope the types of content to retrieve in OneDrive or SharePoint by specifying the **entityTypes** property on the [searchRequest](/graph/api/resources/searchRequest).</span></span> <span data-ttu-id="1fc0b-106">В следующей части этой статьи показаны некоторые примеры:</span><span class="sxs-lookup"><span data-stu-id="1fc0b-106">The later part of this article shows a few examples:</span></span>

- [<span data-ttu-id="1fc0b-107">Пример 1: Поиск файлов</span><span class="sxs-lookup"><span data-stu-id="1fc0b-107">Example 1: Search files</span></span>](#example-1-search-files)
- [<span data-ttu-id="1fc0b-108">Пример 2: Поиск элементов списка</span><span class="sxs-lookup"><span data-stu-id="1fc0b-108">Example 2: Search list items</span></span>](#example-2-search-list-items)
- [<span data-ttu-id="1fc0b-109">Пример 3: Поиск на сайтах</span><span class="sxs-lookup"><span data-stu-id="1fc0b-109">Example 3: Search sites</span></span>](#example-3-search-sites)
- [<span data-ttu-id="1fc0b-110">Пример 4: Поиск по всему контенту в OneDrive и SharePoint</span><span class="sxs-lookup"><span data-stu-id="1fc0b-110">Example 4: Search all content in OneDrive and SharePoint</span></span>](#example-4-search-all-content-in-onedrive-and-sharepoint)
- [<span data-ttu-id="1fc0b-111">Пример 5: использование фильтров в поисковых запросах</span><span class="sxs-lookup"><span data-stu-id="1fc0b-111">Example 5: Use filters in search queries</span></span>](#example-5-use-filters-in-search-queries)
- [<span data-ttu-id="1fc0b-112">Пример 6: Указание свойств Select</span><span class="sxs-lookup"><span data-stu-id="1fc0b-112">Example 6: Specify select properties</span></span>](#example-6-specify-select-properties)


## <a name="example-1-search-files"></a><span data-ttu-id="1fc0b-113">Пример 1: Поиск файлов</span><span class="sxs-lookup"><span data-stu-id="1fc0b-113">Example 1: Search files</span></span>

### <a name="request"></a><span data-ttu-id="1fc0b-114">Запрос</span><span class="sxs-lookup"><span data-stu-id="1fc0b-114">Request</span></span>

```HTTP
POST /search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "driveItem"
      ],
      "query": {
        "queryString": "contoso"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="1fc0b-115">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fc0b-115">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#search",
  "value": [
    {
      "searchTerms": [
        "contoso"
      ],
      "hitsContainers": [
        {
          "total": 1,
          "moreResultsAvailable": false,
          "hits": [
            {
              "hitId": "FlULeN/ui/1GjLx1rUfio5UAAEl",
              "rank": 1,
              "summary": "<c0>Contoso</c0> Detailed Design <ddd/>",
              "resource": {
                "@odata.type": "#microsoft.graph.driveItem",
                "createdDateTime": "2019-06-10T06:37:43Z",
                "lastModifiedDateTime": "2019-06-10T06:37:43Z",
                "name": "web_part_test_long Notebook",
                "webUrl": "https://contoso.sharepoint.com/sites/contoso-team/contoso-designs.docx",
                "createdBy": {
                 "user": {
                   "displayName": "Michaelvincent Santos;Provisioning User"
                  }
                },
                "lastModifiedBy": {
                  "user": {
                    "displayName": "Richard Mayer"
                  }
                },
                "parentReference": {
                  "siteId": "m365x231305.sharepoint.com,5724d91f-650c-4810-83cc-61a8818917d6,c3ba25dc-2c9f-48cb-83be-74cdf68ea5a0",
                  "driveId": "da61a2b0-4120-4a3f-812b-0fc0d79bf16b"
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

## <a name="example-2-search-list-items"></a><span data-ttu-id="1fc0b-116">Пример 2: Поиск элементов списка</span><span class="sxs-lookup"><span data-stu-id="1fc0b-116">Example 2: Search list items</span></span>

### <a name="request"></a><span data-ttu-id="1fc0b-117">Запрос</span><span class="sxs-lookup"><span data-stu-id="1fc0b-117">Request</span></span>

```HTTP
POST /search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "listItem"
      ],
      "query": {
        "queryString": "contoso"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="1fc0b-118">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fc0b-118">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#search",
  "value": [
    {
      "searchTerms": [
        "contoso"
      ],
      "hitsContainers": [
        {
          "total": 1,
          "moreResultsAvailable": false,
          "hits": [
            {
              "hitId": "FlULeN/ui/1GjLx1rUfio5UAAEl",
              "rank": 1,
              "summary": "",
              "resource": {
                "@odata.type": "#microsoft.graph.listItem",
                "createdDateTime": "2019-06-10T06:37:43Z",
                "lastModifiedDateTime": "2019-06-10T06:37:43Z",
                "name": "web_part_test_long Notebook",
                "webUrl": "https://contoso.sharepoint.com/sites/contoso-team/Lists/Issue tracker list/DispForm.aspx?ID=1",
                "createdBy": {
                 "user": {
                   "displayName": "Michaelvincent Santos;Provisioning User"
                  }
                },
                "lastModifiedBy": {
                  "user": {
                    "displayName": "Richard Mayer"
                  }
                },
                "parentReference": {
                  "sharepointIds":{
                    "listId":"da61a2b0-4120-4a3f-812b-0fc0d79bf16b"  
                  },
                  "siteId": "m365x231305.sharepoint.com,5724d91f-650c-4810-83cc-61a8818917d6,c3ba25dc-2c9f-48cb-83be-74cdf68ea5a0"
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

## <a name="example-3-search-sites"></a><span data-ttu-id="1fc0b-119">Пример 3: Поиск на сайтах</span><span class="sxs-lookup"><span data-stu-id="1fc0b-119">Example 3: Search sites</span></span>

### <a name="request"></a><span data-ttu-id="1fc0b-120">Запрос</span><span class="sxs-lookup"><span data-stu-id="1fc0b-120">Request</span></span>

```HTTP
POST /search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "site"
      ],
      "query": {
        "queryString": "contoso"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="1fc0b-121">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fc0b-121">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#search",
  "value": [
    {
      "searchTerms": [
        "contoso"
      ],
      "hitsContainers": [
        {
          "total": 1,
          "moreResultsAvailable": false,
          "hits": [
            {
              "hitId": "contoso.sharepoint.com,6598ee0b-0f5f-4416-a0ae-66d864efb43a,60024ce8-e74d-4d63-a939-ad00cd738670",
              "rank": 1,
              "summary": "",
              "resource": {
                "@odata.type": "#microsoft.graph.site",
                "id": "contoso.sharepoint.com,6598ee0b-0f5f-4416-a0ae-66d864efb43a,60024ce8-e74d-4d63-a939-ad00cd738670",
                "createdDateTime": "2019-06-10T06:37:43Z",
                "description": "Contoso Communication Site",
                "lastModifiedDateTime": "2020-08-30T06:41:56Z",
                "webUrl": "https://contoso.sharepoint.com/sites/contoso-team/"
              }
            }
          ]
        }
      ]
    }
  ]
}
```

## <a name="example-4-search-all-content-in-onedrive-and-sharepoint"></a><span data-ttu-id="1fc0b-122">Пример 4: Поиск по всему контенту в OneDrive и SharePoint</span><span class="sxs-lookup"><span data-stu-id="1fc0b-122">Example 4: Search all content in OneDrive and SharePoint</span></span>

<span data-ttu-id="1fc0b-123">В этом примере запрашивается весь контент на сайтах OneDrive и SharePoint, к которым вошедшего в систему пользователя предоставлен доступ для чтения.</span><span class="sxs-lookup"><span data-stu-id="1fc0b-123">This example queries all the content in OneDrive and SharePoint sites to which the signed-in user has read access.</span></span> <span data-ttu-id="1fc0b-124">Свойство **ресурса** в ответе возвращает совпадения, которые представляют собой файлы и папки в виде объектов **driveItem** , совпадений, которые являются контейнерами **(списками SharePoint), и** всеми остальными совпадениями как **ListItem**.</span><span class="sxs-lookup"><span data-stu-id="1fc0b-124">The **resource** property in the response returns matches that are files and folders as **driveItem** objects, matches that are containers (SharePoint lists) as **list**, and all other matches as **listItem**.</span></span>

### <a name="request"></a><span data-ttu-id="1fc0b-125">Запрос</span><span class="sxs-lookup"><span data-stu-id="1fc0b-125">Request</span></span>

```HTTP
POST /search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "driveItem", "listItem", "list"
      ],
      "query": {
        "queryString": "contoso"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="1fc0b-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fc0b-126">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#search",
  "value": [
    {
      "searchTerms": [
        "contoso"
      ],
      "hitsContainers": [
        {
          "total": 1,
          "moreResultsAvailable": false,
          "hits": [
            {
              "@odata.type": "#microsoft.graph.searchHitsContainer",
              "hitId": "FlULeN/ui/1GjLx1rUfio5UAAEl",
              "rank": 1,
              "summary": "<c0>Contoso</c0> Detailed Design <ddd/>",
              "resource": {
                "@odata.type": "#microsoft.graph.driveItem",
                "createdDateTime": "2019-06-10T06:37:43Z",
                "lastModifiedDateTime": "2019-06-10T06:37:43Z",
                "name": "web_part_test_long Notebook",
                "webUrl": "https://contoso.sharepoint.com/sites/contoso-team/contoso-designs.docx",
                "createdBy": {
                 "user": {
                   "displayName": "Michaelvincent Santos;Provisioning User"
                  }
                },
                "lastModifiedBy": {
                  "user": {
                    "displayName": "Richard Mayer"
                  }
                },
                "parentReference": {
                  "siteId": "m365x231305.sharepoint.com,5724d91f-650c-4810-83cc-61a8818917d6,c3ba25dc-2c9f-48cb-83be-74cdf68ea5a0",
                  "driveId": "da61a2b0-4120-4a3f-812b-0fc0d79bf16b"
                },
                "fileSystemInfo": {
                  "createdDateTime": "2019-06-10T06:37:43Z",
                  "lastModifiedDateTime": "2019-06-10T06:37:43Z"
                }
              }
            },
            {
              "@odata.type": "#microsoft.graph.searchHit",
              "hitId": "51eef59e-5d49-4d28-96f0-864cf90765e0",
              "rank": 2,
              "summary": "",
              "resource": {
                "@odata.type": "#microsoft.graph.list",
                "displayName": "Contoso - Documents",
                "id": "51eef59e-5d49-4d28-96f0-864cf90765e0",
                "description": "",
                "lastModifiedDateTime": "2020-07-08T18:17:59+00:00",
                "name": "Shared Documents",
                "parentReference": {
                  "siteId": "microsoft.sharepoint-df.com,220fd155-0ea2-477c-a816-5c08fdc45f5d,fad16ab6-0736-4fbc-a053-087296b47c99"
                },
                "webUrl": "https://microsoft.sharepoint-df.com/teams/spoppe/collab/TaskBoard/Contoso/Shared Documents/Forms/AllItems.aspx"
              }
            }
          ]
        }
      ]
    }
  ]
}
```

## <a name="example-5-use-filters-in-search-queries"></a><span data-ttu-id="1fc0b-127">Пример 5: использование фильтров в поисковых запросах</span><span class="sxs-lookup"><span data-stu-id="1fc0b-127">Example 5: Use filters in search queries</span></span>

<span data-ttu-id="1fc0b-128">KQL можно использовать в условиях поиска запросов для OneDrive и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1fc0b-128">You can use KQL in search terms of queries for OneDrive and SharePoint.</span></span> <span data-ttu-id="1fc0b-129">Пример:</span><span class="sxs-lookup"><span data-stu-id="1fc0b-129">For example:</span></span>

- <span data-ttu-id="1fc0b-130">`"query": "contoso filetype:docx OR filetype:doc"` ограничивает область запроса документами Word.</span><span class="sxs-lookup"><span data-stu-id="1fc0b-130">`"query": "contoso filetype:docx OR filetype:doc"` scopes the query to Word documents.</span></span>
- <span data-ttu-id="1fc0b-131">`"query": "test path:\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""` ограничивает область запроса определенной папкой на сайте.</span><span class="sxs-lookup"><span data-stu-id="1fc0b-131">`"query": "test path:\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""` scopes the query to a particular folder within a site.</span></span>
- <span data-ttu-id="1fc0b-132">`"query": "contoso AND isDocument=true"` ограничивает область запроса, возвращающий только документы.</span><span class="sxs-lookup"><span data-stu-id="1fc0b-132">`"query": "contoso AND isDocument=true"` scopes the query to only return documents.</span></span> <span data-ttu-id="1fc0b-133">Любой контейнер (папка, Библиотека документов) не будет возвращен.</span><span class="sxs-lookup"><span data-stu-id="1fc0b-133">Any container (folder, document library) will not be returned.</span></span>
- <span data-ttu-id="1fc0b-134">`"query": "contoso contentclass:STS_List_Events"` область действия запроса на события календаря, хранящиеся в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1fc0b-134">`"query": "contoso contentclass:STS_List_Events"` scopes the query to Calendar events stored in SharePoint.</span></span>

<span data-ttu-id="1fc0b-135">Для того чтобы оно было допустимым, ограничение свойств должно указывать допустимое имя управляемого свойства, запрашиваемое в условии.</span><span class="sxs-lookup"><span data-stu-id="1fc0b-135">In order to be valid, properties restriction should specify a valid, queryable managed property name in the condition.</span></span>

## <a name="example-6-specify-select-properties"></a><span data-ttu-id="1fc0b-136">Пример 6: Указание свойств Select</span><span class="sxs-lookup"><span data-stu-id="1fc0b-136">Example 6: Specify select properties</span></span>

<span data-ttu-id="1fc0b-137">Вы можете указать поля, которые вы хотите вернуть в ответе, как часть вложенного свойства **Fields** объекта [сеарчхит](/graph/api/resources/searchhit) в отклике.</span><span class="sxs-lookup"><span data-stu-id="1fc0b-137">You can specify the fields you want back in the response, as part of the **fields** sub-property of a [searchHit](/graph/api/resources/searchhit) object in the response.</span></span> <span data-ttu-id="1fc0b-138">Это позволяет либо обрезать ответ по сети, либо запрашивать определенные свойства, не входящие в состав встроенной схемы.</span><span class="sxs-lookup"><span data-stu-id="1fc0b-138">This is a way to either trim down the response over the wire, or to request some specific properties that are not part of the out-of-the-box schema.</span></span>

<span data-ttu-id="1fc0b-139">Обратите внимание, что выбор свойства доступен только для элемента **ListItem** , так как это единственная сущность SharePoint в Microsoft Graph, поддерживающая настраиваемые свойства.</span><span class="sxs-lookup"><span data-stu-id="1fc0b-139">Note that property selection is only available for **listItem** since this is the only SharePoint entity in Microsoft Graph that supports custom properties.</span></span>

<span data-ttu-id="1fc0b-140">Чтобы получить настраиваемое свойство для объекта **driveItem**, необходимо вместо этого запросить свойство **ListItem** .</span><span class="sxs-lookup"><span data-stu-id="1fc0b-140">To retrieve a custom property for a **driveItem**, query **listItem** instead.</span></span>

### <a name="request"></a><span data-ttu-id="1fc0b-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="1fc0b-141">Request</span></span>

```HTTP
POST /search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "listItem"
      ],
      "query": {
        "queryString": "contoso"
      },
      "fields": [
          "title",
          "contentclass"
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="1fc0b-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fc0b-142">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#search",
  "value": [
    {
      "searchTerms": [
        "contoso"
      ],
      "hitsContainers": [
        {
          "total": 1,
          "moreResultsAvailable": false,
          "hits": [
            {
              "hitId": "contoso.sharepoint.com,6598ee0b-0f5f-4416-a0ae-66d864efb43a,60024ce8-e74d-4d63-a939-ad00cd738670",
              "rank": 1,
              "summary": "",
              "resource": {
                "@odata.type": "#microsoft.graph.listItem",
                "createdDateTime": "2019-06-10T06:37:43Z",
                "webUrl": "https://contoso.sharepoint.com/sites/contoso-team/contoso-designs.docx",
                "parentReference": {
                  "sharepointIds":{
                    "listId":"da61a2b0-4120-4a3f-812b-0fc0d79bf16b"  
                  },
                  "siteId": "m365x231305.sharepoint.com,5724d91f-650c-4810-83cc-61a8818917d6,c3ba25dc-2c9f-48cb-83be-74cdf68ea5a0"
                },
                "fields": {
                  "contentclass": "STS_ListItem_GenericList",
                  "title": "Contoso issue "
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

## <a name="known-limitations"></a><span data-ttu-id="1fc0b-143">Известные ограничения</span><span class="sxs-lookup"><span data-stu-id="1fc0b-143">Known limitations</span></span>

<span data-ttu-id="1fc0b-144">При поиске **диска** необходимо включить в **строку queryString** термин, содержащийся в имени библиотеки документов.</span><span class="sxs-lookup"><span data-stu-id="1fc0b-144">When searching for **drive**, you need to include in the **queryString** a term contained in the name of the document library.</span></span> <span data-ttu-id="1fc0b-145">Запросы `*` не поддерживаются и не возвращают все доступные диски.</span><span class="sxs-lookup"><span data-stu-id="1fc0b-145">Querying `*` is not supported and does not return all available drives.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1fc0b-146">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="1fc0b-146">Next steps</span></span>

- [<span data-ttu-id="1fc0b-147">Использование API Поиска (Майкрософт) для запроса данных</span><span class="sxs-lookup"><span data-stu-id="1fc0b-147">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview)
