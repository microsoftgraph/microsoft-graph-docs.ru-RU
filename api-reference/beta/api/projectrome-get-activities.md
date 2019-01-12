---
title: Получение действия пользователя
description: Получение действий для определенного пользователя. В отличие от **последние** функции OData будут возвращены действия без личных дел. Разрешение UserActivity.ReadWrite.CreatedByApp будут применяться дополнительных фильтрации в ответ, чтобы возвращаются только действий, созданных приложением. В этом фильтрации на сервере может привести к пустой страницы Если пользователь является особенно active и другие приложения были созданы более последние действия. Для получения действия этого приложения, используйте свойство **nextLink** для разбиения по страницам.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: d6b2f4c14e1f33a09ed81aeb2c8d626ed70bcdc5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928187"
---
# <a name="get-user-activities"></a>Получение действия пользователя

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Получение действий для определенного пользователя. В отличие от **последние** функции OData будут возвращены действия без личных дел. Разрешение UserActivity.ReadWrite.CreatedByApp будут применяться дополнительных фильтрации в ответ, чтобы возвращаются только действий, созданных приложением. В этом фильтрации на сервере может привести к пустой страницы Если пользователь является особенно active и другие приложения были созданы более последние действия. Для получения действия этого приложения, используйте свойство **nextLink** для разбиения по страницам.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | UserActivity.ReadWrite.CreatedByApp    |
|Делегированные (личная учетная запись Майкрософт) | UserActivity.ReadWrite.CreatedByApp    |
|Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает некоторые [Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа. Поддерживаются следующие параметры запроса:

- для свойства **historyItems** навигации разверните $.
- Чтобы ограничить максимальное число элементов на страницах $top.
- $filter свойства **lastModifiedDateTime** для **действия** или **historyItems**, если были развернуты.

Ниже приведены некоторые примеры поддерживаемых запросов с кодировкой URL-адрес:

```
/me/activities?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities?$top=5
```

## <a name="request-headers"></a>Заголовки запросов

|Имя | Тип | Описание|
|:----|:-----|:-----------|
|Authorization | string | Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Тело запроса

Нет текста запроса.

## <a name="response"></a>Ответ

Успешно завершена, этот метод возвращает `200 OK` код ответа с помощью действий пользователя для приложения.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "ignored",
  "name": "get_activities"
}-->

```http
GET https://graph.microsoft.com/beta/me/activities
```

##### <a name="response"></a>Ответ

Ниже приведен пример ответа.

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.activity)"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(userActivity)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/activities?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
    "value": [{
        "@odata.type": "#microsoft.graph.activity",
        "activitySourceHost": "https://www.contoso.com",
        "createdDateTime": "2018-02-26T18:34:29.592Z",
        "lastModifiedDateTime": "2018-02-26T18:34:29.607Z",
        "id": "5347642601316252694",
        "appActivityId": "/article?12345",
        "visualElements": {
            "attribution": {
              "iconUrl": "https://www.contoso.com/icon",
              "alternateText": "Contoso, Ltd.",
              "addImageQuery": "false",
              },
            "displayText": "Contoso How-To: How to Tie a Reef Knot",
            "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
            "backgroundColor": "#ff0000",
            "content": {
              "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
              "type": "AdaptiveCard",
              "body":
              [{
                  "type": "TextBlock",
                  "text": "Contoso MainPage"
              }]
            }
        },
        "activationUrl": "https://www.contoso.com/article?id=12345",
        "appDisplayName": "Contoso, Ltd.",
        "userTimezone": "Africa/Casablanca",
        "fallbackUrl": "https://www.contoso.com/article?id=12345",
        "contentUrl": "https://www.contoso.com/article?id=12345",
        "contentInfo": {
            "@context": "https://schema.org",
            "@type": "Article",
            "author": "John Doe",
            "name": "How to Tie a Reef Knot"
        },
        "expirationDateTime": "2018-03-28T18:34:29.607Z",
        "status": "updated"
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get activities",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
