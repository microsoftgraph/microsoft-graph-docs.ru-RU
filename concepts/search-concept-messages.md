---
title: Поиск сообщений
description: API Microsoft Search позволяет приложениям искать информацию в сообщениях электронной почты, получать сообщения, Ранжированные по релевантности, и отображать выделенный интерфейс для поиска.
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: f78ad8af81a7d2b72ab61914cc441db279913dc1
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939546"
---
# <a name="search-messages"></a><span data-ttu-id="b9231-103">Поиск сообщений</span><span class="sxs-lookup"><span data-stu-id="b9231-103">Search messages</span></span>

<span data-ttu-id="b9231-104">API Microsoft Search позволяет приложениям искать информацию в сообщениях электронной почты, получать сообщения, Ранжированные по релевантности, и отображать выделенный интерфейс для поиска.</span><span class="sxs-lookup"><span data-stu-id="b9231-104">The Microsoft Search API lets apps search for information in email messages, return messages ranked by relevance, and render a dedicated search experience.</span></span> <span data-ttu-id="b9231-105">Поиск применяется к тексту и вложениям сообщений в собственном почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="b9231-105">The search applies to the body and attachments of messages in the user's own mailbox.</span></span> 

<span data-ttu-id="b9231-106">Поисковый запрос может включать в себя [фильтры](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da) , вводимые пользователями в текстовое поле **поиска** в Outlook.</span><span class="sxs-lookup"><span data-stu-id="b9231-106">A search query can include [filters](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da) that end users enter in the **Search** text box in Outlook.</span></span>

<span data-ttu-id="b9231-107">Результаты поиска сообщений сортируются по **receivedDateTime** в порядке убывания.</span><span class="sxs-lookup"><span data-stu-id="b9231-107">Message search results are sorted by **receivedDateTime** in descending order.</span></span>

<span data-ttu-id="b9231-108">В настоящее время поиск сообщений применяется только к собственным личным учетным записям пользователей, но не к рабочим или учебным учетным записям, а не к делегированным почтовым ящикам.</span><span class="sxs-lookup"><span data-stu-id="b9231-108">Currently, message search applies to only users' own personal accounts, but not work or school accounts, and not in delegated mailboxes.</span></span> <span data-ttu-id="b9231-109">Ниже приводятся более [Известные ограничения](#known-limitations) .</span><span class="sxs-lookup"><span data-stu-id="b9231-109">See further [known limitations](#known-limitations) below.</span></span>

## <a name="examples"></a><span data-ttu-id="b9231-110">Примеры</span><span class="sxs-lookup"><span data-stu-id="b9231-110">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="b9231-111">Пример 1</span><span class="sxs-lookup"><span data-stu-id="b9231-111">Example 1</span></span>

<span data-ttu-id="b9231-112">В следующем примере выполняется запрос сообщений в почтовом ящике вошедшего пользователя, который содержит строку "contoso" в любой части сообщения (имя отправителя, тема, текст сообщения или вложения).</span><span class="sxs-lookup"><span data-stu-id="b9231-112">The following example queries messages in the signed-in user's mailbox that contain the string "contoso" in any part of the message (the sender name, subject, message body, or any attachments).</span></span> <span data-ttu-id="b9231-113">Запрос возвращает первые 25 результатов.</span><span class="sxs-lookup"><span data-stu-id="b9231-113">The query returns the first 25 results.</span></span> <span data-ttu-id="b9231-114">Результаты поиска упорядочиваются по убыванию даты и времени.</span><span class="sxs-lookup"><span data-stu-id="b9231-114">The search results are ordered by Datetime descending.</span></span>

