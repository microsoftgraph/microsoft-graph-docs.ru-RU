---
title: Поиск событий календаря
description: Вы можете выполнять поиск в собственном календаре пользователя.
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 2db61462670a553376467cf2329d26cbb339c452
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703976"
---
# <a name="search-calendar-events"></a>Поиск событий календаря

Приложение может находиться в собственном основном календаре пользователя. Удостоверение пользователя, используемое для поиска, основано на маркере авторизации.

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

В этом примере выполняется поиск по ключевому слову "contoso" в календаре пользователя, а также загружается до 25 результатов.

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "entityTypes": [
        "microsoft.graph.event"
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

Можно получить доступ к собственному календарю пользователя. Общий календарь, делегированный доступ не поддерживается.

## <a name="next-steps"></a>Дальнейшие действия

Дополнительные сведения:

- [Использование API поиска](/graph/api/resources/search-api-overview?view=graph-rest-beta)
