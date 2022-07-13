---
title: 'chatMessage: undoSoftDelete'
description: Отмена удаления одного сообщения или ответа на сообщение в канале или чате.
author: Ramjot Singh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.localizationpriority: medium
ms.openlocfilehash: 353b41cee2ab489f88eaec8b5a6d6f3d19560722
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2022
ms.locfileid: "66768385"
---
# <a name="chatmessage-undosoftdelete"></a>chatMessage: undoSoftDelete

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Отмените обратимое удаление одного [сообщения](../resources/chatmessage.md) или ответа на [](../resources/chatmessage.md) сообщение в [канале или](../resources/channel.md) [чате](../resources/chat.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

### <a name="permissions-for-channel"></a>Разрешения для канала

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)| ChannelMessage.ReadWrite |
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается |
|Приложение| Не поддерживается |

> **Примечание**. Разрешения, отмеченные **, поддерживаются только для обратной совместимости. Рекомендуется обновить решения, чтобы использовать другое разрешение, указанное в предыдущей таблице, и избегать использования этих разрешений в будущем.

### <a name="permissions-for-chat"></a>Разрешения для чата

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)| ChatMessage.ReadWrite |
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается |
|Приложение| Не поддерживается |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{userId}/chats/{chatsId}/messages/{chatMessageId}/undoSoftDelete
POST /teams/{teamsId}/channels/{channelId}/messages/{chatMessageId}/undoSoftDelete
POST /teams/{teamId}/channels/{channelId}/messages/{messageId}/replies/{replyId}/undoSoftDelete
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения это действие возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="example-1-undo-soft-deletion-of-a-message-in-a-chat"></a>Пример 1. Отмена обратимого удаления сообщения в чате

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "chatmessagethis-undosoftdelete1"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/8f98f01d-1a73-401a-b9e9-9fd1e6f5e5ap/chats/19:22273db3497f4b32bue61f6e82be21c5@thread.tacv2/messages/1649864053377/undoSoftDelete
```

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response"
} -->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-undo-soft-deletion-of-a-message-in-a-channel"></a>Пример 2. Отмена обратимого удаления сообщения в канале

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "chatmessagethis2undosoftdelete2"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/172b0cce-e65d-44ce-9a49-91d9f2e8593a/channels/19:22273db3497f4b32bue61f6e82be21c5@thread.tacv2/messages/1649864053377/undoSoftDelete
```

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response"
} -->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-undo-soft-deletion-of-a-message-of-a-reply-in-a-channel"></a>Пример 3. Отмена обратимого удаления сообщения ответа в канале

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "chatmessagethis-undosoftdelete3"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/172b0cce-e65d-44ce-9a49-91d9f2e8593a/channels/19:22273db3497f4b32bue61f6e82be21c5@thread.tacv2/messages/1649864053377/undoSoftDelete
```

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response"
} -->

``` http
HTTP/1.1 204 No Content
```
