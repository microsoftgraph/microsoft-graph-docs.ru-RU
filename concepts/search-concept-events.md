---
title: Использование API поиска (Майкрософт) для поиска событий календаря Outlook
description: Используйте API поиска (Майкрософт) в Microsoft Graph для поиска событий в основном календаре вошедвшего пользователя. Удостоверение пользователя основано на маркере проверки подлинности.
author: knightsu
ms.localizationpriority: medium
ms.prod: search
ms.openlocfilehash: 3c5956efa60a54cd4f0cfaae6dcf5f56ddb85dc7
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66445862"
---
# <a name="use-the-microsoft-search-api-to-search-outlook-calendar-events"></a>Использование API поиска (Майкрософт) для поиска событий календаря Outlook

Используйте API поиска (Майкрософт) в Microsoft Graph для поиска событий в основном календаре вошедвшего пользователя. Удостоверение пользователя для поиска основано на маркере проверки подлинности.

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

В этом примере выполняется поиск ключевого слова contoso в календаре пользователя и возвращается до 25 результатов.

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

### <a name="response"></a>Отклик

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

- Вы можете получить доступ только к собственному почтовому ящику пользователя, выполнившего вход. Поиск в делегированных почтовых ящиках не поддерживается.
- Для событий общее свойство  типа [searchHitsContainer](/graph/api/resources/searchhitscontainer) содержит количество результатов на странице, а не общее число соответствующих результатов.
- Сортировка результатов не поддерживается для событий. Предложение сортировки в запросе возвращает код ошибки "Недопустимый запрос" в ответе.

## <a name="next-steps"></a>Дальнейшие действия

- [Использование API Поиска (Майкрософт) для запроса данных](/graph/api/resources/search-api-overview)
