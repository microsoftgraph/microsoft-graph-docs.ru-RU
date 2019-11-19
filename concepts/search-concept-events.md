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
# <a name="search-calendar-events"></a><span data-ttu-id="62de3-103">Поиск событий календаря</span><span class="sxs-lookup"><span data-stu-id="62de3-103">Search calendar events</span></span>

<span data-ttu-id="62de3-104">Приложение может находиться в собственном основном календаре пользователя.</span><span class="sxs-lookup"><span data-stu-id="62de3-104">You app can in a user’s own primary calendar.</span></span> <span data-ttu-id="62de3-105">Удостоверение пользователя, используемое для поиска, основано на маркере авторизации.</span><span class="sxs-lookup"><span data-stu-id="62de3-105">The user identity used to search is based on the Authorization Token.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

## <a name="example"></a><span data-ttu-id="62de3-106">Пример</span><span class="sxs-lookup"><span data-stu-id="62de3-106">Example</span></span>

### <a name="request"></a><span data-ttu-id="62de3-107">Запрос</span><span class="sxs-lookup"><span data-stu-id="62de3-107">Request</span></span>

<span data-ttu-id="62de3-108">В этом примере выполняется поиск по ключевому слову "contoso" в календаре пользователя, а также загружается до 25 результатов.</span><span class="sxs-lookup"><span data-stu-id="62de3-108">This example searches in the user's calendar for the keyword "contoso", and will retrieve up to 25 results.</span></span>

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

## <a name="known-limitations"></a><span data-ttu-id="62de3-109">Известные ограничения</span><span class="sxs-lookup"><span data-stu-id="62de3-109">Known limitations</span></span>

<span data-ttu-id="62de3-110">Можно получить доступ к собственному календарю пользователя.</span><span class="sxs-lookup"><span data-stu-id="62de3-110">You can only access user’s own calendar.</span></span> <span data-ttu-id="62de3-111">Общий календарь, делегированный доступ не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62de3-111">Shared Calendar, delegated access is not supported.</span></span>

## <a name="next-steps"></a><span data-ttu-id="62de3-112">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="62de3-112">Next steps</span></span>

<span data-ttu-id="62de3-113">Дополнительные сведения:</span><span class="sxs-lookup"><span data-stu-id="62de3-113">Find out more about:</span></span>

- [<span data-ttu-id="62de3-114">Использование API поиска</span><span class="sxs-lookup"><span data-stu-id="62de3-114">Use the search API</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)
