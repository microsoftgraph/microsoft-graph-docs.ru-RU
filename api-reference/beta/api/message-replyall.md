---
title: 'message: replyAll'
description: Ответьте всем получателям сообщения в формате JSON или MIME.
author: abheek-das
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0ddb81baaffa9a309e1613d7b1b91465c7f1be87
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341099"
---
# <a name="message-replyall"></a>message: replyAll

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ответьте всем получателям [сообщения в](../resources/message.md) формате JSON или MIME.

При использовании формата JSON:
- Укажите комментарий или **свойство** тела параметра `message` . При указании обоих возвращается ошибка http 400 Bad Request.
- Если исходное сообщение указывает получателя в свойстве **replyTo**, в формате интернет-сообщений ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), отправьте ответ получателям в **replyTo**, а не получателю в свойстве.

При использовании формата MIME:
- Укажите соответствующие [заголовки сообщений Интернета](https://tools.ietf.org/html/rfc2076) и [содержимое MIME](https://tools.ietf.org/html/rfc2045), а также закодируйте их в формате **Base64** в тексте запроса.
- Добавьте все вложения и свойства S/MIME в содержимое MIME.

Этот метод сохраняет сообщение в папке **Отправленные**.

Кроме того, [создайте черновик](../api/message-createreplyall.md) для ответа на сообщение и [отправьте его](../api/message-send.md) позже.

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
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {token}. Обязательно|
| Content-Type | string  | Характер данных в теле объекта. Обязательно <br/> Использование `application/json` объекта JSON и контента `text/plain` MIME |

## <a name="request-body"></a>Текст запроса
При использовании формата JSON укажите объект JSON со следующими параметрами.

| Параметр    | Тип   |Описание|
|:---------------|:--------|:----------|
|comment|String|Добавляемый комментарий. Может быть пустой строкой.|
|сообщение|[message](../resources/message.md)|Любые свойства, которые можно записать для обновления в ответном сообщении.|

При указании тела в формате MIME укажите содержимое MIME с применимыми заглавными сообщениями в Интернете, все закодированные в **формате base64** в тексте запроса. Этот метод загружает отправитель и всех получателей исходного сообщения в качестве получателей нового сообщения.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.

Если текст запроса содержит неправильно отформатированное содержимое MIME, этот метод возвращает `400 Bad request` и следующее сообщение об ошибке: "Недопустимая строка Base 64 для содержимого MIME".

## <a name="examples"></a>Примеры
### <a name="example-1-reply-all-to-a-message-in-json-format"></a>Пример 1. Ответ на сообщение в формате JSON
В следующем примере содержится комментарий и добавляется вложение в сообщение для всех ответов.
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_replyall"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaKAAA=/replyAll
Content-Type: application/json

{
    "message":{
      "attachments": [ 
        { 
          "@odata.type": "#microsoft.graph.fileAttachment", 
          "name": "guidelines.txt", 
          "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk=" 
        } 
      ]
    },
    "comment": "Please take a look at the attached guidelines before you decide on the name." 
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-replyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-replyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-replyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-replyall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/message-replyall-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/message-replyall-powershell-snippets.md)]
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

### <a name="example-2-reply-all-to-a-message-in-mime-format"></a>Пример 2. Ответ на сообщение в формате MIME
##### <a name="request"></a>Запрос

<!-- {
  "blockType": "ignored",
  "name": "message_replyAll_mime_beta"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaLAAA=/replyAll
Content-Type: text/plain

RnJvbTogQWxleCBXaWxiZXIgPEFsZXhXQGNvbnRvc28uY29tPgpUbzogTWVnYW4gQm93ZW4gPE1l
Z2FuQkBjb250b3NvLmNvbT4KU3ViamVjdDogSW50ZXJuYWwgUmVzdW1lIFN1Ym1pc3Npb246IFNh
bGVzIEFzc29jaWF0ZQpUaHJlYWQtVG9waWM...

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
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


