---
title: Обновление чата
description: Обновление свойств объекта чата.
author: bhartono
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b0b7fcccb3de2716aa30fdeb577ed3dc31ca99e6
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753935"
---
# <a name="update-chat"></a>Обновление чата
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [чата.](../resources/chat.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Chat.ReadWrite|
|Делегированное (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /chats/{chat-id}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса укажу представление объекта [чата](../resources/chat.md) в JSON.

В следующей таблице показаны свойства, которые можно использовать с этим действием.

|Свойство|Тип|Описание|
|:---|:---|:---|
|topic|String|Название чата. Это можно сделать только для чата со значением **chatType.** `group`|


## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код и обновленный ресурс `200 OK response` **чата** в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chat"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/chats/19:1c5b01696d2e4a179c292bc9cf04e63b@thread.v2
Content-Type: application/json

{
    "topic": "Group chat title update",
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats/$entity",
    "id": "19:1c5b01696d2e4a179c292bc9cf04e63b@thread.v2",
    "topic": "Group chat title update",
    "createdDateTime": "2020-12-04T23:11:16.175Z",
    "lastUpdatedDateTime": "2020-12-04T23:12:19.943Z",
    "chatType": "group"
}
```

