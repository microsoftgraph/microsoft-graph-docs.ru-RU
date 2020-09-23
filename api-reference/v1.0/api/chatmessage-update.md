---
title: Обновление chatMessage
description: Обновление свойства Полицивиолатион объекта chatMessage.
author: laujan
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b36f02ec2193bfc1eda1706265fa1392b04a4e70
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223963"
---
# <a name="update-chatmessage"></a>Обновление chatMessage

Обновление объекта [chatMessage](../resources/chatMessage.md) . Можно обновить только свойство **полицивиолатион** элемента **chatMessage** .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Не поддерживается.    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | Chat. Упдатеполицивиолатион. ALL для сообщения чата.</br>Чаннелмессаже. Упдатеполицивиолатион. ALL для сообщения канала. |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/(team-id)/channels/{channel-id}/chatMessages/{message-id}
PATCH /users/(user-id)/chats/{chatThread-id}/chatMessages/{message-id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:-----------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |
| Content-Type | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса добавьте представление объекта [chatMessage](../resources/chatMessage.md) в формате JSON, указав только свойство **полицивиолатион** .

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` отклик.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса на обновление свойства **полицивиолатион** сообщения канала Microsoft Teams.

<!-- {
  "blockType": "request",
  "name": "chatMessage.PatchPolicyViolation.All"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/teams/e1234567-e123-4276-55555-6232b0e3a89a/channels/a7654321-e321-0000-0000-123b0e3a00a/messages/19%3Aa21b0b0c05194ebc9e30000000000f61%40thread.skype
Content-Type: application/json
Content-Length: 248

{
  "policyViolation": {
    "policyTip": {
      "generalText" : "This item has been blocked by the administrator.",
      "complianceUrl" : "https://contoso.com/dlp-policy-page",
      "matchedConditionDescriptions" : ["Credit Card Number"]
    },
    "verdictDetails" : "AllowOverrideWithoutJustification,AllowFalsePositiveOverride",
    "dlpAction" : "BlockAccess"
  }
}
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a>Отклик

Ниже приведен пример отклика.

<!-- {
  "blockType": "response",
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatMessage.UpdatePolicyViolation.All",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
