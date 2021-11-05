---
title: 'чат: markChatReadForUser'
description: Пометить чат в качестве чтения до текущего времени или последнего сообщения, полученного или отправленного.
author: sweta-thapliyal
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d20031641befc87ef198544798adc397560b3982
ms.sourcegitcommit: f9e71d3b8a54a98c282ef49783babe5698300c06
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2021
ms.locfileid: "60793988"
---
# <a name="chat-markchatreadforuser"></a>чат: markChatReadForUser
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Пометить чат](../resources/chat.md) как чтение для пользователя.

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
POST /chats/{chat-id}/markChatReadForUser
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON параметров.

В следующей таблице указаны параметры, которые можно использовать с этим действием.

|Параметр|Тип|Описание|
|:---|:---|:---|
|tenantId|String|ID клиента пользователя.|
|пользователь|[teamworkUserIdentity](../resources/teamworkuseridentity.md)|Пользователь для чтения чата.|

## <a name="response"></a>Ответ

В случае успешного выполнения это действие возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "chat_markchatreadforuser"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats/19:7d898072-792c-4006-bb10-5ca9f2590649_8ea0e38b-efb3-4757-924a-5f94061cf8c2@unq.gbl.spaces/markChatReadForUser
Content-Type: application/json
Content-length: 106

{
 "user": {
    "id" : "d864e79f-a516-4d0f-9fee-0eeb4d61fdc2"
  },
  "tenantId": "2a690434-97d9-4eed-83a6-f5f13600199a"
}
```


### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

