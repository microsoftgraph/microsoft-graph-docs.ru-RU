---
title: Список timeCard
description: Извлечение списка записей timeCard в расписании.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1635e8c524b25b3795bf90f03449eddf259ff208
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787905"
---
# <a name="list-timecard"></a>Список timeCard

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Извлечение списка [записей timeCard](../resources/timecard.md) в расписании. [](../resources/schedule.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Schedule.Read.All, Schedule.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | Schedule.Read.All *, Schedule.ReadWrite.All* |

>\***Важно:** При использовании разрешений приложения необходимо включить в запрос `MS-APP-ACTS-AS` заготвую.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timecards
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает `$filter` параметры `$orderBy` запроса `$top` `$skipToken` OData, которые помогут настроить ответ. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов

| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |
| MS-APP-ACTS-AS | ID пользователя, от имени которого действует приложение. Требуется при использовании области разрешений приложения. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и список объектов `200 OK` [timeCard](../resources/timeCard.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса. 

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timecard-list"
}-->

```http
GET https://graph.microsoft.com/beta/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards?$top=2&$filter=state eq 'clockedOut'

```

### <a name="response"></a>Отклик

Ниже приведен пример ответа. 

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeCard"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "@odata.etag": "\"3400c313-0000-0d00-0000-60afe1940000\"",
            "id": "TCK_d1e0f245-9996-4125-b128-d3eb5c4b0164",
            "createdDateTime": "2020-09-21T18:01:29.302Z",
            "lastModifiedDateTime": "2021-05-27T18:14:44.503Z",
            "userId": "66b4f2a4-425d-4dec-8172-7e889950885e",
            "state": "clockedOut",
            "confirmedBy": "none",
            "notes": null,
            "lastModifiedBy": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
                    "displayName": "Jing Jing GuTwo"
                }
            },
            "clockInEvent": {
                "dateTime": "2020-09-21T18:01:29.302Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "ClockIn-OBO Shorbani"
                }
            },
            "clockOutEvent": {
                "dateTime": "2021-05-27T18:14:44.503Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "clock out notes"
                }
            },
            "breaks": [],
            "originalEntry": {
                "clockInEvent": {
                    "dateTime": "2020-09-21T18:01:29.302Z",
                    "atApprovedLocation": null,
                    "notes": {
                        "contentType": "text",
                        "content": "ClockIn-OBO Shorbani"
                    }
                },
                "clockOutEvent": {
                    "dateTime": "2021-05-27T18:14:44.503Z",
                    "atApprovedLocation": null,
                    "notes": {
                        "contentType": "text",
                        "content": "clock out notes"
                    }
                },
                "breaks": []
            },
            "createdBy": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "66b4f2a4-425d-4dec-8172-7e889950885e",
                    "displayName": "Janani Varadharajan"
                }
            }
        },
        {
            "@odata.etag": "\"3400d914-0000-0d00-0000-60afe1ee0000\"",
            "id": "TCK_aa73c610-dd75-4021-bb5c-6b071c7aa835",
            "createdDateTime": "2020-09-21T18:02:48.688Z",
            "lastModifiedDateTime": "2021-05-27T18:16:14.766Z",
            "userId": "3041ccde-7544-4ae0-b44f-3618b08ba1ce",
            "state": "clockedOut",
            "confirmedBy": "none",
            "notes": null,
            "lastModifiedBy": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
                    "displayName": "Jing Jing GuTwo"
                }
            },
            "clockInEvent": {
                "dateTime": "2020-09-21T18:02:48.688Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "ClockIn-OBO Shorbani"
                }
            },
            "clockOutEvent": {
                "dateTime": "2021-05-27T18:16:14.766Z",
                "atApprovedLocation": null,
                "notes": {
                    "contentType": "text",
                    "content": "clock out notes"
                }
            },
            "breaks": [],
            "originalEntry": {
                "clockInEvent": {
                    "dateTime": "2020-09-21T18:02:48.688Z",
                    "atApprovedLocation": null,
                    "notes": {
                        "contentType": "text",
                        "content": "ClockIn-OBO Shorbani"
                    }
                },
                "clockOutEvent": {
                    "dateTime": "2021-05-27T18:16:14.766Z",
                    "atApprovedLocation": null,
                    "notes": {
                        "contentType": "text",
                        "content": "clock out notes"
                    }
                },
                "breaks": []
            },
            "createdBy": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "66b4f2a4-425d-4dec-8172-7e889950885e",
                    "displayName": "Janani Varadharajan"
                }
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Retrieve a list of timeCard entries in the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
