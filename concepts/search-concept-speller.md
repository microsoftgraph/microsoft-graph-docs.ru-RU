---
title: Использование API Поиска (Майкрософт) для запроса исправлений орфографии
description: Используйте API Поиска (Майкрософт) в Microsoft Graph, чтобы запросить исправления орфографии для обработки несоответствий между опечаток в запросах пользователей и правильными словами в соответствующем содержимом.
author: nmoreau
ms.localizationpriority: medium
ms.prod: search
ms.openlocfilehash: 16375f1c0e38cc5e0acf3f2f89e668d32a042e51
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66438264"
---
# <a name="use-the-microsoft-search-api-to-request-spelling-corrections"></a>Использование API Поиска (Майкрософт) для запроса исправлений орфографии

API поиска (Майкрософт) в Microsoft Graph можно использовать для запроса исправлений орфографии для обработки несоответствий между опечаток в запросах пользователей и правильными словами в соответствующем содержимом. Чтобы запросить исправления орфографии, укажите следующие свойства в свойстве **queryAlterationOptions** [объекта searchRequest](/graph/api/resources/searchrequest):

- **enableSuggestion** позволяет включить или отключить предложения орфографии для пользовательского запроса. Вы можете передать, `true` чтобы получить рекомендуемые сведения о исправлении орфографии для опечаток в пользовательском запросе.

- **enableModification** позволяет включить или отключить изменения орфографии для пользовательского запроса. Вы можете передать результаты `true` поиска для исправленного запроса, если отсутствуют результаты для исходного запроса с опечаток, и получить соответствующие сведения об исправлении.

Приоритет изменения орфографии выше, чем предложение орфографии, если они включены.

Все строки пользовательского запроса должны быть одинаковыми, чтобы включить исправления орфографии для поиска нескольких сущностей.

## <a name="example-1-request-spelling-suggestions"></a>Пример 1. Запрос предложений орфографии

В следующем примере запрашивают **ресурсы listItem** , `accountt` содержащие строку, и запрашивает предложение орфографии для запроса.

Ответ содержит [объекты alterationResponse](/graph/api/resources/alterationResponse) для предложения орфографии.

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
            "size": 25,
            "queryAlterationOptions": {
                "enableSuggestion": true,
                "enableModification": false
            }
        }
    ]
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
    ]
}
```

## <a name="example-2-request-spelling-modifications"></a>Пример 2. Запрос на изменение орфографии

В следующем примере выполняется запрос **ресурсов listItem**`accountt`, содержащих строку, и запрашивает изменение орфографии для запроса.

В этом примере нет результатов для исходного запроса с опечатки `accountt`. Ответ содержит результаты, связанные с исправленной строкой `account` [и объектами alterationResponse](/graph/api/resources/alterationResponse) для изменения орфографии.

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
            "size": 25,
            "queryAlterationOptions": {
                "enableSuggestion": true,
                "enableModification": true
            }
        }
    ]
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
    ]
}
```

## <a name="known-limitations"></a>Известные ограничения

Исправление орфографии поддерживается только для следующих ресурсов: **message**, **event**, **site**, **drive**, **driveItem**, **list**, **listItem** и **externalItem**.

## <a name="next-steps"></a>Дальнейшие действия

- [Использование API Поиска (Майкрософт) для запроса данных](/graph/api/resources/search-api-overview)
