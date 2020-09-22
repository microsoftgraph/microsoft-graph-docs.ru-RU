---
title: Использование API службы поиска Microsoft в Microsoft Graph для поиска событий календаря
description: Вы можете выполнять поиск в собственном календаре пользователя.
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 802f6fdbb45d93ed46cd0b8033816abf5df07288
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192597"
---
# <a name="use-the-microsoft-search-api-to-search-calendar-events"></a><span data-ttu-id="c7357-103">Использование API службы поиска Microsoft для поиска событий календаря</span><span class="sxs-lookup"><span data-stu-id="c7357-103">Use the Microsoft Search API to search calendar events</span></span>

<span data-ttu-id="c7357-104">Используйте API службы поиска Microsoft для поиска событий в основном календаре вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="c7357-104">Use the Microsoft Search API to search for events in the signed-in user’s primary calendar.</span></span> <span data-ttu-id="c7357-105">Удостоверение пользователя для поиска основано на маркере проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="c7357-105">The user identity for the search is based on the auth token.</span></span>

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

## <a name="example"></a><span data-ttu-id="c7357-106">Пример</span><span class="sxs-lookup"><span data-stu-id="c7357-106">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7357-107">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7357-107">Request</span></span>

<span data-ttu-id="c7357-108">В этом примере выполняется поиск ключевого слова "contoso" в календаре пользователя и возвращается до 25 результатов.</span><span class="sxs-lookup"><span data-stu-id="c7357-108">This example searches in the user's calendar for the keyword "contoso", and will return up to 25 results.</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "event"
      ],
      "query": {
        "queryString":"contoso"
      },
      "from": 0,
      "size": 25
    }
  ]
}
```

#### <a name="response"></a><span data-ttu-id="c7357-109">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7357-109">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#search",
  "value": [
  {
   "@odata.type": "#microsoft.graph.searchResponse",
   "searchTerms": [
    "contoso"
   ],
   "hitsContainers": [
    {
     "@odata.type": "#microsoft.graph.searchHitsContainer",
     "hits": [
      {
       "@odata.type": "#microsoft.graph.searchHit",
       "hitId": "AAMkADEwODY2NzllLTQ3MmEtNGRlMC05ZTUyLTE4ZDRhYmU1ZGM3NABGAAAAAAA3+iYQBnJnQabRVDelNhnzBwAejhWkAOAxQ6M4c1c9NwfrAAAAAAENAAAejhWkAOAxQ6M4c1c9NwfrAABbUZLJAAA=",
       "rank": 1,
       "summary": "Here is a summary of your events from last week",
       "resource": {
        "@odata.type": "#microsoft.graph.event",
        "end": {
         "dateTime": "2020-06-16T04:15:00Z",
         "timeZone": "UTC"
        },
        "hasAttachments": false,
        "iCalUId": "040000008200E00074C5B7101A82E008000000007093FDD79B3AD60100000000000000001000000036DAA2262EB4E04DA27DA77985FB8251",
        "isAllDay": false,
        "sensitivity": "Normal",
        "start": {
         "dateTime": "2020-06-16T03:30:00Z",
         "timeZone": "UTC"
        },
        "subject": "Weekly digest: Microsoft 365 changes",
        "type": "Single"
       }
      }
     ],
     "total": 1,
     "moreResultsAvailable": false
    }
   ]
  }
 ]
}
```

## <a name="known-limitations"></a><span data-ttu-id="c7357-110">Известные ограничения</span><span class="sxs-lookup"><span data-stu-id="c7357-110">Known limitations</span></span>

- <span data-ttu-id="c7357-111">Доступ к почтовому ящику вошедшего пользователя можно получить только из собственного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="c7357-111">You can access only the signed-in user’s own mailbox.</span></span> <span data-ttu-id="c7357-112">Поиск делегированных почтовых ящиков не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7357-112">Searching delegated mailboxes is not supported.</span></span>
- <span data-ttu-id="c7357-113">Для событий свойство **Total** объекта [сеарчхитсконтаинер](/graph/api/resources/searchhitscontainer?view=graph-rest-beta&preserve-view=true) содержит количество результатов на странице, а не общее количество результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="c7357-113">For events, the **total** property of the [searchHitsContainer](/graph/api/resources/searchhitscontainer?view=graph-rest-beta&preserve-view=true) type contains the number of results on the page, not the total number of matching results.</span></span>
- <span data-ttu-id="c7357-114">Сортировка результатов не поддерживается для событий.</span><span class="sxs-lookup"><span data-stu-id="c7357-114">Sorting results is not supported for events.</span></span> <span data-ttu-id="c7357-115">Предложение Sort в запросе возвратит код ошибки ошибочного запроса в ответе.</span><span class="sxs-lookup"><span data-stu-id="c7357-115">A sort clause in the request will return a Bad Request error code in the response.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c7357-116">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="c7357-116">Next steps</span></span>

- [<span data-ttu-id="c7357-117">Использование API Поиска (Майкрософт) для запроса данных</span><span class="sxs-lookup"><span data-stu-id="c7357-117">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
