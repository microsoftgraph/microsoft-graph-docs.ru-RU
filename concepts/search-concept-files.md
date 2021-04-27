---
title: Используйте API поиска Майкрософт в Microsoft Graph для поиска файлов
description: API поиска Майкрософт можно использовать для поиска файлов, хранимых в OneDrive или SharePoint.
author: nmoreau
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: dc9d27255ca5306abf85462ca8e5715fe2345dac
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048654"
---
# <a name="use-the-microsoft-search-api-to-search-content-in-onedrive-and-sharepoint"></a><span data-ttu-id="41cdc-103">Используйте API поиска Майкрософт для поиска контента в OneDrive и SharePoint</span><span class="sxs-lookup"><span data-stu-id="41cdc-103">Use the Microsoft Search API to search content in OneDrive and SharePoint</span></span>

<span data-ttu-id="41cdc-104">Используйте API поиска Майкрософт для поиска контента, OneDrive или SharePoint: файлов, папок, списков, элементов списка или сайтов.</span><span class="sxs-lookup"><span data-stu-id="41cdc-104">Use the Microsoft Search API to search content stored in OneDrive or SharePoint: files, folders, lists, list items, or sites.</span></span>

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

<span data-ttu-id="41cdc-105">API поиска позволяет область типов контента для получения в OneDrive или SharePoint, указав свойство **entityTypes** в [searchRequest](/graph/api/resources/searchRequest).</span><span class="sxs-lookup"><span data-stu-id="41cdc-105">The Search API lets you scope the types of content to retrieve in OneDrive or SharePoint by specifying the **entityTypes** property on the [searchRequest](/graph/api/resources/searchRequest).</span></span> <span data-ttu-id="41cdc-106">В этой статье описаны некоторые примеры.</span><span class="sxs-lookup"><span data-stu-id="41cdc-106">This article describes some examples.</span></span>

## <a name="example-1-search-files"></a><span data-ttu-id="41cdc-107">Пример 1. Файлы поиска</span><span class="sxs-lookup"><span data-stu-id="41cdc-107">Example 1: Search files</span></span>

