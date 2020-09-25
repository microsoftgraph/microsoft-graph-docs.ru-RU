---
title: Список участников
description: Получение conversationMembers группы.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 43b487dfdcccec53ace184d4cbedda7992ad1f3e
ms.sourcegitcommit: 3c0fa2d13ede0fdfa66d966d4ec32cb468c3befa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/25/2020
ms.locfileid: "48273650"
---
# <a name="list-members"></a>Список участников
Пространство имен: microsoft.graph

Получение [conversationMember](../resources/conversationmember.md) [группы](../resources/team.md).

>Примечание. в настоящее время данный API не поддерживает разбивку на страницы, поэтому если в одном запросе помещено слишком много участников, вы не сможете получить доступ ко всем участникам.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|TeamMember.Read.All, TeamMember.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение|TeamMember.Read.All, TeamMember.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teams/{teamsId}/members
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает некоторые параметры запросов OData для настройки отклика. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [conversationMember](../resources/conversationmember.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversationmember"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/teams/{teamsId}/members
```
# <a name="c"></a>[C#](#tab/csharp)

[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)

[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)

[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Отклик
**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "get_conversationmember",
  "@odata.type": "collection(microsoft.graph.aadUserConversationMember)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members",
    "@odata.count": 2,
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
            "roles": [],
            "displayName": "Adele Vance",
            "userId": "73761f06-2ac9-469c-9f10-279a8cc267f9",
            "email": "AdeleV@M365x987948.OnMicrosoft.com"
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM1OThlZmNkNC1lNTQ5LTQwMmEtOTYwMi0wYjUwMjAxZmFlYmU=",
            "roles": [
                "owner"
            ],
            "displayName": "MOD Administrator",
            "userId": "598efcd4-e549-402a-9602-0b50201faebe",
            "email": "admin@M365x987948.OnMicrosoft.com"
        }
    ]
}
```
