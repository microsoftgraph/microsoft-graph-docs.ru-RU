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
# <a name="search-messages"></a>Поиск сообщений

API Microsoft Search позволяет приложениям искать информацию в сообщениях электронной почты, получать сообщения, Ранжированные по релевантности, и отображать выделенный интерфейс для поиска. Поиск применяется к тексту и вложениям сообщений в собственном почтовом ящике пользователя. 

Поисковый запрос может включать в себя [фильтры](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da) , вводимые пользователями в текстовое поле **поиска** в Outlook.

Результаты поиска сообщений сортируются по **receivedDateTime** в порядке убывания.

В настоящее время поиск сообщений применяется только к собственным личным учетным записям пользователей, но не к рабочим или учебным учетным записям, а не к делегированным почтовым ящикам. Ниже приводятся более [Известные ограничения](#known-limitations) .

## <a name="examples"></a>Примеры

### <a name="example-1"></a>Пример 1

В следующем примере выполняется запрос сообщений в почтовом ящике вошедшего пользователя, который содержит строку "contoso" в любой части сообщения (имя отправителя, тема, текст сообщения или вложения). Запрос возвращает первые 25 результатов. Результаты поиска упорядочиваются по убыванию даты и времени.

#### <a name="request"></a>Запрос

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

#### <a name="response"></a>Отклик 

Ниже приведен пример ответа, содержащего одно сообщение, которое соответствует заданному критерию поиска. 

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

### <a name="example-2-search-top-results-messages"></a>Пример 2. сообщения о главных результатах поиска
В следующем примере используется тот же поисковый запрос, что и в [примере 1](#example-1), а результаты сортируются по релевантности. 

#### <a name="request"></a>Запрос

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

## <a name="known-limitations"></a>Известные ограничения

- Доступ к почтовому ящику пользователя можно получить только. Поиск делегированного почтового ящика не поддерживается 

- Для сообщений свойство **Total** объекта [сеарчхитсконтаинер](/graph/api/resources/searchhitscontainer?view=graph-rest-beta) содержит количество результатов на странице, а не общее число результатов поиска.

## <a name="next-steps"></a>Дальнейшие действия

Дополнительные сведения:

- [Использование API поиска](/graph/api/resources/search-api-overview?view=graph-rest-beta)
