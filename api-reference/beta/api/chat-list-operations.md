---
title: Список операций в чате
description: Извлечение операций в чате.
author: jecha
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fce94d591d6d1bde1e15f78674b18623ba80cb33
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031522"
---
# <a name="list-operations-on-a-chat"></a>Список операций в чате
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Список [всех Teams async,](../resources/teamsasyncoperation.md) которые запускались или запускались в указанном [чате.](../resources/chat.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)|
| :------------------------------------- | :--------------------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | Chat.ReadBasic, Chat.Read, Chat.ReadWrite|
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Приложение                            | ChatSettings.Read.Chat *, ChatSettings.ReadWrite.Chat*, Chat.Manage.Chat*, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All |

> **Примечание**. Разрешения, помеченные звездочкой (*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).

## <a name="http-request"></a>HTTP-запрос
<!-- { 
    "blockType": "ignored" 
} 
-->
``` http
GET /chats/{chat-id}/operations
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает `$filter` параметры `$select` запросов , и `$top` `$skip` [OData,](/graph/query-parameters) чтобы помочь настроить ответ.

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы возвращается код ответа и коллекция объектов `200 OK` [teamsAsyncOperation](../resources/teamsasyncoperation.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "list_chat_operations"
}
-->
``` http
GET https://graph.microsoft.com/beta/chats/19:c253a29b5f694b55a6baad8e83510af7@thread.v2/operations
```

---

### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAsyncOperation",
  "isCollection": true
}
-->
``` http
HTTP/1.1 202 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3Ac253a29b5f694b55a6baad8e83510af7%40thread.v2')/operations",
    "@odata.count": 1,
    "value": [
        {
            "id": "2432b57b-0abd-43db-aa7b-16eadd115d34-e88ae9aa-887e-4972-ac3e-bd578e38232e-cf58835e-43f0-4fc1-825e-5de55630e7e4",
            "operationType": "createChat",
            "createdDateTime": "2021-05-27T21:23:41.9085453Z",
            "status": "succeeded",
            "lastActionDateTime": "2021-05-27T21:23:45.1899277Z",
            "attemptsCount": 1,
            "targetResourceId": "19:c253a29b5f694b55a6baad8e83510af7@thread.v2",
            "targetResourceLocation": "/chats('19:c253a29b5f694b55a6baad8e83510af7@thread.v2')",
            "values": "{\"appIds\":[\"1542629c-01b3-4a6d-8f76-1938b779e48d\"]}",
            "error": null
        }
    ]
}
```
