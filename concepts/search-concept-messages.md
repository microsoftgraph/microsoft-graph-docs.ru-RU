---
title: Использование API службы поиска Microsoft в Microsoft Graph для поиска сообщений
description: Вы можете использовать API Microsoft Search API для поиска информации в сообщениях электронной почты, получения сообщений, упорядоченных по релевантности, и отображения выделенного интерфейса поиска.
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: e9917b8153946161168e90f78399f29b6a7f3df3
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288828"
---
# <a name="use-the-microsoft-search-api-to-search-outlook-messages"></a>Использование API службы поиска Microsoft для поиска сообщений Outlook

Используйте API Microsoft Search API для поиска информации в сообщениях электронной почты, получения сообщений, упорядоченных по релевантности, и отображения выделенного интерфейса поиска. Поиск применяется к основному тексту и вложениям сообщений в собственном почтовом ящике вошедшего пользователя.

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

Поисковый запрос может включать в себя [фильтры](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da) , вводимые пользователями в текстовое поле **поиска** в Outlook.

Результаты поиска сообщений сортируются по **receivedDateTime** в порядке убывания.

Поиск сообщений применяется к рабочим или учебным учетным записям. Пользователи могут выполнять поиск в своем почтовом ящике, но не могут искать делегированные почтовые ящики. Подробнее: [Известные ограничения](#known-limitations).

При поиске сообщений также выполняется поиск вложений. [Поддерживаются такие же типы файлов](/SharePoint/technical-reference/default-crawled-file-name-extensions-and-parsed-file-types) , что и для поиска в SharePoint Online.

## <a name="example-1-search-messages-in-a-users-mailbox"></a>Пример 1: Поиск сообщений в почтовом ящике пользователя

В следующем примере выполняется запрос сообщений в почтовом ящике вошедшего пользователя, который содержит строку "contoso" в любой части сообщения (имя отправителя, тема, текст сообщения или вложения). Запрос возвращает первые 25 результатов. Результаты поиска упорядочиваются по убыванию **даты и времени** .

### <a name="request"></a>Запрос

```HTTP
POST https://graph.microsoft.com/beta/search/query
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

### <a name="response"></a>Отклик

Ниже приведен пример ответа, содержащего одно сообщение, которое соответствует заданному критерию поиска.

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

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

## <a name="example-2-search-top-results-messages"></a>Пример 2: Поиск в сообщениях с наибольшим результатом

В следующем примере используется поисковый запрос, показанный в примере 1, и отсортирует результаты по релевантности. 

<!-- markdownlint-disable MD024 -->
### <a name="request"></a>Запрос

```HTTP
POST https://graph.microsoft.com/beta/search/query
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

#### <a name="response"></a>Отклик
```HTTP
HTTP/1.1 200 OK
Content-type: application/json

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

## <a name="known-limitations"></a>Известные ограничения

- Доступ к почтовому ящику вошедшего пользователя можно получить только из собственного почтового ящика. Поиск делегированных почтовых ящиков не поддерживается.
- Для сообщений свойство **Total** объекта [сеарчхитсконтаинер](/graph/api/resources/searchhitscontainer?view=graph-rest-beta&preserve-view=true) содержит количество результатов на странице, а не общее число результатов поиска.
- Сортировка результатов не поддерживается для событий. Предложение Sort в запросе возвратит код ошибки ошибочного запроса в ответе.

## <a name="next-steps"></a>Дальнейшие действия

- [Использование API службы поиска Microsoft](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)