---
title: Поиск сообщений Outlook с помощью API поиска (Майкрософт)
description: API поиска (Майкрософт) в Microsoft Graph можно использовать для поиска информации в сообщениях электронной почты и возврата сообщений, ранжированных по релевантности.
author: knightsu
ms.localizationpriority: medium
ms.prod: search
ms.openlocfilehash: 1769bda3a6d4f4ed2fed6fc8294b7dc049749482
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436976"
---
# <a name="use-the-microsoft-search-api-to-search-outlook-messages"></a>Поиск сообщений Outlook с помощью API поиска (Майкрософт)

Используйте API поиска (Майкрософт) в Microsoft Graph для поиска информации в сообщениях электронной почты, возврата сообщений, ранжированных по релевантности, и отображения выделенного интерфейса поиска. Поиск применяется к основному тексту и вложениям сообщений в собственном почтовом ящике пользователя, выполнившего вход.

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

Поисковый запрос может включать [фильтры](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da), которые конечные пользователи введите в текстовое поле поиска в Outlook.

Результаты поиска сообщений сортируются по **receivedDateTime** в порядке убывания.

Поиск сообщений применяется к рабочим или учебным учетным записям. Пользователи могут выполнять поиск в собственном почтовом ящике, но не могут выполнять поиск в делегированных почтовых ящиках. Дополнительные сведения см [. в разделе об известных ограничениях](#known-limitations).

Поиск сообщений также ищет вложения. [Поддерживаемые типы файлов для](/SharePoint/technical-reference/default-crawled-file-name-extensions-and-parsed-file-types) поиска вложений сообщений совпадают с типами файлов для поиска в SharePoint Online.

## <a name="example-1-search-messages-in-a-users-mailbox"></a>Пример 1. Поиск сообщений в почтовом ящике пользователя

В следующем примере запрашиваются сообщения в почтовом ящике вошедщего пользователя, содержащие строку contoso в любой части сообщения (имя отправителя, тема, текст сообщения или любые вложения). Запрос возвращает первые 25 результатов. Результаты поиска упорядочены по убыванию **даты и** времени.

### <a name="request"></a>Запрос

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

### <a name="response"></a>Отклик

Ниже приведен пример ответа, который содержит одно сообщение, соответствующее условию поиска.

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

## <a name="example-2-search-top-results-messages"></a>Пример 2. Поиск сообщений с наиболее распространенными результатами

В следующем примере используется поисковый запрос, показанный в примере 1, и результаты сортируются по релевантности. 

<!-- markdownlint-disable MD024 -->
### <a name="request"></a>Запрос

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

### <a name="response"></a>Отклик

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

## <a name="known-limitations"></a>Известные ограничения

- Вы можете получить доступ только к собственному почтовому ящику пользователя, выполнившего вход. Поиск в делегированных почтовых ящиках не поддерживается.
- Для сообщений общее свойство  типа [searchHitsContainer](/graph/api/resources/searchhitscontainer) содержит количество результатов на странице, а не общее число соответствующих результатов.
- Сортировка результатов не поддерживается для событий. Предложение сортировки в запросе возвращает код ошибки "Недопустимый запрос" в ответе.

## <a name="next-steps"></a>Дальнейшие действия

- [Использование API Поиска (Майкрософт) для запроса данных](/graph/api/resources/search-api-overview)
