---
title: 'чат: markChatUnreadForUser'
description: Пометить чат как непрочитанные для пользователя.
author: sweta-thapliyal
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f107f67d388ead1876a0478b1a1a5840bff28e03
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890619"
---
# <a name="chat-markchatunreadforuser"></a>чат: markChatUnreadForUser
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Пометить чат](../resources/chat.md) как непрочитанные для пользователя.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Chat.ReadWrite|
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /chats/{chat-id}/markChatUnreadForUser
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Основной текст запроса
В теле запроса поставляем представление JSON параметров.

В следующей таблице указаны параметры, которые можно использовать с этим действием.

|Параметр|Тип|Описание|
|:---|:---|:---|
|lastMessageReadDateTime|DateTimeOffset|Timestamp, который указывает время, по истечении которого все отправленные или полученные сообщения должны быть помечены как непрочитанные.|
|tenantId|String|ID клиента пользователя.|
|пользователь|[teamworkUserIdentity](../resources/teamworkuseridentity.md)|Пользователь, чтобы отчитать чат для.|

> **Примечание.** **lastMessageReadDateTime** является необязательным в запросе. Если не упомянуть, последнее сообщение будет помечено как непрочитанные.

## <a name="response"></a>Ответ

В случае успешного выполнения это действие возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chat_markchatunreadforuser"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats/19:7d898072-792c-4006-bb10-5ca9f2590649_8ea0e38b-efb3-4757-924a-5f94061cf8c2@unq.gbl.spaces/markChatUnreadForUser
Content-Type: application/json
Content-length: 158

{
  "user": {
    "id" : "d864e79f-a516-4d0f-9fee-0eeb4d61fdc2"
  },
  "tenantId": "2a690434-97d9-4eed-83a6-f5f13600199a",
  "lastMessageReadDateTime": "2021-05-27T22:13:01.577Z"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chat-markchatunreadforuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chat-markchatunreadforuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chat-markchatunreadforuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chat-markchatunreadforuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

