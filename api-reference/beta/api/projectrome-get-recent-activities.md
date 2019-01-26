---
title: Получите последние действия пользователя
description: " API-ИНТЕРФЕЙС. Служба запросов для последних historyItems и затем по запросу этих связанных действий. Действия будут упорядочены в соответствии с самыми последними **lastModified** на **historyItem**. Это означает, что действия без **historyItems** не будут включены в ответе. Разрешение UserActivity.ReadWrite.CreatedByApp будут также применены дополнительные фильтрации в ответ, чтобы возвращаются только действий, созданных приложением. В этом фильтрации на сервере может привести к пустой страницы Если пользователь является особенно active и другие приложения были созданы более последние действия. Для получения действия этого приложения, используйте свойство **nextLink** для разбиения по страницам."
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: f19dc8eea40d61afba8e34891431a73f565d6ec3
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573167"
---
# <a name="get-recent-user-activities"></a>Получите последние действия пользователя

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите последние действия для данного пользователя. Эта функция OData имеет некоторые поведения по умолчанию для работы как API «использовался последним». Служба запросов для последних [historyItems](../resources/projectrome-historyitem.md)и затем по запросу этих связанных действий. Действия будут упорядочены в соответствии с самыми последними **lastModified** на **historyItem**. Это означает, что действия без **historyItems** не будут включены в ответе. Разрешение UserActivity.ReadWrite.CreatedByApp будут также применены дополнительные фильтрации в ответ, чтобы возвращаются только действий, созданных приложением. В этом фильтрации на сервере может привести к пустой страницы Если пользователь является особенно active и другие приложения были созданы более последние действия. Для получения действия этого приложения, используйте свойство **nextLink** для разбиения по страницам.

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

Этот метод поддерживает некоторые [Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа. Поддерживаются следующие параметры запроса:

- для свойства **historyItems** навигации разверните $.
- Чтобы ограничить максимальное число элементов на страницах $top.
- $filter свойства **lastModifiedDateTime** для **действия** или **historyItems**, если были развернуты.

Ниже приведены некоторые примеры поддерживаемых запросов с кодировкой URL-адрес.

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

Не указывайте текста запроса.

## <a name="response"></a>Отклик

Успешно завершена, этот метод возвращает `200 OK` код ответа с помощью последние действия пользователя для приложения.

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

Ниже приведен пример отклика.

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "isCollection": true,
  "@odata.type": "microsoft.graph.activity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(userActivity)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/activities/recent?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
    "value": [{
        "@odata.type": "microsoft.graph.activity",
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
  "suppressions": [
    "Error: /api-reference/beta/api/projectrome-get-recent-activities.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
