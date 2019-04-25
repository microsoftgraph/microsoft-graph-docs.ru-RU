---
title: Создание или замена действия
description: Создание нового или замена существующего действия пользователя для вашего приложения. Если вы хотите создать действия пользователя и связанные с ним **historyitem** в одном запросе, вы можете использовать глубокую вставку.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: e0c010e7aefd16dca90d2b43d4f18f73d6c4f374
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538486"
---
# <a name="create-or-replace-an-activity"></a>Создание или замена действия

Создание нового или замена существующего действия пользователя для вашего приложения. Если вы хотите создать действия пользователя и связанные с ним **historyitem** в одном запросе, вы можете использовать глубокую [вставку](#example-2-deep-insert).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | UserActivity.ReadWrite.CreatedByApp |
| Делегированные (личная учетная запись Майкрософт) | UserActivity.ReadWrite.CreatedByApp |
| Для приложений                            | Не поддерживается.                      |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{appActivityId}
```

> **Примечание:** Аппактивитид в URL-АДРЕСе должен быть безопасным по URL-АДРЕСу (все символы, кроме зарезервированных символов RFC 2396, должны быть преобразованы в шестнадцатеричное представление), но исходный Аппактивитид не обязательно должен быть безопасным по URL-АДРЕСу.

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Тип   | Описание               |
|:--------------|:-------|:--------------------------|
| Authorization | string | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса добавьте представление объекта [Activity](../resources/projectrome-activity.md) в формате JSON.

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает `201 Created` код отклика, если действие было `200 OK` создано, или если действие было заменено.

## <a name="examples"></a>Примеры

### <a name="example-1-create-an-activity"></a>Пример 1: Создание действия

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
    "blockType": "ignored",
    "name": "upsert_activity"
} -->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/%2Farticle%3F12345
Content-type: application/json

{
  "appActivityId": "/article?12345",
  "activitySourceHost": "https://www.contoso.com",
  "userTimezone": "Africa/Casablanca",
  "appDisplayName": "Contoso, Ltd.",
  "activationUrl": "https://www.contoso.com/article?id=12345",
  "contentUrl": "https://www.contoso.com/article?id=12345",
  "fallbackUrl": "https://www.contoso.com/article?id=12345",
  "contentInfo": {
    "@context": "https://schema.org",
    "@type": "Article",
    "author": "Jennifer Booth",
    "name": "How to Tie a Reef Knot"
  },
  "visualElements": {
    "attribution": {
      "iconUrl": "https://www.contoso.com/icon",
      "alternateText": "Contoso, Ltd.",
      "addImageQuery": false
    },
    "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
    "backgroundColor": "#ff0000",
    "displayText": "Contoso How-To: How to Tie a Reef Knot",
    "content": {
      "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
      "type": "AdaptiveCard",
      "body": [
        {
          "type": "TextBlock",
          "text": "Contoso MainPage"
        }
      ]
    }
  }
}
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.userActivity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "activitySourceHost": "https://contoso.com",
  "createdDateTime": "2017-06-09T20:54:43.969Z",
  "lastModifiedDateTime": "2017-06-09T20:54:43.969Z",
  "id": "14332800362997268276",
  "appActivityId": "/article?12345",
  "status": "updated",
  "expirationDateTime": "2017-02-26T20:20:48.114Z",
  "visualElements": {
    "displayText": "Contoso How-To: How to Tie a Reef Knot",
    "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
    "attribution": {
      "iconUrl": "https://www.contoso.com/icon",
      "alternateText": "Contoso, Ltd.",
      "addImageQuery": "false"
    },
    "backgroundColor": "#ff0000",
    "content": {
      "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
      "type": "AdaptiveCard",
      "body": [
        {
          "type": "TextBlock",
          "text": "Contoso MainPage"
        }
      ]
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
    "author": "Jennifer Booth",
    "name": "How to Tie a Reef Knot"
  }
}
```

### <a name="example-2-deep-insert"></a>Пример 2: глубокая Вставка

В этом примере показано создание нового действия и элемента журнала для этого действия в одном запросе.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
    "blockType": "ignored",
    "name": "upsert_activity"
} -->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/%2Farticle%3F12345
Content-type: application/json

{
  "appActivityId": "/article?12345",
  "activitySourceHost": "https://www.contoso.com",
  "userTimezone": "Africa/Casablanca",
  "appDisplayName": "Contoso, Ltd.",
  "activationUrl": "https://www.contoso.com/article?id=12345",
  "contentUrl": "https://www.contoso.com/article?id=12345",
  "fallbackUrl": "https://www.contoso.com/article?id=12345",
  "contentInfo": {
    "@context": "https://schema.org",
    "@type": "Article",
    "author": "Jennifer Booth",
    "name": "How to Tie a Reef Knot"
  },
  "visualElements": {
    "attribution": {
      "iconUrl": "https://www.contoso.com/icon",
      "alternateText": "Contoso, Ltd.",
      "addImageQuery": "false"
    },
    "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
    "backgroundColor": "#ff0000",
    "displayText": "Contoso How-To: How to Tie a Reef Knot",
    "content": {
      "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
      "type": "AdaptiveCard",
      "body": [
        {
          "type": "TextBlock",
          "text": "Contoso MainPage"
        }
      ]
    }
  },
  "historyItems": [
    {
      "userTimezone": "Africa/Casablanca",
      "startedDateTime": "2018-02-26T20:54:04.345Z",
      "lastActiveDateTime": "2018-02-26T20:54:24.345Z"
    }
  ]
}
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.userActivity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "activitySourceHost": "https://contoso.com",
  "createdDateTime": "2017-06-09T20:54:43.969Z",
  "lastModifiedDateTime": "2017-06-09T20:54:43.969Z",
  "id": "14332800362997268276",
  "appActivityId": "/article?12345",
  "status": "updated",
  "expirationDateTime": "2017-02-26T20:20:48.114Z",
  "visualElements": {
    "displayText": "Contoso How-To: How to Tie a Reef Knot",
    "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
    "attribution": {
      "iconUrl": "https://www.contoso.com/icon",
      "alternateText": "Contoso, Ltd.",
      "addImageQuery": "false"
    },
    "backgroundColor": "#ff0000",
    "content": {
      "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
      "type": "AdaptiveCard",
      "body": [
        {
          "type": "TextBlock",
          "text": "Contoso MainPage"
        }
      ]
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
    "author": "Jennifer Booth",
    "name": "How to Tie a Reef Knot"
  },
  "historyItems": [
    {
      "status": "updated",
      "userTimezone": "Africa/Casablanca",
      "createdDateTime": "2018-04-12T21:42:42.495Z",
      "lastModifiedDateTime": "2018-04-12T21:42:42.495Z",
      "id": "61fc8f36-919f-4b73-89d4-1cb7b159d912",
      "startedDateTime": "2018-02-26T20:54:04.345Z",
      "lastActiveDateTime": "2018-02-26T20:54:24.345Z",
      "expirationDateTime": "2018-05-12T21:42:42.495Z",
      "activeDurationSeconds": 20
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Upsert activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
