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
# <a name="search-calendar-events"></a><span data-ttu-id="65ed0-103">Поиск событий календаря</span><span class="sxs-lookup"><span data-stu-id="65ed0-103">Search calendar events</span></span>

<span data-ttu-id="65ed0-104">Приложение может находиться в собственном основном календаре пользователя.</span><span class="sxs-lookup"><span data-stu-id="65ed0-104">You app can in a user’s own primary calendar.</span></span> <span data-ttu-id="65ed0-105">Удостоверение пользователя, используемое для поиска, основано на маркере авторизации.</span><span class="sxs-lookup"><span data-stu-id="65ed0-105">The user identity used to search is based on the Authorization Token.</span></span>

## <a name="example"></a><span data-ttu-id="65ed0-106">Пример</span><span class="sxs-lookup"><span data-stu-id="65ed0-106">Example</span></span>

### <a name="request"></a><span data-ttu-id="65ed0-107">Запрос</span><span class="sxs-lookup"><span data-stu-id="65ed0-107">Request</span></span>

<span data-ttu-id="65ed0-108">В этом примере выполняется поиск по ключевому слову "contoso" в календаре пользователя, а также загружается до 25 результатов.</span><span class="sxs-lookup"><span data-stu-id="65ed0-108">This example searches in the user's calendar for the keyword "contoso", and will retrieve up to 25 results.</span></span>

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

## <a name="known-limitations"></a><span data-ttu-id="65ed0-109">Известные ограничения</span><span class="sxs-lookup"><span data-stu-id="65ed0-109">Known limitations</span></span>

<span data-ttu-id="65ed0-110">Можно получить доступ к собственному календарю пользователя.</span><span class="sxs-lookup"><span data-stu-id="65ed0-110">You can only access user’s own calendar.</span></span> <span data-ttu-id="65ed0-111">Общий календарь, делегированный доступ не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65ed0-111">Shared Calendar, delegated access is not supported.</span></span>

## <a name="next-steps"></a><span data-ttu-id="65ed0-112">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="65ed0-112">Next steps</span></span>

<span data-ttu-id="65ed0-113">Дополнительные сведения:</span><span class="sxs-lookup"><span data-stu-id="65ed0-113">Find out more about:</span></span>

- [<span data-ttu-id="65ed0-114">Использование API поиска</span><span class="sxs-lookup"><span data-stu-id="65ed0-114">Use the search API</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)