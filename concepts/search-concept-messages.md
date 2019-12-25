---
title: Использование API службы поиска Microsoft в Microsoft Graph для поиска сообщений
description: Вы можете использовать API Microsoft Search API для поиска информации в сообщениях электронной почты, получения сообщений, упорядоченных по релевантности, и отображения выделенного интерфейса поиска.
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: e57cbed67c3c224c26779b3c98e400c0411937ee
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868557"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-search-messages"></a><span data-ttu-id="867c9-103">Использование API службы поиска Microsoft в Microsoft Graph для поиска сообщений</span><span class="sxs-lookup"><span data-stu-id="867c9-103">Use the Microsoft Search API in Microsoft Graph to search messages</span></span>

<span data-ttu-id="867c9-104">Вы можете использовать API Microsoft Search API для поиска информации в сообщениях электронной почты, получения сообщений, упорядоченных по релевантности, и отображения выделенного интерфейса поиска.</span><span class="sxs-lookup"><span data-stu-id="867c9-104">You can use the Microsoft Search API to search for information in email messages, return messages ranked by relevance, and render a dedicated search experience.</span></span> <span data-ttu-id="867c9-105">Поиск применяется к тексту и вложениям сообщений в собственном почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="867c9-105">The search applies to the body and attachments of messages in the user's own mailbox.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<span data-ttu-id="867c9-106">Поисковый запрос может включать в себя [фильтры](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da) , вводимые пользователями в текстовое поле **поиска** в Outlook.</span><span class="sxs-lookup"><span data-stu-id="867c9-106">A search query can include [filters](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da) that end users enter in the **Search** text box in Outlook.</span></span>

<span data-ttu-id="867c9-107">Результаты поиска сообщений сортируются по **receivedDateTime** в порядке убывания.</span><span class="sxs-lookup"><span data-stu-id="867c9-107">Message search results are sorted by **receivedDateTime** in descending order.</span></span>

<span data-ttu-id="867c9-108">Поиск сообщений применяется к рабочим или учебным учетным записям.</span><span class="sxs-lookup"><span data-stu-id="867c9-108">Message search applies to work or school accounts.</span></span> <span data-ttu-id="867c9-109">Пользователи могут выполнять поиск в своем почтовом ящике, но не могут искать делегированные почтовые ящики.</span><span class="sxs-lookup"><span data-stu-id="867c9-109">Users can search their own mailbox, but can't search delegated mailboxes.</span></span> <span data-ttu-id="867c9-110">Подробнее: [Известные ограничения](#known-limitations).</span><span class="sxs-lookup"><span data-stu-id="867c9-110">For details, see [known limitations](#known-limitations).</span></span>

