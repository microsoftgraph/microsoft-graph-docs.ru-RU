---
title: Список участников чата
description: Получение списка участников чата.
author: anandjo
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e57a693adcf4714225ca67e58ba9a6bb836d0f44
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66442421"
---
# <a name="list-members-of-a-chat"></a>Список участников чата

Пространство имен: microsoft.graph

Перечисление всех [участников беседы](../resources/conversationmember.md) в [чате](../resources/chat.md).

> [!NOTE]
> Идентификаторы членства, возвращаемые сервером, должны рассматриваться как непрозрачные строки. Клиент не должен пытаться анализировать или делать какие-либо предположения об этих идентификаторах ресурсов.
>
> В дальнейшем результаты участия могут сопоставляться с пользователями из разных клиентов, как указано в отклике. Клиент не должен предполагать, что все участники относятся только к текущему клиенту.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|---------|-------------|
|Делегированные (рабочая или учебная учетная запись)| ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений| ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All |

> [!NOTE]
> Перед вызовом этого API с разрешениями приложения необходимо запросить доступ. Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{chat-id}/members
GET /users/{user-id | user-principal-name}/chats/{chat-id}/members
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.

## <a name="request-headers"></a>Заголовки запросов

| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {token}. Обязательный.  |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и список объектов [conversationMember](../resources/conversationmember.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_conversation_members_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/chats/19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_5031bb31-22c0-4f6f-9f73-91d34ab2b32d@unq.gbl.spaces/members
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-conversation-members-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-conversation-members-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-conversation-members-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-conversation-members-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-conversation-members-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/list-conversation-members-1-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример отклика.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')/chats('19%3A8b081ef6-4792-4def-b2c9-c363a1bf41d5_5031bb31-22c0-4f6f-9f73-91d34ab2b32d%40unq.gbl.spaces')/members",
   "@odata.count":3,
   "value":[
      {
         "@odata.type":"#microsoft.graph.aadUserConversationMember",
         "id":"8b081ef6-4792-4def-b2c9-c363a1bf41d5",
         "roles":[
            "owner"
         ],
         "displayName":"John Doe",
         "userId":"8b081ef6-4792-4def-b2c9-c363a1bf41d5",
         "email":null,
         "tenantId":"6e5147da-6a35-4275-b3f3-fc069456b6eb",
         "visibleHistoryStartDateTime":"2019-04-18T23:51:43.255Z"
      },
      {
         "@odata.type":"#microsoft.graph.aadUserConversationMember",
         "id":"2de87aaf-844d-4def-9dee-2c317f0be1b3",
         "roles":[
            "owner"
         ],
         "displayName":"Bart Hogan",
         "userId":"2de87aaf-844d-4def-9dee-2c317f0be1b3",
         "email":null,
         "tenantId":"6e5147da-6a35-4275-b3f3-fc069456b6eb",
         "visibleHistoryStartDateTime":"0001-01-01T00:00:00Z"
      },
      {
         "@odata.type":"#microsoft.graph.aadUserConversationMember",
         "id":"07ad17ad-ada5-4f1f-a650-7a963886a8a7",
         "roles":[
            "owner"
         ],
         "displayName":"Minna Pham",
         "userId":"07ad17ad-ada5-4f1f-a650-7a963886a8a7",
         "email":null,
         "tenantId":"6e5147da-6a35-4275-b3f3-fc069456b6eb",
         "visibleHistoryStartDateTime":"2019-04-18T23:51:43.255Z"
      }
   ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversation: member list",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


