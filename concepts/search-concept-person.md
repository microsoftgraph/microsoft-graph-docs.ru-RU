---
title: Использование API поиска (Майкрософт) для поиска людей
description: Используйте API поиска (Майкрософт) в Microsoft Graph для поиска людей, относящихся к пользователю, определяемого шаблонами общения и бизнес-связями пользователя.
author: acsehi
ms.localizationpriority: medium
ms.prod: search
ms.openlocfilehash: 3b1165a0bcac91ef7a74078b2d88fb268d0f40c6
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436199"
---
# <a name="use-the-microsoft-search-api-to-search-people"></a>Использование API поиска (Майкрософт) для поиска людей

Приложения Microsoft Graph могут использовать API поиска (Майкрософт) для извлечения людей, наиболее релевантных для пользователя. Релевантность определяется шаблонами общения и совместной работы пользователя, а также его бизнес-отношениями. Пользователи могут быть локальными контактами или из каталога организации или пользователями из последних сообщений.

Наряду с созданием этой аналитики поиск также обеспечивает поддержку поиска нечетких соответствий и возможность получения списка пользователей, относящихся к другому пользователю в организации вошедвшего пользователя.

## <a name="example-search-person-by-name"></a>Пример: поиск пользователя по имени

Следующий запрос возвращает людей, наиболее релевантных для вошедвшего пользователя, на основе шаблонов взаимодействия и совместной работы и бизнес-связей.

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

Ниже приведен пример ответа, который содержит одно сообщение, соответствующее условию поиска.

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

- [Использование API Поиска (Майкрософт) для запроса данных](/graph/api/resources/search-api-overview)
