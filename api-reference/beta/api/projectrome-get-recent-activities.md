---
title: Получение последних действий пользователя
description: " Функцию. Служба будет запрашивать последние Historyitem, а затем извлекать эти связанные действия. Действия сортируются в соответствии с последним значением **LastModified** в **historyItem**. Это означает, что действия без **historyitem** не будут включены в ответ. Разрешение UserActivity. ReadWrite. CreatedByApp также будет применять к отклику дополнительную фильтрацию, чтобы возвращались только действия, созданные приложением. Такая фильтрация на стороне сервера может привести к пустым страницам, если пользователь является особенно активным и другие приложения создали более новые действия. Чтобы получить действия приложения, используйте свойство **nextLink** для разбивки на страницы."
localization_priority: Normal
ms.prod: project-rome
doc_type: apiPageType
author: ailae
ms.openlocfilehash: 146b4d83b6fda3dc56744e1b60daf15811ed3747
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314974"
---
# <a name="get-recent-user-activities"></a>Получение последних действий пользователя

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение последних действий для определенного пользователя. Эта функция OData имеет некоторые варианты поведения по умолчанию, которые могут работать так же, как и "самый последний использованный" API. Служба будет запрашивать последние [historyitem](../resources/projectrome-historyitem.md), а затем извлекать эти связанные действия. Действия сортируются в соответствии с последним значением **LastModified** в **historyItem**. Это означает, что действия без **historyitem** не будут включены в ответ. Разрешение UserActivity. ReadWrite. CreatedByApp также будет применять к отклику дополнительную фильтрацию, чтобы возвращались только действия, созданные приложением. Такая фильтрация на стороне сервера может привести к пустым страницам, если пользователь является особенно активным и другие приложения создали более новые действия. Чтобы получить действия приложения, используйте свойство **nextLink** для разбивки на страницы.

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
GET /me/activities/recent
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает некоторые [Параметры запроса OData](/graph/query-parameters) для настройки ответа. Поддерживаются следующие параметры запросов:

- $expand для свойства навигации **historyitem** .
- $top, чтобы ограничить максимальное количество элементов на страницах.
- $filter в свойстве **lastModifiedDateTime** для **действий** или **historyitem**, если она развернута.

Ниже приведено несколько примеров поддерживаемых запросов с кодированием URL-адресов.

```
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a>Заголовки запросов

|Имя | Тип | Описание|
|:----|:-----|:-----------|
|Authorization | string | Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика с последними действиями пользователя для вашего приложения.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "ignored",
  "name": "get_recent_activities"
}-->

```http
GET https://graph.microsoft.com/beta/me/activities/recent
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(userActivity)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/activities/recent?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
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
<!--
{
  "type": "#page.annotation",
  "description": "Get recent activities",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->