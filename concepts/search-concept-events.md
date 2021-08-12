---
title: Используйте API Поиск (Майкрософт) в Microsoft Graph для поиска событий календаря
description: Вы можете искать в собственном календаре пользователя.
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 277c46e6298aa532d300b23fcba707c678e38e035007d2ef63fa249951afa633
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54171975"
---
# <a name="use-the-microsoft-search-api-to-search-calendar-events"></a>Используйте API Поиск (Майкрософт) для поиска событий календаря

Используйте API Поиск (Майкрософт) для поиска событий в основном календаре пользователя. Идентификатор пользователя для поиска основан на маркере auth.

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

В этом примере в календаре пользователя выполняется поиск по ключевому слову "contoso" и возвращается до 25 результатов.

```HTTP
POST https://graph.microsoft.com/v1.0/search/query
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#search",
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

- Вы можете получить доступ только к собственному почтовому ящику пользователя. Поиск делегирования почтовых ящиков не поддерживается.
- Для событий **общее** свойство [типа searchHitsContainer](/graph/api/resources/searchhitscontainer) содержит количество результатов на странице, а не общее число совпадающих результатов.
- Результаты сортировки не поддерживаются для событий. Сортивная оговорка в запросе возвращает код ошибки "Плохой запрос" в ответе.

## <a name="next-steps"></a>Дальнейшие действия

- [Использование API Поиска (Майкрософт) для запроса данных](/graph/api/resources/search-api-overview)
