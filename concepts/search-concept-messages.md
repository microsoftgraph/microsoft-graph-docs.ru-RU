---
title: Использование API службы поиска Microsoft в Microsoft Graph для поиска сообщений
description: Вы можете использовать API Microsoft Search API для поиска информации в сообщениях электронной почты, получения сообщений, упорядоченных по релевантности, и отображения выделенного интерфейса поиска.
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 0ee9950ff136b3f97e063da252ec22d166f05b74
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49521364"
---
# <a name="use-the-microsoft-search-api-to-search-outlook-messages"></a><span data-ttu-id="463dd-103">Использование API службы поиска Microsoft для поиска сообщений Outlook</span><span class="sxs-lookup"><span data-stu-id="463dd-103">Use the Microsoft Search API to search Outlook messages</span></span>

<span data-ttu-id="463dd-104">Используйте API Microsoft Search API для поиска информации в сообщениях электронной почты, получения сообщений, упорядоченных по релевантности, и отображения выделенного интерфейса поиска.</span><span class="sxs-lookup"><span data-stu-id="463dd-104">Use the Microsoft Search API to search for information in email messages, return messages ranked by relevance, and render a dedicated search experience.</span></span> <span data-ttu-id="463dd-105">Поиск применяется к основному тексту и вложениям сообщений в собственном почтовом ящике вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="463dd-105">The search applies to the body and attachments of messages in the signed-in user's own mailbox.</span></span>

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

<span data-ttu-id="463dd-106">Поисковый запрос может включать в себя [фильтры](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da) , вводимые пользователями в текстовое поле **поиска** в Outlook.</span><span class="sxs-lookup"><span data-stu-id="463dd-106">A search query can include [filters](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da) that end users enter in the **Search** text box in Outlook.</span></span>

<span data-ttu-id="463dd-107">Результаты поиска сообщений сортируются по **receivedDateTime** в порядке убывания.</span><span class="sxs-lookup"><span data-stu-id="463dd-107">Message search results are sorted by **receivedDateTime** in descending order.</span></span>

<span data-ttu-id="463dd-108">Поиск сообщений применяется к рабочим или учебным учетным записям.</span><span class="sxs-lookup"><span data-stu-id="463dd-108">Message search applies to work or school accounts.</span></span> <span data-ttu-id="463dd-109">Пользователи могут выполнять поиск в своем почтовом ящике, но не могут искать делегированные почтовые ящики.</span><span class="sxs-lookup"><span data-stu-id="463dd-109">Users can search their own mailbox, but can't search delegated mailboxes.</span></span> <span data-ttu-id="463dd-110">Подробнее: [Известные ограничения](#known-limitations).</span><span class="sxs-lookup"><span data-stu-id="463dd-110">For details, see [known limitations](#known-limitations).</span></span>

<span data-ttu-id="463dd-111">При поиске сообщений также выполняется поиск вложений.</span><span class="sxs-lookup"><span data-stu-id="463dd-111">Message search also looks for attachments.</span></span> <span data-ttu-id="463dd-112">[Поддерживаются такие же типы файлов](/SharePoint/technical-reference/default-crawled-file-name-extensions-and-parsed-file-types) , что и для поиска в SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="463dd-112">The [supported file types](/SharePoint/technical-reference/default-crawled-file-name-extensions-and-parsed-file-types) for message attachment search are the same as those for SharePoint Online search.</span></span>

## <a name="example-1-search-messages-in-a-users-mailbox"></a><span data-ttu-id="463dd-113">Пример 1: Поиск сообщений в почтовом ящике пользователя</span><span class="sxs-lookup"><span data-stu-id="463dd-113">Example 1: Search messages in a user's mailbox</span></span>

<span data-ttu-id="463dd-114">В следующем примере выполняется запрос сообщений в почтовом ящике вошедшего пользователя, который содержит строку "contoso" в любой части сообщения (имя отправителя, тема, текст сообщения или вложения).</span><span class="sxs-lookup"><span data-stu-id="463dd-114">The following example queries messages in the signed-in user's mailbox that contain the string "contoso" in any part of the message (the sender name, subject, message body, or any attachments).</span></span> <span data-ttu-id="463dd-115">Запрос возвращает первые 25 результатов.</span><span class="sxs-lookup"><span data-stu-id="463dd-115">The query returns the first 25 results.</span></span> <span data-ttu-id="463dd-116">Результаты поиска упорядочиваются по убыванию **даты и времени** .</span><span class="sxs-lookup"><span data-stu-id="463dd-116">The search results are ordered by **DateTime** descending.</span></span>

### <a name="request"></a><span data-ttu-id="463dd-117">Запрос</span><span class="sxs-lookup"><span data-stu-id="463dd-117">Request</span></span>

