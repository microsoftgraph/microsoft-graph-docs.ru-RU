---
title: Закрепление сообщения в чате
description: Закрепите сообщение чата в указанном чате.
author: sumanac
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8e1324113f305ea7fbb5a671c61321fab12ef6c9
ms.sourcegitcommit: 10b45b3e666bf6b438803885128bc2f0fa2fa994
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/24/2022
ms.locfileid: "65653648"
---
# <a name="pin-a-message-in-a-chat"></a>Закрепление сообщения в чате
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Закрепите сообщение чата в указанном [чате](../resources/chat.md). Этот API не может создать новый чат; Чтобы закрепить сообщение [чата](chat-list.md) , необходимо использовать метод чатов списка для получения идентификатора существующего чата.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
| Делегированные (рабочая или учебная учетная запись)     | ChatMessage.Send, Chat.ReadWrite |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Приложение                            | Chat.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /chats/{chat-Id}/pinnedMessages
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
Текст запроса должен содержать идентификатор сообщения чата.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `201 Created` отклика и объект [pinnedChatMessageInfo](../resources/pinnedchatmessageinfo.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "create_pinnedchatmessageinfo_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/pinnedMessages
Content-Type: application/json
Content-length: 63

{
   "message@odata.bind":"https://graph.microsoft.com/beta/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages/1616964509832"
}
```


### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.pinnedChatMessageInfo"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.pinnedChatMessageInfo",
  "id": "1616964509832"
}
```
