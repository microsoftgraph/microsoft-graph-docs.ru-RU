---
title: Get teamsAsyncOperation
description: Сведения о teamsAsyncOperation.
author: jecha
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bfbb9f7face458382af90f9899d76461a336871b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118158"
---
# <a name="get-teamsasyncoperation"></a>Get teamsAsyncOperation
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите указанную операцию [Teams async,](../resources/teamsasyncoperation.md) которая запущена или запущена на определенном ресурсе.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

Следующие разрешения для получения операции в чате:

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
GET /chats/{chat-id}/operations/{operation-id}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает параметр `$select` [запроса OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Тело запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы возвращается код ответа и объект `200 OK` [teamsAsyncOperation](../resources/teamsasyncoperation.md) в тексте ответа.

## <a name="example-get-operation-on-chat"></a>Пример. Получить операцию в чате

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chat_operation"
}
-->
``` http
GET https://graph.microsoft.com/beta/chats/19:c253a29b5f694b55a6baad8e83510af7@thread.v2/operations/2432b57b-0abd-43db-aa7b-16eadd115d34-e88ae9aa-887e-4972-ac3e-bd578e38232e-cf58835e-43f0-4fc1-825e-5de55630e7e4
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chat-operation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chat-operation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chat-operation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chat-operation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-chat-operation-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-chat-operation-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsAsyncOperation"
}
-->
``` http
HTTP/1.1 202 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3Ac253a29b5f694b55a6baad8e83510af7%40thread.v2')/operations/$entity",
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
```