### <a name="request"></a><span data-ttu-id="41cdc-108">Запрос</span><span class="sxs-lookup"><span data-stu-id="41cdc-108">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="41cdc-109">Отклик</span><span class="sxs-lookup"><span data-stu-id="41cdc-109">Response</span></span>

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
                  "driveId": "da61a2b0-4120-4a3f-812b-0fc0d79bf16b",
                  "sharepointIds": {
                      "listId": "c61d1892-ca82-4f53-b16f-6bb8a379e2b2",
                      "listItemId": "1027",
                      "listItemUniqueId": "E320AFEB-AD73-46A2-83D7-985FAA4B206D"
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

## <a name="example-2-search-list-items"></a><span data-ttu-id="41cdc-110">Пример 2. Элементы списка поиска</span><span class="sxs-lookup"><span data-stu-id="41cdc-110">Example 2: Search list items</span></span>

### <a name="request"></a><span data-ttu-id="41cdc-111">Запрос</span><span class="sxs-lookup"><span data-stu-id="41cdc-111">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="41cdc-112">Отклик</span><span class="sxs-lookup"><span data-stu-id="41cdc-112">Response</span></span>

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
                "sharepointIds": {
                    "listId": "33498de0-d695-4d23-ac26-e1bf95a3206e",
                    "listItemId": "13"
                },
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

## <a name="example-3-search-sites"></a><span data-ttu-id="41cdc-113">Пример 3. Сайты поиска</span><span class="sxs-lookup"><span data-stu-id="41cdc-113">Example 3: Search sites</span></span>

### <a name="request"></a><span data-ttu-id="41cdc-114">Запрос</span><span class="sxs-lookup"><span data-stu-id="41cdc-114">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="41cdc-115">Отклик</span><span class="sxs-lookup"><span data-stu-id="41cdc-115">Response</span></span>

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

## <a name="example-4-search-all-content-in-onedrive-and-sharepoint"></a><span data-ttu-id="41cdc-116">Пример 4. Поиск всего контента в OneDrive и SharePoint</span><span class="sxs-lookup"><span data-stu-id="41cdc-116">Example 4: Search all content in OneDrive and SharePoint</span></span>

<span data-ttu-id="41cdc-117">В этом примере запрашивается все содержимое OneDrive и SharePoint сайтов, к которым пользователь с входом в вход имеет доступ к считываемому.</span><span class="sxs-lookup"><span data-stu-id="41cdc-117">This example queries all the content in OneDrive and SharePoint sites to which the signed-in user has read access.</span></span> <span data-ttu-id="41cdc-118">Свойство **ресурса** в ответе возвращает совпадения файлов и папок в качестве объектов **driveItem,** совпадающих с контейнерами (SharePoint списков) в качестве списка и всеми другими совпадениями как **listItem**.</span><span class="sxs-lookup"><span data-stu-id="41cdc-118">The **resource** property in the response returns matches that are files and folders as **driveItem** objects, matches that are containers (SharePoint lists) as **list**, and all other matches as **listItem**.</span></span>

### <a name="request"></a><span data-ttu-id="41cdc-119">Запрос</span><span class="sxs-lookup"><span data-stu-id="41cdc-119">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="41cdc-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="41cdc-120">Response</span></span>

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
                  "driveId": "da61a2b0-4120-4a3f-812b-0fc0d79bf16b",
                  "sharepointIds": {
                      "listId": "c61d1892-ca82-4f53-b16f-6bb8a379e2b2",
                      "listItemId": "1027",
                      "listItemUniqueId": "E320AFEB-AD73-46A2-83D7-985FAA4B206D"
                  }
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

## <a name="example-5-use-filters-in-search-queries"></a><span data-ttu-id="41cdc-121">Пример 5. Использование фильтров в поисковых запросах</span><span class="sxs-lookup"><span data-stu-id="41cdc-121">Example 5: Use filters in search queries</span></span>

<span data-ttu-id="41cdc-122">Вы можете использовать KQL в условиях поиска запросов для OneDrive и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="41cdc-122">You can use KQL in search terms of queries for OneDrive and SharePoint.</span></span> <span data-ttu-id="41cdc-123">Например:</span><span class="sxs-lookup"><span data-stu-id="41cdc-123">For example:</span></span>

- <span data-ttu-id="41cdc-124">`"query": "contoso filetype:docx OR filetype:doc"` областью запроса к документам Word.</span><span class="sxs-lookup"><span data-stu-id="41cdc-124">`"query": "contoso filetype:docx OR filetype:doc"` scopes the query to Word documents.</span></span>
- <span data-ttu-id="41cdc-125">`"query": "test path:\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""` область запроса в определенную папку на сайте.</span><span class="sxs-lookup"><span data-stu-id="41cdc-125">`"query": "test path:\"https://contoso.sharepoint.com/sites/Team Site/Documents/Project\\""` scopes the query to a particular folder within a site.</span></span>
- <span data-ttu-id="41cdc-126">`"query": "contoso AND isDocument=true"` область запроса только для возврата документов.</span><span class="sxs-lookup"><span data-stu-id="41cdc-126">`"query": "contoso AND isDocument=true"` scopes the query to only return documents.</span></span> <span data-ttu-id="41cdc-127">Любой контейнер (папка, библиотека документов) не возвращается.</span><span class="sxs-lookup"><span data-stu-id="41cdc-127">Any container (folder, document library) will not be returned.</span></span>
- <span data-ttu-id="41cdc-128">`"query": "contoso contentclass:STS_List_Events"`область запроса событий Calendar, хранимые в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="41cdc-128">`"query": "contoso contentclass:STS_List_Events"` scopes the query to Calendar events stored in SharePoint.</span></span>
- <span data-ttu-id="41cdc-129">`"query": "contoso (LastModifiedTime > 2021-02-01 AND Created > 2021-02-01)"`область запроса для фильтрации SharePoint и OneDrive элементов по дате</span><span class="sxs-lookup"><span data-stu-id="41cdc-129">`"query": "contoso (LastModifiedTime > 2021-02-01 AND Created > 2021-02-01)"` scopes the query to filter SharePoint and OneDrive items by date</span></span>

<span data-ttu-id="41cdc-130">Чтобы быть допустимым, ограничение свойств должно указывать допустимое, запрашиваемое имя управляемого свойства в состоянии.</span><span class="sxs-lookup"><span data-stu-id="41cdc-130">In order to be valid, properties restriction should specify a valid, queryable managed property name in the condition.</span></span>

## <a name="example-6-specify-select-properties"></a><span data-ttu-id="41cdc-131">Пример 6. Укажите свойства выбора</span><span class="sxs-lookup"><span data-stu-id="41cdc-131">Example 6: Specify select properties</span></span>

<span data-ttu-id="41cdc-132">В ответе можно указать нужные поля в  качестве части поля под свойства [объекта searchHit](/graph/api/resources/searchhit) в ответе.</span><span class="sxs-lookup"><span data-stu-id="41cdc-132">You can specify the fields you want back in the response, as part of the **fields** sub-property of a [searchHit](/graph/api/resources/searchhit) object in the response.</span></span> <span data-ttu-id="41cdc-133">Это способ либо обрезать ответ по проводу, либо запрашивать некоторые конкретные свойства, которые не являются частью схемы из окна.</span><span class="sxs-lookup"><span data-stu-id="41cdc-133">This is a way to either trim down the response over the wire, or to request some specific properties that are not part of the out-of-the-box schema.</span></span>

<span data-ttu-id="41cdc-134">Обратите внимание, что выбор свойств доступен только **для listItem,** так как это единственное SharePoint в Microsoft Graph, которое поддерживает настраиваемые свойства.</span><span class="sxs-lookup"><span data-stu-id="41cdc-134">Note that property selection is only available for **listItem** since this is the only SharePoint entity in Microsoft Graph that supports custom properties.</span></span>

<span data-ttu-id="41cdc-135">Для получения настраиваемой свойства **для driveItem** вместо этого запрашивайте **listItem.**</span><span class="sxs-lookup"><span data-stu-id="41cdc-135">To retrieve a custom property for a **driveItem**, query **listItem** instead.</span></span>

### <a name="request"></a><span data-ttu-id="41cdc-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="41cdc-136">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="41cdc-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="41cdc-137">Response</span></span>

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
                "sharepointIds": {
                    "listId": "33498de0-d695-4d23-ac26-e1bf95a3206e",
                    "listItemId": "13"
                },
                "parentReference": {
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

## <a name="known-limitations"></a><span data-ttu-id="41cdc-138">Известные ограничения</span><span class="sxs-lookup"><span data-stu-id="41cdc-138">Known limitations</span></span>

<span data-ttu-id="41cdc-139">При **поиске диска** необходимо включить в **запросString** термин, содержащийся в имени библиотеки документов.</span><span class="sxs-lookup"><span data-stu-id="41cdc-139">When searching for **drive**, you need to include in the **queryString** a term contained in the name of the document library.</span></span> <span data-ttu-id="41cdc-140">Запрос не `*` поддерживается и не возвращает все доступные диски.</span><span class="sxs-lookup"><span data-stu-id="41cdc-140">Querying `*` is not supported and does not return all available drives.</span></span>

## <a name="next-steps"></a><span data-ttu-id="41cdc-141">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="41cdc-141">Next steps</span></span>

- [<span data-ttu-id="41cdc-142">Использование API Поиска (Майкрософт) для запроса данных</span><span class="sxs-lookup"><span data-stu-id="41cdc-142">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview)
