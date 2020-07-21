---
title: Использование API службы поиска Microsoft в Microsoft Graph для поиска событий календаря
description: Вы можете выполнять поиск в собственном календаре пользователя.
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 8cafb01337581d1b1d2e355363aec14f658ee4f6
ms.sourcegitcommit: 79267b6d78c3510ef609953c5a664e692794caaa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/21/2020
ms.locfileid: "45196829"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-search-calendar-events"></a>Использование API службы поиска Microsoft в Microsoft Graph для поиска событий календаря

С помощью API поиска Microsoft можно искать события в основном календаре пользователя. Удостоверение пользователя для поиска основано на маркере проверки подлинности.

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

В этом примере выполняется поиск ключевого слова "contoso" в календаре пользователя и возвращается до 25 результатов.

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "entityTypes": [
        "event"
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

## <a name="known-limitations"></a>Известные ограничения

Можно получить доступ к собственному календарю пользователя. Сценарии общего календаря и делегированного доступа не поддерживаются.

## <a name="next-steps"></a>Дальнейшие действия

- [Использование API Поиска (Майкрософт) для запроса данных](/graph/api/resources/search-api-overview?view=graph-rest-beta)
