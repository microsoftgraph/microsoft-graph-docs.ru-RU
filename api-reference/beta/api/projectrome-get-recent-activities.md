---
title: Получение последних действий пользователя
description: " API. Служба будет запрашивать последние historyItems, а затем извлекать эти связанные действия. Действия будут отсортированы в соответствии с последним **элементом lastModified** в **historyItem**. Это означает, что действия без **historyItems** не будут включены в ответ. Разрешение UserActivity.ReadWrite.CreatedByApp также применяет дополнительную фильтрацию к ответу, чтобы возвращались только действия, созданные приложением. Такая фильтрация на стороне сервера может привести к пустым страницам, если пользователь особенно активен и другие приложения создали более последние действия. Чтобы получить действия приложения, используйте свойство **nextLink** для разбиения на страницы."
ms.localizationpriority: medium
ms.prod: project-rome
doc_type: apiPageType
author: ailae
ms.openlocfilehash: 2ab0089a4653b2762fec5e1ae47ebce1f533ac54
ms.sourcegitcommit: 423e698a580c3b902f2816b0216ab9d5b91e6d20
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2022
ms.locfileid: "66034539"
---
# <a name="get-recent-user-activities"></a>Получение последних действий пользователя

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение последних действий для заданного пользователя. Эта функция OData имеет некоторые стандартные функции, которые позволяют работать как "недавно использовавшихся" API. Служба будет запрашивать последние [historyItems](../resources/projectrome-historyitem.md), а затем извлекать эти связанные действия. Действия будут отсортированы в соответствии с последним **элементом lastModified** в **historyItem**. Это означает, что действия без **historyItems** не будут включены в ответ. Разрешение UserActivity.ReadWrite.CreatedByApp также применяет дополнительную фильтрацию к ответу, чтобы возвращались только действия, созданные приложением. Такая фильтрация на стороне сервера может привести к пустым страницам, если пользователь особенно активен и другие приложения создали более последние действия. Чтобы получить действия приложения, используйте свойство **nextLink** для разбиения на страницы.

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

Этот метод поддерживает некоторые [параметры запроса OData](/graph/query-parameters) для настройки ответа. Поддерживаются следующие параметры запроса:

- $expand для свойства **навигации historyItems** .
- $top ограничить максимальное количество элементов на страницах.
- $filter свойства **lastModifiedDateTime** для **действий** или **historyItems**, если они развернуты.

Ниже приведены некоторые примеры поддерживаемых запросов с кодированием URL-адресов.

```http
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a>Заголовки запросов

|Имя | Тип | Описание|
|:----|:-----|:-----------|
|Authorization | string | Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `200 OK` отклика с последними действиями пользователя для приложения.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "ignored",
  "name": "get_recent_activities"
}-->

```http
GET https://graph.microsoft.com/beta/me/activities/recent
```

### <a name="response"></a>Отклик

Ниже приведен пример отклика.

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.activity",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(userActivity)",
   "@odata.nextLink":"https://graph.microsoft.com/beta/me/activities/recent?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
   "value":[
      {
         "@odata.type":"#microsoft.graph.activity",
         "activitySourceHost":"https://www.contoso.com",
         "createdDateTime":"2018-02-26T18:34:29.592Z",
         "lastModifiedDateTime":"2018-02-26T18:34:29.607Z",
         "id":"5347642601316252694",
         "appActivityId":"/article?12345",
         "visualElements":{
            "attribution":{
               "iconUrl":"https://www.contoso.com/icon",
               "alternateText":"Contoso, Ltd.",
               "addImageQuery":"false"
            },
            "displayText":"Contoso How-To: How to Tie a Reef Knot",
            "description":"How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
            "backgroundColor":"#ff0000",
            "content":{
               "$schema":"https://adaptivecards.io/schemas/adaptive-card.json",
               "type":"AdaptiveCard",
               "body":[
                  {
                     "type":"TextBlock",
                     "text":"Contoso MainPage"
                  }
               ]
            }
         },
         "activationUrl":"https://www.contoso.com/article?id=12345",
         "appDisplayName":"Contoso, Ltd.",
         "userTimezone":"Africa/Casablanca",
         "fallbackUrl":"https://www.contoso.com/article?id=12345",
         "contentUrl":"https://www.contoso.com/article?id=12345",
         "contentInfo":{
            "@context":"https://schema.org",
            "@type":"Article",
            "author":"John Doe",
            "name":"How to Tie a Reef Knot"
         },
         "expirationDateTime":"2018-03-28T18:34:29.607Z",
         "status":"updated"
      }
   ]
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
