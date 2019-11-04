---
title: Поиск событий календаря
description: Вы можете выполнять поиск в собственном календаре пользователя.
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 1b749c0b45b8250d011589e20b05a3d715b40bcb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939560"
---
# <a name="search-calendar-events"></a>Поиск событий календаря

Приложение может находиться в собственном основном календаре пользователя. Удостоверение пользователя, используемое для поиска, основано на маркере авторизации.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

В этом примере выполняется поиск по ключевому слову "contoso" в календаре пользователя, а также загружается до 25 результатов.

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
       "entityTypes": ["microsoft.graph.event"],
       "query": {
        "query_string": {
          "query": "contoso"
        }
      },
      "from": 0,
      "size": 25
    }
  ]
}
```

## <a name="known-limitations"></a>Известные ограничения

Можно получить доступ к собственному календарю пользователя. Общий календарь, делегированный доступ не поддерживается.

## <a name="next-steps"></a>Дальнейшие действия

Дополнительные сведения:

- [Использование API поиска](/graph/api/resources/search-api-overview?view=graph-rest-beta)