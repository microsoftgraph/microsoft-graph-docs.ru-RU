---
title: Использование API службы поиска Microsoft в Microsoft Graph для поиска событий календаря
description: Вы можете выполнять поиск в собственном календаре пользователя.
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 6326fead96cd0b777ff6c3e257d6aa36d4d5c4ce
ms.sourcegitcommit: 093d89c7583bb6880c8395e9498a1f33cdd938b4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2020
ms.locfileid: "44568783"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-search-calendar-events"></a><span data-ttu-id="d0dd5-103">Использование API службы поиска Microsoft в Microsoft Graph для поиска событий календаря</span><span class="sxs-lookup"><span data-stu-id="d0dd5-103">Use the Microsoft Search API in Microsoft Graph to search calendar events</span></span>

<span data-ttu-id="d0dd5-104">С помощью API поиска Microsoft можно искать события в основном календаре пользователя.</span><span class="sxs-lookup"><span data-stu-id="d0dd5-104">You can use the Microsoft Search API to search for events in a user’s primary calendar.</span></span> <span data-ttu-id="d0dd5-105">Удостоверение пользователя для поиска основано на маркере проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="d0dd5-105">The user identity for the search is based on the auth token.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

## <a name="example"></a><span data-ttu-id="d0dd5-106">Пример</span><span class="sxs-lookup"><span data-stu-id="d0dd5-106">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0dd5-107">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0dd5-107">Request</span></span>

<span data-ttu-id="d0dd5-108">В этом примере выполняется поиск ключевого слова "contoso" в календаре пользователя и возвращается до 25 результатов.</span><span class="sxs-lookup"><span data-stu-id="d0dd5-108">This example searches in the user's calendar for the keyword "contoso", and will return up to 25 results.</span></span>

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

## <a name="known-limitations"></a><span data-ttu-id="d0dd5-109">Известные ограничения</span><span class="sxs-lookup"><span data-stu-id="d0dd5-109">Known limitations</span></span>

<span data-ttu-id="d0dd5-110">Можно получить доступ к собственному календарю пользователя.</span><span class="sxs-lookup"><span data-stu-id="d0dd5-110">You can only access user’s own calendar.</span></span> <span data-ttu-id="d0dd5-111">Общий календарь и делегированный сченариос доступа не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="d0dd5-111">Shared calendar and delegated access schenarios are not supported.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d0dd5-112">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="d0dd5-112">Next steps</span></span>

- [<span data-ttu-id="d0dd5-113">Использование API Поиска (Майкрософт) для запроса данных</span><span class="sxs-lookup"><span data-stu-id="d0dd5-113">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)
