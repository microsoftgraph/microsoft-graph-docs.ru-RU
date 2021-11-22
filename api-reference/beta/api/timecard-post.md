---
title: Создание timeCard
description: Создайте экземпляр timeCard в расписании.
author: akumar39
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 25c837de92da4aed25c061ab7a993d5e53c54c4d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60989126"
---
# <a name="create-timecard"></a>Создание timeCard

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание [экземпляра timeCard](../resources/timeCard.md) в [расписании.](../resources/schedule.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Schedule.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Schedule.ReadWrite.All* |

>\***Важно:** При использовании разрешений приложения необходимо включить в запрос `MS-APP-ACTS-AS` заготвую.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timecards
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {token}. Обязательный.  |
| Content-Type | application/json. Обязательный.|
| MS-APP-ACTS-AS | ID пользователя, от имени которого действует приложение. Требуется при использовании области разрешений приложения. |

## <a name="request-body"></a>Текст запроса

Предокажи новый [объект timeCard](../resources/timecard.md) в теле запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект timeCard](../resources/timeCard.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса. 

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timecard-post"
}-->

```http
POST https://graph.microsoft.com/beta/teams/871dbd5c-3a6a-4392-bfe1-042452793a50/schedule/timecards
Content-type: application/json

{
  "onBehalfOfUserId":"a3601044-a1b5-438e-b742-f78d01d68a67",
  "clockInEvent":{
     "dateTime":"2019-03-18T00:00:00.000Z",
     "atApprovedLocation":true,
     "notes": {
        "content": "Started late due to traffic in CA 237",
        "contentType": "text"
     },
  },
  "notes":{
        "content": "8 To 5 Inventory management",
        "contentType": "text"
   },
  "breaks":[
     {
       "breakId": "string",
        "notes":{
             "content": "Lunch break",
             "contentType": "text"
        },
        "start":{
           "dateTime":"2019-03-18T02:00:00.000Z",
           "atApprovedLocation":true,
           "notes": {
                "content": "Reduced break to make up for lost time",
                "contentType": "text"
             },
        }
     }
  ]
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timecard-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timecard-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/timecard-post-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример ответа. 

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeCard"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
   "id":"3895809b-a618-4c0d-86a0-d42b25b7d74f",
   "userId":"a3601044-a1b5-438e-b742-f78d01d68a67",
   "createdDateTime":"2019-03-18T00:00:00.000Z",
   "createdBy":{
      "user":{
         "id":"a3601044-a1b5-438e-b742-f78d01d68a67",
         "displayName":"Dwight Schrute"
      }
   },
   "lastModifiedDateTime":"2019-03-18T00:00:00.000Z",
   "lastModifiedBy":{
      "user":{
         "id":"a3601044-a1b5-438e-b742-f78d01d68a67",
         "displayName":"Dwight Schrute"
      }
   },
   "state":"onBreak",
   "confirmationStatus":"notConfirmed",
   "originalEntry":{
      "clockInEvent":{
         "dateTime":"2019-03-18T00:00:00.000Z",
         "atApprovedLocation":true,
         "notes": {
            "content": "Started late due to traffic in CA 237",
           "contentType": "text"
         },
      },
      "clockOutEvent":null,
      "breaks":[
         {
            "breakId":"string",
            "notes":{
                "content": "Lunch break",
                "contentType": "text"
             },
            "start":{
               "dateTime":"2019-03-18T02:00:00.000Z",
               "atApprovedLocation":true,
               "notes": {
                  "content": "Reduced break to make up for lost time",
                  "contentType": "text"
               },
            },
            "end":null
         }
      ]
   },
   "clockInEvent":{
      "dateTime":"2019-03-18T00:00:00.000Z",
      "atApprovedLocation":true,
      "notes": {
        "content": "Started late due to traffic in CA 237",
        "contentType": "text"
     },
   },
   "clockOutEvent":null,
   "notes":{
        "content": "8 To 5 Inventory management",
        "contentType": "text"
   },
   "breaks":[
      {
         "breakId":"string",
         "notes":{
             "content": "Lunch break",
             "contentType": "text"
         },
         "start":{
            "dateTime":"2019-03-18T02:00:00.000Z",
            "atApprovedLocation":true,
            "notes": {
                "content": "Reduced break to make up for lost time",
                "contentType": "text"
             },
         },
         "end":null
      }
   ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create timeCard",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
