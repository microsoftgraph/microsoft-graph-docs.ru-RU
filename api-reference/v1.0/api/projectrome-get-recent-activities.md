---
title: Получать последние действия пользователя
description: " API. Служба запрашивает последние historyItems и затем вытягивает связанные действия. Действия будут сортироваться в соответствии с последним **lastModified** на **historyItem**. Это означает, что действия без **historyItems** не будут включены в ответ. Разрешение UserActivity.ReadWrite.CreatedByApp также применяет дополнительную фильтрацию к ответу, чтобы возвращались только действия, созданные вашим приложением. Это фильтрация на стороне сервера может привести к пустым страницам, если пользователь особенно активен, а другие приложения создали более последние действия. Чтобы получить действия приложения, используйте свойство **nextLink** для пагинации."
ms.localizationpriority: medium
ms.prod: project-rome
author: ailae
doc_type: apiPageType
ms.openlocfilehash: d4640a54c00caaa8e0ecb10a31429afad613fb05
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61016204"
---
# <a name="get-recent-user-activities"></a>Получать последние действия пользователя

Пространство имен: microsoft.graph

Получите последние действия для данного пользователя. Эта функция OData имеет некоторые действия по умолчанию, включаемые, чтобы заставить ее работать как API "последнего времени". Служба запрашивает последние [historyItems,](../resources/projectrome-historyitem.md)а затем вытягивает связанные действия. Действия будут сортироваться в соответствии с последним **lastModified** на **historyItem**. Это означает, что действия без **historyItems** не будут включены в ответ. Разрешение UserActivity.ReadWrite.CreatedByApp также применяет дополнительную фильтрацию к ответу, чтобы возвращались только действия, созданные вашим приложением. Это фильтрация на стороне сервера может привести к пустым страницам, если пользователь особенно активен, а другие приложения создали более последние действия. Чтобы получить действия приложения, используйте свойство **nextLink** для пагинации.

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

Этот метод поддерживает некоторые [параметры запроса OData для](/graph/query-parameters) настройки ответа. Поддерживаются следующие параметры запроса:

- $expand для свойства **навигации historyItems.**
- $top ограничить максимальное количество элементов на страницах.
- $filter в **свойстве lastModifiedDateTime** для  действий или **historyItems,** если они расширены.

Ниже приводится несколько примеров поддерживаемых запросов с кодией URL-адресов.

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

Не укажите тело запроса.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа с последними действиями пользователя `200 OK` для приложения.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_recent_activities"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/activities/recent
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-recent-activities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-recent-activities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-recent-activities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-recent-activities-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-recent-activities-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userActivity)"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(userActivity)",
   "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/activities/recent?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
   "value":[
      {
         "@odata.type":"#microsoft.graph.userActivity",
         "activitySourceHost":"https://www.contoso.com",
         "createdDateTime":"2018-02-26T18:34:29.592Z",
         "lastModifiedDateTime":"2018-02-26T18:34:29.607Z",
         "id":"5347642601316252694",
         "appActivityId":"/article?12345",
         "visualElements":{
            "attribution":{
               "iconUrl":"https://www.contoso.com/icon",
               "alternateText":"Contoso, Ltd.",
               "addImageQuery":false
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
<!-- {
  "type": "#page.annotation",
  "description": "Get recent activities",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
  ],
  "tocPath": ""
}-->