<span data-ttu-id="867c9-111">При поиске сообщений также выполняется поиск вложений.</span><span class="sxs-lookup"><span data-stu-id="867c9-111">Message search also looks for attachments.</span></span> <span data-ttu-id="867c9-112">[Поддерживаются такие же типы файлов](https://docs.microsoft.com/SharePoint/technical-reference/default-crawled-file-name-extensions-and-parsed-file-types) , что и для поиска в SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="867c9-112">The [supported file types](https://docs.microsoft.com/SharePoint/technical-reference/default-crawled-file-name-extensions-and-parsed-file-types) for message attachment search are the same as those for SharePoint Online search.</span></span>

## <a name="examples"></a><span data-ttu-id="867c9-113">Примеры</span><span class="sxs-lookup"><span data-stu-id="867c9-113">Examples</span></span>

### <a name="example-1-search-messages-in-a-users-mailbox"></a><span data-ttu-id="867c9-114">Пример 1: Поиск сообщений в почтовом ящике пользователя</span><span class="sxs-lookup"><span data-stu-id="867c9-114">Example 1: Search messages in a user's mailbox</span></span>

<span data-ttu-id="867c9-115">В следующем примере выполняется запрос сообщений в почтовом ящике вошедшего пользователя, который содержит строку "contoso" в любой части сообщения (имя отправителя, тема, текст сообщения или вложения).</span><span class="sxs-lookup"><span data-stu-id="867c9-115">The following example queries messages in the signed-in user's mailbox that contain the string "contoso" in any part of the message (the sender name, subject, message body, or any attachments).</span></span> <span data-ttu-id="867c9-116">Запрос возвращает первые 25 результатов.</span><span class="sxs-lookup"><span data-stu-id="867c9-116">The query returns the first 25 results.</span></span> <span data-ttu-id="867c9-117">Результаты поиска упорядочиваются по убыванию **даты и времени** .</span><span class="sxs-lookup"><span data-stu-id="867c9-117">The search results are ordered by **DateTime** descending.</span></span>

#### <a name="request"></a><span data-ttu-id="867c9-118">Запрос</span><span class="sxs-lookup"><span data-stu-id="867c9-118">Request</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "entityTypes": [
        "microsoft.graph.message"
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

#### <a name="response"></a><span data-ttu-id="867c9-119">Ответ</span><span class="sxs-lookup"><span data-stu-id="867c9-119">Response</span></span>

<span data-ttu-id="867c9-120">Ниже приведен пример ответа, содержащего одно сообщение, которое соответствует заданному критерию поиска.</span><span class="sxs-lookup"><span data-stu-id="867c9-120">The following is an example of the response, which contains one message that matches the search criterion.</span></span> 

```json
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#search",
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
              "_id": "ptWLQ4o6HYpQg8xmAAATzOzRAAA=",
              "_score": 1,
              "_sortField": "DateTime",
              "_summary": "Here is a summary of your messages from last week",
              "_source": {
                "@odata.type": "#microsoft.graph.message",
                "createdDateTime": "2019-10-07T10:00:08Z",
                "lastModifiedDateTime": "2019-10-07T10:00:11Z",
                "receivedDateTime": "2019-10-07T10:00:09Z",
                "sentDateTime": "2019-10-07T09:59:52Z",
                "hasAttachments": false,
                "subject": "Weekly digest: Office 365 changes",
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

### <a name="example-2-search-top-results-messages"></a><span data-ttu-id="867c9-121">Пример 2: Поиск в сообщениях с наибольшим результатом</span><span class="sxs-lookup"><span data-stu-id="867c9-121">Example 2: Search top results messages</span></span>
<span data-ttu-id="867c9-122">В следующем примере используется поисковый запрос, показанный в [примере 1](#example-1), и отсортирует результаты по релевантности.</span><span class="sxs-lookup"><span data-stu-id="867c9-122">The following example uses the search query shown in [Example 1](#example-1), and sorts the results by relevance.</span></span> 

<!-- markdownlint-disable MD024 -->
#### <a name="request"></a><span data-ttu-id="867c9-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="867c9-123">Request</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "entityTypes": [
        "microsoft.graph.message"
      ],
      "query": {
        "query_string": {
          "query": "contoso"
        }
      },
      "from": 0,
      "size": 15,
      "enableTopResults": true
    }
  ]
}
```

## <a name="known-limitations"></a><span data-ttu-id="867c9-124">Известные ограничения</span><span class="sxs-lookup"><span data-stu-id="867c9-124">Known limitations</span></span>

- <span data-ttu-id="867c9-125">Доступ к почтовому ящику пользователя можно получить только.</span><span class="sxs-lookup"><span data-stu-id="867c9-125">You can only access a user’s own mailbox.</span></span> <span data-ttu-id="867c9-126">Поиск делегированных почтовых ящиков не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="867c9-126">Searching delegated mailboxes is not supported.</span></span>
- <span data-ttu-id="867c9-127">Для сообщений свойство **Total** объекта [сеарчхитсконтаинер](/graph/api/resources/searchhitscontainer?view=graph-rest-beta) содержит количество результатов на странице, а не общее число результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="867c9-127">For messages, the **total** property of the [searchHitsContainer](/graph/api/resources/searchhitscontainer?view=graph-rest-beta) type contains the number of results on the page, not the total number of matching results.</span></span>

## <a name="next-steps"></a><span data-ttu-id="867c9-128">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="867c9-128">Next steps</span></span>

- [<span data-ttu-id="867c9-129">Использование API службы поиска Microsoft</span><span class="sxs-lookup"><span data-stu-id="867c9-129">Use the Microsoft Search API</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)
