---
title: 'сообщение: отказ от подписки'
description: Отправка запроса электронной почты от имени вошедшего пользователя для отказа от подписки на список рассылки электронной почты. Использует информацию в `List-Unsubscribe` заголовке.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 87cfe7616319f52561bec46d711770081bf1a32e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879389"
---
# <a name="message-unsubscribe"></a>сообщение: отказ от подписки

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Отправка запроса электронной почты от имени вошедшего пользователя для отказа от подписки на список рассылки электронной почты. Использует информацию в `List-Unsubscribe` заголовке.

Отправители сообщений могут использовать списки рассылки в удобном для пользователя виде, включая возможность отказаться от получателей. Это можно сделать, указав `List-Unsubscribe` заголовок в каждом сообщении, описанном в [документе RFC – 2369](https://www.faqs.org/rfcs/rfc2369.html).

**Note (Примечание** ) В частности, чтобы действие **отмены подписки** работало, отправителю необходимо указать и не `mailto:` указывать сведения об отмене подписки на основе URL-адреса.

При задании этого заголовка `true`для свойства **unsubscribeEnabled** экземпляра [Message](../resources/message.md) также будет задано значение, а свойству **unsubscribeData** — данные заголовка.

Если свойство **unsubscribeEnabled** сообщения имеет `true`значение, можно использовать действие **Отменить подписку** , чтобы отменить подписку на пользователя из похожих будущих сообщений, которыми управляет отправитель сообщения.

При успешном завершении операции **отмены подписки** сообщение перемещается в папку " **Удаленные** ". Фактическим исключением пользователя из будущей рассылки почты управляет отправитель.

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
POST /users/{id | userPrincipalName}/messages/{id}/unsubscribe
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Тело запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`. В тексте отклика не возвращается никаких данных.

## <a name="example"></a>Пример
Ниже приведен пример вызова этого API.
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_unsubscribe"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/{id}/unsubscribe
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-unsubscribe-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-unsubscribe-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Цель — C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-unsubscribe-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-unsubscribe-java-snippets.md)]
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: unsubscribe",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
