---
title: Используйте API Поиск (Майкрософт) в Microsoft Graph для запроса исправлений орфографии
description: Вы можете использовать API Поиск (Майкрософт) для получения предложения орфографии или изменения орфографии для поиска запроса.
author: nmoreau
ms.localizationpriority: medium
ms.prod: search
ms.openlocfilehash: a16c1e0a69e202ca34c1c52c176a15c0b5da7e88
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59071730"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-request-spelling-correction-preview"></a>Используйте API Поиск (Майкрософт) в Microsoft Graph для запроса исправления орфографии (предварительный просмотр)

Вы можете использовать API Поиск (Майкрософт) для запроса исправлений орфографии для обработки несоответствий между опечатками в запросах пользователей и правильными словами в содержимом. Чтобы запросить исправления орфографии, укажите следующие свойства в **свойстве requestAlterationOptions** тела запроса [метода](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) запроса:

- **enableSuggestion** для включения и отключения предложений орфографии для запроса пользователя. Вы можете передать, чтобы получить рекомендуемые сведения об исправлении орфографии для `true` опечаток в запросе пользователя.

- **enableModification,** чтобы включить/отключить изменения орфографии для пользовательского запроса. Вы можете передать, чтобы получить результаты поиска для исправленного запроса, если нет результатов для исходного запроса с опечатки, и получить соответствующие `true` сведения о  исправлении.

Приоритет изменения орфографии выше, чем предложение орфографии, если они включены.

Все строки запросов пользователей должны быть одинаковыми, чтобы включить исправления орфографии для поиска нескольких сущностями.

## <a name="example-1-request-spelling-suggestions"></a>Пример 1. Запрос предложений по написанию

В следующем примере запрашиваются **ресурсы listItem,** содержащие строку "учетная запись", и запрашивается предложение орфографии для запроса.

Ответ содержит [объекты alterationResponse](/graph/api/resources/alterationResponse?view=graph-rest-beta&preserve-view=true) для предложения орфографии.

### <a name="request"></a>Запрос

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json

{
    "requests": [
        {
            "entityTypes": [
                "listItem"
            ],
            "query": {
                "queryString": "accountt"
            },
            "from": 0,
            "size": 25
        }
    ],
    "queryAlterationOptions": {
        "enableSuggestion": true,
        "enableModification": false
    }
}
```

### <a name="response"></a>Отклик

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.searchResponse)",
    "value": [
        {
            "searchTerms": [
                "accountt"
            ],
            "hitsContainers": [
                {
                    "total": 0,
                    "moreResultsAvailable": false
                }
            ]
        }
    ],
    "queryAlterationResponse": {
        "@odata.type": "#microsoft.substrateSearch.alterationResponse",
        "originalQueryString": "accountt",
        "queryAlteration": {
            "@odata.type": "#microsoft.substrateSearch.searchAlteration",
            "alteredQueryString": "account",
            "alteredHighlightedQueryString": "account",
            "alteredQueryTokens": [
                {
                    "offset": 0,
                    "length": 8,
                    "suggestion": "account"
                }
            ]
        },
        "queryAlterationType": "Suggestion"
    }
}
```

## <a name="example-2-request-spelling-modifications"></a>Пример 2. Запрос на изменения орфографии

В следующем примере запрашиваются **ресурсы listItem,** содержащие строку "учетная запись", и запрашивается изменение орфографии для запроса.

В этом примере нет результатов для исходного запроса с помощью опечатки "учетная запись". Ответ содержит результаты, связанные с исправленными объектами строки "учетная запись" и [объектами alterationResponse](/graph/api/resources/alterationResponse?view=graph-rest-beta&preserve-view=true) для изменения орфографии.

### <a name="request"></a>Запрос

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json

{
    "requests": [
        {
            "entityTypes": [
                "listItem"
            ],
            "query": {
                "queryString": "accountt"
            },
            "from": 0,
            "size": 25
        }
    ],
    "queryAlterationOptions": {
        "enableSuggestion": true,
        "enableModification": true
    }
}
```

### <a name="response"></a>Отклик

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.searchResponse)",
    "value": [
        {
            "searchTerms": [
                "account"
            ],
            "hitsContainers": [
                {
                    "total": 1,
                    "moreResultsAvailable": false,
                    "hits": [
                        {
                            "hitId": "FlULeN/ui/1GjLx1rUfio5UAAEl",
                            "rank": 1,
                            "summary": "",
                            "resource": {
                                "@odata.type": "#microsoft.graph.listItem",
                                "createdDateTime": "2019-06-10T06:37:43Z",
                                "lastModifiedDateTime": "2019-06-10T06:37:43Z",
                                "name": "web_part_test_long Notebook",
                                "webUrl": "https://contoso.sharepoint.com/sites/contoso-team/Lists/Issue tracker list/DispForm.aspx?ID=1",
                                "sharepointIds": {
                                    "listId": "33498de0-d695-4d23-ac26-e1bf95a3206e",
                                    "listItemId": "13"
                                },
                                "createdBy": {
                                    "user": {
                                        "displayName": "System Account"
                                    }
                                },
                                "lastModifiedBy": {
                                    "user": {
                                        "displayName": "System Account"
                                    }
                                },
                                "parentReference": {
                                    "sharepointIds": {
                                        "listId": "da61a2b0-4120-4a3f-812b-0fc0d79bf16b"
                                    },
                                    "siteId": "m365x231305.sharepoint.com,5724d91f-650c-4810-83cc-61a8818917d6,c3ba25dc-2c9f-48cb-83be-74cdf68ea5a0"
                                }
                            }
                        }
                    ]
                }
            ]
        }
    ],
    "queryAlterationResponse": {
        "@odata.type": "#microsoft.substrateSearch.alterationResponse",
        "originalQueryString": "accountt",
        "queryAlteration": {
            "@odata.type": "#microsoft.substrateSearch.searchAlteration",
            "alteredQueryString": "account",
            "alteredHighlightedQueryString": "account",
            "alteredQueryTokens": [
                {
                    "offset": 0,
                    "length": 8,
                    "suggestion": "account"
                }
            ]
        },
        "queryAlterationType": "Modification"
    }
}
```

## <a name="known-limitations"></a>Известные ограничения

Исправление орфографии поддерживается только для следующих ресурсов: **сообщение,** **событие,** **сайт,** **диск**, **driveItem**, **список**, **listItem** и **externalItem**.

## <a name="next-steps"></a>Дальнейшие действия

- [Использование API Поиска (Майкрософт) для запроса данных](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
