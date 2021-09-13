---
title: Получения действий пользователя
description: Получите действия для данного пользователя. В отличие **от недавней** функции OData, будут возвращены действия без историй. Разрешение UserActivity.ReadWrite.CreatedByApp применяет дополнительную фильтрацию к ответу, чтобы возвращались только действия, созданные вашим приложением. Это фильтрация на стороне сервера может привести к пустым страницам, если пользователь особенно активен, а другие приложения создали более последние действия. Чтобы получить действия приложения, используйте свойство **nextLink** для пагинации.
ms.localizationpriority: medium
ms.prod: project-rome
author: ailae
doc_type: apiPageType
ms.openlocfilehash: 9a9829c420cb937bd137875b775ab42479c56664
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59104763"
---
# <a name="get-user-activities"></a>Получения действий пользователя

Пространство имен: microsoft.graph

Получите действия для данного пользователя. В отличие **от недавней** функции OData, будут возвращены действия без историй. Разрешение UserActivity.ReadWrite.CreatedByApp применяет дополнительную фильтрацию к ответу, чтобы возвращались только действия, созданные вашим приложением. Это фильтрация на стороне сервера может привести к пустым страницам, если пользователь особенно активен, а другие приложения создали более последние действия. Чтобы получить действия приложения, используйте свойство **nextLink** для пагинации.

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

Этот метод поддерживает некоторые [параметры запроса OData для](/graph/query-parameters) настройки ответа. Поддерживаются следующие параметры запроса:

- $expand для свойства **навигации historyItems.**
- $top ограничить максимальное количество элементов на страницах.
- $filter в **свойстве lastModifiedDateTime** для действий или **historyItems,** если они расширены.

Ниже приводится несколько примеров поддерживаемых запросов с кодией URL-адресов:

```
/me/activities?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities?$top=5
```

## <a name="request-headers"></a>Заголовки запросов

|Имя | Тип | Описание|
|:----|:-----|:-----------|
|Authorization | string | Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса

Нет тела запроса.

## <a name="response"></a>Отклик

В случае успешного применения этот метод возвращает код ответа с действиями `200 OK` пользователя для приложения.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "ignored",
  "name": "get_activities"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/activities
```

##### <a name="response"></a>Отклик

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(userActivity)",
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/activities?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
    "value": [{
        "@odata.type": "#microsoft.graph.userActivity",
        "activitySourceHost": "https://www.contoso.com",
        "createdDateTime": "2018-02-26T18:34:29.592Z",
        "lastModifiedDateTime": "2018-02-26T18:34:29.607Z",
        "id": "5347642601316252694",
        "appActivityId": "/article?12345",
        "visualElements": {
            "attribution": {
              "iconUrl": "https://www.contoso.com/icon",
              "alternateText": "Contoso, Ltd.",
              "addImageQuery": false,
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
