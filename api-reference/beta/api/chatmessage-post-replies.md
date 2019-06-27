---
title: Создание ответа chatMessage в канале
description: Создает новый объект chatMessage в ответе на существующий объект chatMessage.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5db3c6932b7272e7a2101390303713c69e00d70b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261385"
---
# <a name="create-chatmessage-reply-in-a-channel"></a>Создание ответа chatMessage в канале

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создает новый объект [chatMessage](../resources/chatmessage.md) в ответе на существующий объект [chatMessage](../resources/chatmessage.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Chat. ReadWrite |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /chats/{id}/messages/{id}/replies
POST /users/{id}/chats/{id}/messages/{id}/replies
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Bearer {code} |

## <a name="request-body"></a>Текст запроса

В тексте запроса добавьте представление объекта [chatMessage](../resources/chatmessage.md) в формате JSON.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [chatMessage](../resources/chatmessage.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_chatmessage"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}/replies
Content-type: application/json

{
  "body": {
     "content" : "Hello world"
  }
}
```

### <a name="response"></a>Отклик

Ниже приведен пример ответа.

> [!NOTE]
> Объект Response, показанный здесь, может быть укорочен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "replyToId": "replyToId-value",
  "from": {
    "application": null,
    "device": null,
    "user": {
      "id": "87ea812c-8816-40e9-b770-5c165fa31397",
      "displayName": "Test User"
    }
  },
  "messageType": "message",
  "body": {
     "content": "Hello world",
     "contentType": "text"
  }
}
```
#### <a name="sdk-sample-code"></a>Пример кода SDK

# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/create_chatmessage_from_chatmessage-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_chatmessage_from_chatmessage-Javascript-snippets.md)]
# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_chatmessage_from_chatmessage-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create chatMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chatmessage-post-replies.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/chatmessage-post-replies.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/chatmessage-post-replies.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)"
  ]
}-->
