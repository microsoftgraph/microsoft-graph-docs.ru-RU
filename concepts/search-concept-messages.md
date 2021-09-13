---
title: Используйте API Поиск (Майкрософт) в Microsoft Graph для поиска сообщений
description: Вы можете использовать API Поиск (Майкрософт) для поиска сведений в сообщениях электронной почты, возврата сообщений, заданной по релевантности, и отрисовки выделенного опыта поиска.
author: knightsu
ms.localizationpriority: medium
ms.prod: search
ms.openlocfilehash: a4dadd4db51acf2e99e69d4d206526100187ba27
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59103937"
---
# <a name="use-the-microsoft-search-api-to-search-outlook-messages"></a>Используйте API Поиск (Майкрософт) для поиска Outlook сообщений

Используйте API Поиск (Майкрософт) для поиска сведений в сообщениях электронной почты, возврата сообщений, заданной по релевантности, и отрисовки выделенного опыта поиска. Поиск применяется к телу и вложениям сообщений в собственном почтовом ящике пользователя.

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

Запрос поиска может включать [фильтры,](https://support.office.com/article/learn-to-narrow-your-search-criteria-for-better-searches-in-outlook-d824d1e9-a255-4c8a-8553-276fb895a8da) которые  конечные пользователи введите в текстовом окне Поиска в Outlook.

Результаты поиска сообщений сортируют по **receivedDateTime** в порядке убывания.

Поиск сообщений применяется к учетным записям в работе или школе. Пользователи могут искать собственный почтовый ящик, но не могут искать делегированную почтовые ящики. Подробные сведения [см. в известных ограничениях.](#known-limitations)

Поиск сообщений также ищет вложения. [Поддерживаемые типы файлов для](/SharePoint/technical-reference/default-crawled-file-name-extensions-and-parsed-file-types) поиска вложений сообщений такие же, как и для SharePoint Поиска в Интернете.

## <a name="example-1-search-messages-in-a-users-mailbox"></a>Пример 1. Поиск сообщений в почтовом ящике пользователя

В следующем примере запрашиваются сообщения в почтовом ящике подписанного пользователя, содержащие строку "contoso" в любой части сообщения (имя отправитель, субъект, тело сообщения или любые вложения). Запрос возвращает первые 25 результатов. Результаты поиска заказать путем убывка **DateTime.**

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

Ниже приводится пример ответа, содержащем одно сообщение, которое соответствует критерию поиска.

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

## <a name="example-2-search-top-results-messages"></a>Пример 2. Сообщения о результатах поиска

В следующем примере используется поисковый запрос, показанный в примере 1, и сортировать результаты по релевантности. 

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

#### <a name="response"></a>Отклик
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

- Вы можете получить доступ только к собственному почтовому ящику пользователя. Поиск делегирования почтовых ящиков не поддерживается.
- Для сообщений  общее свойство [типа searchHitsContainer](/graph/api/resources/searchhitscontainer) содержит количество результатов на странице, а не общее число совпадающих результатов.
- Результаты сортировки не поддерживаются для событий. Сортивная оговорка в запросе возвращает код ошибки "Плохой запрос" в ответе.

## <a name="next-steps"></a>Дальнейшие действия

- [Использование Поиск (Майкрософт) API](/graph/api/resources/search-api-overview)
