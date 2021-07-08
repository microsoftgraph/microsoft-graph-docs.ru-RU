---
title: Используйте API Поиск (Майкрософт) в Microsoft Graph для поиска людей (предварительный просмотр)
description: Вы можете использовать API Поиск (Майкрософт) для поиска подходящих для вас людей.
author: acsehi
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: b9e53fadf7df205c315daf090350e7b4748b9025
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334820"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-search-people-preview"></a>Используйте API Поиск (Майкрософт) в Microsoft Graph для поиска людей (предварительный просмотр)

Microsoft Graph приложения могут использовать API поиска для получения людей, наиболее подходящих для пользователя. Релевантность определяется шаблонами общения и совместной работы пользователя, а также его бизнес-отношениями. Люди могут быть локальными контактами или из каталога организации, а также людьми из последних сообщений. Наряду с созданием этого анализа поиск также предоставляет нечеткие соответствующие поддержку поиска и возможность получения списка пользователей, соответствующих другому пользователю в организации пользователя.

## <a name="example-search-person-by-name"></a>Пример: Поиск человека по имени

Следующий запрос получает людей, наиболее подходящих для подписанного пользователя, на основе шаблонов связи и совместной работы и деловых отношений.

### <a name="request"></a>Запрос

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "person"
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
    "@odata.context": "https://canary.graph.microsoft.com/testprodbetapersoninsearch/$metadata#microsoft.graph.searchResponse",
    "value": [
        {
            "hitsContainers": [
                {
                    "total": 1,
                    "moreResultsAvailable": false,
                    "hits": [
                        {
                            "hitId": "fc138b85-18ac-48e0-80a4-633ae4b594e0@41f988bf-86f1-53af-91ab-2d7cd034db47",
                            "rank": 1,
                            "summary": "",
                            "resource": {
                                "@odata.type": "#microsoft.graph.person",
                                "displayName": "Example User",
                                "givenName": "User",
                                "surname": "User",
                                "department": "Finance",
                                "officeLocation": "London",
                                "userPrincipalName": "example.user@contoso.com",
                                "emailAddresses": [
                                    {
                                        "address": "example.user@contoso.com",
                                        "rank": 1
                                    }
                                ],
                                "phones": [
                                    {
                                        "type": "business",
                                        "number": "+44 (20) 12345678"
                                    }
                                ]
                            }
                        }
                    ]
                }
            ]
        }
    ]
}
```

## <a name="next-steps"></a>Дальнейшие действия

- [Использование Поиск (Майкрософт) API](/graph/api/resources/search-api-overview)