#### <a name="request"></a><span data-ttu-id="b9231-115">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9231-115">Request</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
  "requests": [{
      "entityTypes": ["microsoft.graph.message"],
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

#### <a name="response"></a><span data-ttu-id="b9231-116">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9231-116">Response</span></span> 

<span data-ttu-id="b9231-117">Ниже приведен пример ответа, содержащего одно сообщение, которое соответствует заданному критерию поиска.</span><span class="sxs-lookup"><span data-stu-id="b9231-117">The following is an example of the response which contains one message that matches the search criterion.</span></span> 

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#search",
    "value": [
        {
            "searchTerms": [
                "contoso"
            ],
            "hitsContainers": [
                {
                    "total": 1,
                    "moreResultsAvailable": false,
                    "hits": [
                        {
                            "_id": "ptWLQ4o6HYpQg8xmAAATzOzRAAA=",
                            "_score": 1,
                            "_sortField": "DateTime",
                            "_summary": "Here is a summary of your messages from last week",
                            "_source": {
                                "@odata.type": "#microsoft.graph.message",
                                "createdDateTime": "2019-10-07T10:00:08Z",
                                "lastModifiedDateTime": "2019-10-07T10:00:11Z",
                                "receivedDateTime": "2019-10-07T10:00:09Z",
                                "sentDateTime": "2019-10-07T09:59:52Z",
                                "hasAttachments": false,
                                "subject": "Weekly digest: Office 365 changes",
                                "bodyPreview": "Here is a summary of your messages from last week -   New Feature: Live captions in English-US a",
                                "importance": "normal",
                                "replyTo": [
                                    {
                                        "emailAddress": {
                                            "name": "Goncalo Torres"
                                        }
                                    }
                                ],
                                "sender": {
                                    "emailAddress": {
                                        "name": "Office365 Message Center",
                                        "address": "gtorres@contoso.com"
                                    }
                                },
                                "from": {
                                    "emailAddress": {
                                        "name": "Office365 Message Center",
                                        "address": "gtorres@contoso.com",
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

### <a name="example-2-search-top-results-messages"></a><span data-ttu-id="b9231-118">Пример 2. сообщения о главных результатах поиска</span><span class="sxs-lookup"><span data-stu-id="b9231-118">Example 2 Search top results messages</span></span>
<span data-ttu-id="b9231-119">В следующем примере используется тот же поисковый запрос, что и в [примере 1](#example-1), а результаты сортируются по релевантности.</span><span class="sxs-lookup"><span data-stu-id="b9231-119">The following example uses the same search query as [example 1](#example-1), and sorts the results by relevance.</span></span> 

#### <a name="request"></a><span data-ttu-id="b9231-120">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9231-120">Request</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
    "requests": [{
        "entityTypes": ["microsoft.graph.message"],
        "query": {
            "query_string": {
                "query": "contoso"
            }
        },
        "from": 0,
        "size": 15,
        "enableTopResults": true
    }]
}
```

## <a name="known-limitations"></a><span data-ttu-id="b9231-121">Известные ограничения</span><span class="sxs-lookup"><span data-stu-id="b9231-121">Known limitations</span></span>

- <span data-ttu-id="b9231-122">Доступ к почтовому ящику пользователя можно получить только.</span><span class="sxs-lookup"><span data-stu-id="b9231-122">You can only access a user’s own mailbox.</span></span> <span data-ttu-id="b9231-123">Поиск делегированного почтового ящика не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b9231-123">Searching delegated mailbox is not supported</span></span> 

- <span data-ttu-id="b9231-124">Для сообщений свойство **Total** объекта [сеарчхитсконтаинер](/graph/api/resources/searchhitscontainer?view=graph-rest-beta) содержит количество результатов на странице, а не общее число результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="b9231-124">For messages, the **total** property of the [searchHitsContainer](/graph/api/resources/searchhitscontainer?view=graph-rest-beta) type contains the number of results on the page, not the total number of matching results.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b9231-125">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="b9231-125">Next steps</span></span>

<span data-ttu-id="b9231-126">Дополнительные сведения:</span><span class="sxs-lookup"><span data-stu-id="b9231-126">Find out more about:</span></span>

- [<span data-ttu-id="b9231-127">Использование API поиска</span><span class="sxs-lookup"><span data-stu-id="b9231-127">Use the search API</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)
