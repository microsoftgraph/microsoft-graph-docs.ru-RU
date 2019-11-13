---
title: Поиск сообщений
description: API Microsoft Search позволяет приложениям искать информацию в сообщениях электронной почты, получать сообщения, Ранжированные по релевантности, и отображать выделенный интерфейс для поиска.
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 985da47e5a7b96cead416e8e5cda32dae0357adb
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/13/2019
ms.locfileid: "38303134"
---
# <a name="search-messages"></a><span data-ttu-id="9ba0f-103">Поиск сообщений</span><span class="sxs-lookup"><span data-stu-id="9ba0f-103">Search messages</span></span>

<span data-ttu-id="9ba0f-104">API Microsoft Search позволяет приложениям искать информацию в сообщениях электронной почты, получать сообщения, Ранжированные по релевантности, и отображать выделенный интерфейс для поиска.</span><span class="sxs-lookup"><span data-stu-id="9ba0f-104">The Microsoft Search API lets apps search for information in email messages, return messages ranked by relevance, and render a dedicated search experience.</span></span> <span data-ttu-id="9ba0f-105">Поиск применяется к тексту и вложениям сообщений в собственном почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="9ba0f-105">The search applies to the body and attachments of messages in the user's own mailbox.</span></span>

<span data-ttu-id="9ba0f-106">Поисковый запрос может включать в себя [фильтры](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da) , вводимые пользователями в текстовое поле **поиска** в Outlook.</span><span class="sxs-lookup"><span data-stu-id="9ba0f-106">A search query can include [filters](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da) that end users enter in the **Search** text box in Outlook.</span></span>

<span data-ttu-id="9ba0f-107">Результаты поиска сообщений сортируются по **receivedDateTime** в порядке убывания.</span><span class="sxs-lookup"><span data-stu-id="9ba0f-107">Message search results are sorted by **receivedDateTime** in descending order.</span></span>

<span data-ttu-id="9ba0f-108">Поиск сообщений применяется к рабочим или учебным учетным записям.</span><span class="sxs-lookup"><span data-stu-id="9ba0f-108">Message search applies to work or school accounts.</span></span> <span data-ttu-id="9ba0f-109">Пользователи могут выполнять поиск в собственном почтовом ящике, но не в делегированных почтовых ящиках.</span><span class="sxs-lookup"><span data-stu-id="9ba0f-109">Users can search their own mailbox, but not in delegated mailboxes.</span></span> <span data-ttu-id="9ba0f-110">Ниже приводятся более [Известные ограничения](#known-limitations) .</span><span class="sxs-lookup"><span data-stu-id="9ba0f-110">See further [known limitations](#known-limitations) below.</span></span>

<span data-ttu-id="9ba0f-111">При поиске сообщений также выполняется поиск вложений.</span><span class="sxs-lookup"><span data-stu-id="9ba0f-111">Message search also looks for attachments.</span></span> <span data-ttu-id="9ba0f-112">[Типы файлов, поддерживаемые для вложений](https://docs.microsoft.com/SharePoint/technical-reference/default-crawled-file-name-extensions-and-parsed-file-types) , одинаковы для SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="9ba0f-112">The [file types supported for attachments](https://docs.microsoft.com/SharePoint/technical-reference/default-crawled-file-name-extensions-and-parsed-file-types) is the same as that for SharePoint Online.</span></span>

## <a name="examples"></a><span data-ttu-id="9ba0f-113">Примеры</span><span class="sxs-lookup"><span data-stu-id="9ba0f-113">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="9ba0f-114">Пример 1</span><span class="sxs-lookup"><span data-stu-id="9ba0f-114">Example 1</span></span>

<span data-ttu-id="9ba0f-115">В следующем примере выполняется запрос сообщений в почтовом ящике вошедшего пользователя, который содержит строку "contoso" в любой части сообщения (имя отправителя, тема, текст сообщения или вложения).</span><span class="sxs-lookup"><span data-stu-id="9ba0f-115">The following example queries messages in the signed-in user's mailbox that contain the string "contoso" in any part of the message (the sender name, subject, message body, or any attachments).</span></span> <span data-ttu-id="9ba0f-116">Запрос возвращает первые 25 результатов.</span><span class="sxs-lookup"><span data-stu-id="9ba0f-116">The query returns the first 25 results.</span></span> <span data-ttu-id="9ba0f-117">Результаты поиска упорядочиваются по убыванию даты и времени.</span><span class="sxs-lookup"><span data-stu-id="9ba0f-117">The search results are ordered by Datetime descending.</span></span>

#### <a name="request"></a><span data-ttu-id="9ba0f-118">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ba0f-118">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="9ba0f-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ba0f-119">Response</span></span> 

<span data-ttu-id="9ba0f-120">Ниже приведен пример ответа, содержащего одно сообщение, которое соответствует заданному критерию поиска.</span><span class="sxs-lookup"><span data-stu-id="9ba0f-120">The following is an example of the response which contains one message that matches the search criterion.</span></span> 

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

### <a name="example-2-search-top-results-messages"></a><span data-ttu-id="9ba0f-121">Пример 2. сообщения о главных результатах поиска</span><span class="sxs-lookup"><span data-stu-id="9ba0f-121">Example 2 Search top results messages</span></span>
<span data-ttu-id="9ba0f-122">В следующем примере используется тот же поисковый запрос, что и в [примере 1](#example-1), а результаты сортируются по релевантности.</span><span class="sxs-lookup"><span data-stu-id="9ba0f-122">The following example uses the same search query as [example 1](#example-1), and sorts the results by relevance.</span></span> 

#### <a name="request"></a><span data-ttu-id="9ba0f-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ba0f-123">Request</span></span>

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

## <a name="known-limitations"></a><span data-ttu-id="9ba0f-124">Известные ограничения</span><span class="sxs-lookup"><span data-stu-id="9ba0f-124">Known limitations</span></span>

- <span data-ttu-id="9ba0f-125">Доступ к почтовому ящику пользователя можно получить только.</span><span class="sxs-lookup"><span data-stu-id="9ba0f-125">You can only access a user’s own mailbox.</span></span> <span data-ttu-id="9ba0f-126">Поиск делегированного почтового ящика не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9ba0f-126">Searching delegated mailbox is not supported</span></span> 

- <span data-ttu-id="9ba0f-127">Для сообщений свойство **Total** объекта [сеарчхитсконтаинер](/graph/api/resources/searchhitscontainer?view=graph-rest-beta) содержит количество результатов на странице, а не общее число результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="9ba0f-127">For messages, the **total** property of the [searchHitsContainer](/graph/api/resources/searchhitscontainer?view=graph-rest-beta) type contains the number of results on the page, not the total number of matching results.</span></span>

## <a name="next-steps"></a><span data-ttu-id="9ba0f-128">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="9ba0f-128">Next steps</span></span>

<span data-ttu-id="9ba0f-129">Дополнительные сведения:</span><span class="sxs-lookup"><span data-stu-id="9ba0f-129">Find out more about:</span></span>

- [<span data-ttu-id="9ba0f-130">Использование API поиска</span><span class="sxs-lookup"><span data-stu-id="9ba0f-130">Use the search API</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)
