---
title: 'message: forward'
description: 'Переслать сообщение, добавить комментарий или изменить любые обновляемые свойства  '
ms.openlocfilehash: 3edb96a90c99f1bc9eb2d8499e9cda83774a7ab3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082418"
---
# <a name="message-forward"></a>message: forward

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Переслать сообщение, добавить комментарий или изменить любые обновляемые свойства  
все в одной **переадресовывать** вызова. Сообщение сохраняется в папке «Отправленные».

Кроме того можно первого [создания переслать сообщение черновиков](../api/message-createforward.md) добавить примечание или обновить все свойства сообщений, а затем [Отправить](../api/message-send.md) сообщение черновиков.

**Примечание**

- Можно указать комментарий или свойству **body** `message` параметр. Указание оба возвратит ошибку HTTP 400 Bad Request.
- Необходимо указать либо `toRecipients` параметр или свойство **toRecipients** `message` параметр. Указание оба или указан ни один из них возвратит ошибку HTTP 400 Bad Request.

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
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |
| Content-Type | string  | Характер данных в теле объекта. Обязательный. |

## <a name="request-body"></a>Текст запроса
В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр    | Тип   |Описание|
|:---------------|:--------|:----------|
|comment|String|Добавляемый комментарий. Может быть пустой строкой.|
|toRecipients|Коллекция [recipient](../resources/recipient.md)|Список получателей.|
|message|[message](../resources/message.md)|Любой доступный свойства для обновления в ответное сообщение.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.

## <a name="example"></a>Пример
В следующем примере задается свойство **isDeliveryReceiptRequested** имеет значение true, добавляется комментарий и перенаправляет сообщение.
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaLAAA=/forward
Content-Type: application/json

{
  "message":{  
    "isDeliveryReceiptRequested": true,
    "toRecipients":[
      {
        "emailAddress": {
          "address":"danas@contoso.onmicrosoft.com",
          "name":"Dana Swope"
        }
      }
     ]
  },
  "comment": "Dana, just want to make sure you get this." 
}
```

##### <a name="response"></a>Ответ
Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
