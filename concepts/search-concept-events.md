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
# <a name="use-the-microsoft-search-api-to-search-calendar-events"></a>Использование API службы поиска Microsoft для поиска событий календаря

Используйте API службы поиска Microsoft для поиска событий в основном календаре вошедшего пользователя. Удостоверение пользователя для поиска основано на маркере проверки подлинности.

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

В этом примере выполняется поиск ключевого слова "contoso" в календаре пользователя и возвращается до 25 результатов.

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

#### <a name="response"></a>Отклик

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

## <a name="known-limitations"></a>Известные ограничения

- Доступ к почтовому ящику вошедшего пользователя можно получить только из собственного почтового ящика. Поиск делегированных почтовых ящиков не поддерживается.
- Для событий свойство **Total** объекта [сеарчхитсконтаинер](/graph/api/resources/searchhitscontainer?view=graph-rest-beta&preserve-view=true) содержит количество результатов на странице, а не общее количество результатов поиска.
- Сортировка результатов не поддерживается для событий. Предложение Sort в запросе возвратит код ошибки ошибочного запроса в ответе.

## <a name="next-steps"></a>Дальнейшие действия

- [Использование API Поиска (Майкрософт) для запроса данных](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
