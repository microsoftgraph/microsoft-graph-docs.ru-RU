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
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-search-people-preview"></a><span data-ttu-id="f00ff-103">Используйте API Поиск (Майкрософт) в Microsoft Graph для поиска людей (предварительный просмотр)</span><span class="sxs-lookup"><span data-stu-id="f00ff-103">Use the Microsoft Search API in Microsoft Graph to search people (preview)</span></span>

<span data-ttu-id="f00ff-104">Microsoft Graph приложения могут использовать API поиска для получения людей, наиболее подходящих для пользователя.</span><span class="sxs-lookup"><span data-stu-id="f00ff-104">Microsoft Graph applications can use the Search API to retrieve the people who are most relevant to a user.</span></span> <span data-ttu-id="f00ff-105">Релевантность определяется шаблонами общения и совместной работы пользователя, а также его бизнес-отношениями.</span><span class="sxs-lookup"><span data-stu-id="f00ff-105">Relevance is determined by the user’s communication and collaboration patterns and business relationships.</span></span> <span data-ttu-id="f00ff-106">Люди могут быть локальными контактами или из каталога организации, а также людьми из последних сообщений.</span><span class="sxs-lookup"><span data-stu-id="f00ff-106">People can be local contacts or from an organization’s directory, and people from recent communications.</span></span> <span data-ttu-id="f00ff-107">Наряду с созданием этого анализа поиск также предоставляет нечеткие соответствующие поддержку поиска и возможность получения списка пользователей, соответствующих другому пользователю в организации пользователя.</span><span class="sxs-lookup"><span data-stu-id="f00ff-107">Along with generating this insight, search also provides fuzzy matching search support and the ability to retrieve the list of users relevant to another user in the signed in user's organization.</span></span>

## <a name="example-search-person-by-name"></a><span data-ttu-id="f00ff-108">Пример: Поиск человека по имени</span><span class="sxs-lookup"><span data-stu-id="f00ff-108">Example: Search person by name</span></span>

<span data-ttu-id="f00ff-109">Следующий запрос получает людей, наиболее подходящих для подписанного пользователя, на основе шаблонов связи и совместной работы и деловых отношений.</span><span class="sxs-lookup"><span data-stu-id="f00ff-109">The following request gets the people most relevant to the signed in user, based on communication and collaboration patterns and business relationships.</span></span>

### <a name="request"></a><span data-ttu-id="f00ff-110">Запрос</span><span class="sxs-lookup"><span data-stu-id="f00ff-110">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="f00ff-111">Отклик</span><span class="sxs-lookup"><span data-stu-id="f00ff-111">Response</span></span>

<span data-ttu-id="f00ff-112">Ниже приводится пример ответа, содержащем одно сообщение, которое соответствует критерию поиска.</span><span class="sxs-lookup"><span data-stu-id="f00ff-112">The following is an example of the response, which contains one message that matches the search criterion.</span></span>

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

## <a name="next-steps"></a><span data-ttu-id="f00ff-113">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="f00ff-113">Next steps</span></span>

- [<span data-ttu-id="f00ff-114">Использование Поиск (Майкрософт) API</span><span class="sxs-lookup"><span data-stu-id="f00ff-114">Use the Microsoft Search API</span></span>](/graph/api/resources/search-api-overview)
