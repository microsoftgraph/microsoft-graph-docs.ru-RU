---
title: 'message: reply'
description: Ответ отправилю сообщения в формате JSON или MIME.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e5a9cab87389f41c795268a1d7964a7d8e987269
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870502"
---
# <a name="message-reply"></a>message: reply

Пространство имен: microsoft.graph.

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ответ отправилю сообщения [в](../resources/message.md) формате JSON или MIME.

При использовании формата JSON:
- Укажите комментарий или **свойство** тела `message` параметра. При указании обоих возвращается ошибка http 400 Bad Request.
- Если исходное сообщение указывает получателя в свойстве **replyTo,** в формате интернет-сообщений [(RFC 2822),](https://www.rfc-editor.org/info/rfc2822)отправьте ответ получателям в **replyTo,** а не получателю из **свойства.**

При использовании формата MIME:
- Укажите соответствующие [заголовки сообщений Интернета](https://tools.ietf.org/html/rfc2076) и [содержимое MIME](https://tools.ietf.org/html/rfc2045), а также закодируйте их в формате **Base64** в тексте запроса.
- Добавьте все вложения и свойства S/MIME в содержимое MIME.

Этот метод сохраняет сообщение в папке **Отправленные**.

Кроме того, [создайте черновик](../api/message-createreply.md)для ответа на сообщение и [отправьте его](../api/message-send.md) позже.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Mail.Send    |
|Делегированные (личная учетная запись Майкрософт) | Mail.Send    |
|Для приложений | Mail.Send |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {token}. Обязательный |
| Content-Type | string  | Характер данных в теле объекта. Обязательный <br/> Использование `application/json` объекта JSON и `text/plain` контента MIME |

## <a name="request-body"></a>Тело запроса
При использовании формата JSON включаем объект JSON со следующими параметрами.

| Параметр    | Тип   |Описание|
|:---------------|:--------|:----------|
|comment|String|Добавляемый комментарий. Может быть пустой строкой.|
|message|[message](../resources/message.md) | Любые свойства, которые можно записать для обновления в ответном сообщении.|

При указании тела в формате MIME укажите содержимое MIME с применимыми заглавными сообщениями в Интернете, все закодированные в **формате base64** в тексте запроса. Этот метод использует отправитель исходного сообщения в качестве получателя.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.

Если текст запроса содержит неправильно отформатированное содержимое MIME, этот метод возвращает `400 Bad request` и следующее сообщение об ошибке: "Недопустимая строка Base 64 для содержимого MIME".

## <a name="examples"></a>Примеры
### <a name="example-1-reply-to-a-message-in-json-format"></a>Пример 1. Ответ на сообщение в формате JSON
В следующем примере содержится комментарий и добавляется получатель в ответное сообщение.
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "message_reply_beta",
  "sampleKeys": ["AAMkADA1MTAAAAqldOAAA="]
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAAqldOAAA=/reply
Content-Type: application/json

{
  "message":{  
    "toRecipients":[
      {
        "emailAddress": {
          "address":"samanthab@contoso.onmicrosoft.com",
          "name":"Samantha Booth"
        }
      },
      {
        "emailAddress":{
          "address":"randiw@contoso.onmicrosoft.com",
          "name":"Randi Welch"
        }
      }
     ]
  },
  "comment": "Samantha, Randi, would you name the group please?" 
}

```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-reply-beta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-reply-beta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-reply-beta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-reply-beta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик
Ниже приведен пример отклика.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-reply-to-a-message-in-mime-format"></a>Пример 2. Ответ на сообщение в формате MIME
##### <a name="request"></a>Запрос

<!-- {
  "blockType": "ignored",
  "name": "message_reply_mime_beta"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADA1MTAAAAqldOAAA=/reply
Content-Type: text/plain

UmVjZWl2ZWQ6IGZyb20gY29udG9zby5jb20gKDEwLjE5NC4yNDEuMTk3KSBieSAKY29udG9zby5jb20gKDEwLjE5NC4yNDEuMTk3KSB3aXRoIE1pY3Jvc29mdCAKU01UUCBTZXJ2ZXIgKHZlcnNpb249VExTMV8yLCAKY2lwaGVyPVRMU19FQ0RIRV9SU0FfV0lUSF9BRVNfMjU2X0NCQ19TSEEzODRfUDI1NikgaW

```

##### <a name="response"></a>Отклик
Ниже приведен пример отклика.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

Если текст запроса содержит неправильно отформатированное содержимое MIME, этот метод возвращает следующее сообщение об ошибке.

<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 400 Bad Request
Content-type: application/json

{
    "error": {
        "code": "ErrorMimeContentInvalidBase64String",
        "message": "Invalid base64 string for MIME content."
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
