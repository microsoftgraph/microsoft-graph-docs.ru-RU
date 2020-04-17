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
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-search-messages"></a>Использование API службы поиска Microsoft в Microsoft Graph для поиска сообщений

Вы можете использовать API Microsoft Search API для поиска информации в сообщениях электронной почты, получения сообщений, упорядоченных по релевантности, и отображения выделенного интерфейса поиска. Поиск применяется к тексту и вложениям сообщений в собственном почтовом ящике пользователя.

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

Поисковый запрос может включать в себя [фильтры](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da) , вводимые пользователями в текстовое поле **поиска** в Outlook.

Результаты поиска сообщений сортируются по **receivedDateTime** в порядке убывания.

Поиск сообщений применяется к рабочим или учебным учетным записям. Пользователи могут выполнять поиск в своем почтовом ящике, но не могут искать делегированные почтовые ящики. Подробнее: [Известные ограничения](#known-limitations).

При поиске сообщений также выполняется поиск вложений. [Поддерживаются такие же типы файлов](https://docs.microsoft.com/SharePoint/technical-reference/default-crawled-file-name-extensions-and-parsed-file-types) , что и для поиска в SharePoint Online.

## <a name="examples"></a>Примеры

### <a name="example-1-search-messages-in-a-users-mailbox"></a>Пример 1: Поиск сообщений в почтовом ящике пользователя

В следующем примере выполняется запрос сообщений в почтовом ящике вошедшего пользователя, который содержит строку "contoso" в любой части сообщения (имя отправителя, тема, текст сообщения или вложения). Запрос возвращает первые 25 результатов. Результаты поиска упорядочиваются по убыванию **даты и времени** .

#### <a name="request"></a>Запрос

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

#### <a name="response"></a>Отклик

Ниже приведен пример ответа, содержащего одно сообщение, которое соответствует заданному критерию поиска. 

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

### <a name="example-2-search-top-results-messages"></a>Пример 2: Поиск в сообщениях с наибольшим результатом
В следующем примере используется поисковый запрос, показанный в [примере 1](#example-1), и отсортирует результаты по релевантности. 

<!-- markdownlint-disable MD024 -->
#### <a name="request"></a>Запрос

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

## <a name="known-limitations"></a>Известные ограничения

- Доступ к почтовому ящику пользователя можно получить только. Поиск делегированных почтовых ящиков не поддерживается.
- Для сообщений свойство **Total** объекта [сеарчхитсконтаинер](/graph/api/resources/searchhitscontainer?view=graph-rest-beta) содержит количество результатов на странице, а не общее число результатов поиска.

## <a name="next-steps"></a>Дальнейшие действия

- [Использование API службы поиска Microsoft](/graph/api/resources/search-api-overview?view=graph-rest-beta)