```HTTP
POST https://graph.microsoft.com/v1.0/search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "message"
      ],
      "query": {
        "queryString": "contoso"
      },
      "from": 0,
      "size": 25
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="463dd-118">Отклик</span><span class="sxs-lookup"><span data-stu-id="463dd-118">Response</span></span>

<span data-ttu-id="463dd-119">Ниже приведен пример ответа, содержащего одно сообщение, которое соответствует заданному критерию поиска.</span><span class="sxs-lookup"><span data-stu-id="463dd-119">The following is an example of the response, which contains one message that matches the search criterion.</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#search",
  "value": [
    {
      "searchTerms": [
        "contoso"
      ],
      "hitsContainers": [
        {
          "total": 1,
          "moreResultsAvailable": false,
          "hits": [
            {
              "hitId": "ptWLQ4o6HYpQg8xmAAATzOzRAAA=",
              "rank": 1,
              "summary": "Here is a summary of your messages from last week",
              "resource": {
                "@odata.type": "#microsoft.graph.message",
                "createdDateTime": "2019-10-07T10:00:08Z",
                "lastModifiedDateTime": "2019-10-07T10:00:11Z",
                "receivedDateTime": "2019-10-07T10:00:09Z",
                "sentDateTime": "2019-10-07T09:59:52Z",
                "hasAttachments": false,
                "subject": "Weekly digest: Microsoft 365 changes",
                "bodyPreview": "Here is a summary of your messages from last week -   New Feature: Live captions in English-US a",
                "importance": "normal",
                "replyTo": [
                  {
                    "emailAddress": {
                      "name": "Goncalo Torres"
                    }
                  }
                ],
                "sender": {
                  "emailAddress": {
                    "name": "Office365 Message Center",
                    "address": "gtorres@contoso.com"
                  }
                },
                "from": {
                  "emailAddress": {
                    "name": "Office365 Message Center",
                    "address": "gtorres@contoso.com"
                  }
                }
              }
            }
          ]
        }
      ]
    }
  ]
}
```

## <a name="example-2-search-top-results-messages"></a><span data-ttu-id="463dd-120">Пример 2: Поиск в сообщениях с наибольшим результатом</span><span class="sxs-lookup"><span data-stu-id="463dd-120">Example 2: Search top results messages</span></span>

<span data-ttu-id="463dd-121">В следующем примере используется поисковый запрос, показанный в примере 1, и отсортирует результаты по релевантности.</span><span class="sxs-lookup"><span data-stu-id="463dd-121">The following example uses the search query shown in Example 1, and sorts the results by relevance.</span></span> 

<!-- markdownlint-disable MD024 -->
### <a name="request"></a><span data-ttu-id="463dd-122">Запрос</span><span class="sxs-lookup"><span data-stu-id="463dd-122">Request</span></span>

```HTTP
POST https://graph.microsoft.com/v1.0/search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "message"
      ],
      "query": {
        "queryString": "contoso"
      },
      "from": 0,
      "size": 15,
      "enableTopResults": true
    }
  ]
}
```

#### <a name="response"></a><span data-ttu-id="463dd-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="463dd-123">Response</span></span>
```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#search",
  "value": [
    {
      "searchTerms": [
        "contoso"
      ],
      "hitsContainers": [
        {
          "total": 1,
          "moreResultsAvailable": false,
          "hits": [
            {
              "hitId": "ptWLQ4o6HYpQg8xmAAATzOzRAAA=",
              "rank": 1,
              "summary": "Here is a summary of your messages from last week",
              "resource": {
                "@odata.type": "#microsoft.graph.message",
                "createdDateTime": "2019-10-07T10:00:08Z",
                "lastModifiedDateTime": "2019-10-07T10:00:11Z",
                "receivedDateTime": "2019-10-07T10:00:09Z",
                "sentDateTime": "2019-10-07T09:59:52Z",
                "hasAttachments": false,
                "subject": "Weekly digest: Microsoft 365 changes",
                "bodyPreview": "Here is a summary of your messages from last week -   New Feature: Live captions in English-US a",
                "importance": "normal",
                "replyTo": [
                  {
                    "emailAddress": {
                      "name": "Goncalo Torres"
                    }
                  }
                ],
                "sender": {
                  "emailAddress": {
                    "name": "Office365 Message Center",
                    "address": "gtorres@contoso.com"
                  }
                },
                "from": {
                  "emailAddress": {
                    "name": "Office365 Message Center",
                    "address": "gtorres@contoso.com"
                  }
                }
              }
            }
          ]
        }
      ]
    }
  ]
}
```

## <a name="known-limitations"></a><span data-ttu-id="463dd-124">Известные ограничения</span><span class="sxs-lookup"><span data-stu-id="463dd-124">Known limitations</span></span>

- <span data-ttu-id="463dd-125">Доступ к почтовому ящику вошедшего пользователя можно получить только из собственного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="463dd-125">You can access only the signed-in user’s own mailbox.</span></span> <span data-ttu-id="463dd-126">Поиск делегированных почтовых ящиков не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="463dd-126">Searching delegated mailboxes is not supported.</span></span>
- <span data-ttu-id="463dd-127">Для сообщений свойство **Total** объекта [сеарчхитсконтаинер](/graph/api/resources/searchhitscontainer) содержит количество результатов на странице, а не общее число результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="463dd-127">For messages, the **total** property of the [searchHitsContainer](/graph/api/resources/searchhitscontainer) type contains the number of results on the page, not the total number of matching results.</span></span>
- <span data-ttu-id="463dd-128">Сортировка результатов не поддерживается для событий.</span><span class="sxs-lookup"><span data-stu-id="463dd-128">Sorting results is not supported for events.</span></span> <span data-ttu-id="463dd-129">Предложение Sort в запросе возвратит код ошибки ошибочного запроса в ответе.</span><span class="sxs-lookup"><span data-stu-id="463dd-129">A sort clause in the request will return a Bad Request error code in the response.</span></span>

## <a name="next-steps"></a><span data-ttu-id="463dd-130">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="463dd-130">Next steps</span></span>

- [<span data-ttu-id="463dd-131">Использование API службы поиска Microsoft</span><span class="sxs-lookup"><span data-stu-id="463dd-131">Use the Microsoft Search API</span></span>](/graph/api/resources/search-api-overview)