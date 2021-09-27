---
title: 'conversationMember: add'
description: Добавьте в команду участников оптом.
author: abshar-teams
doc_type: apiPageType
ms.localizationpriority: medium
ms.prod: microsoft-teams
ms.openlocfilehash: 9d313e6d609ad8192541e0d2a19ab15f14c5ed11
ms.sourcegitcommit: 30fca91ed203a9ab7b0562833ce0c20c7fb7b7b1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/27/2021
ms.locfileid: "59932075"
---
# <a name="conversationmember-add"></a>conversationMember: add

Пространство имен: microsoft.graph

Добавление нескольких участников в [команду](../resources/team.md) одним запросом. В ответе приводится подробная информация о том, какие членства могут быть созданы и не могут быть созданы.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий) | 
|:--------------------|:--------------------------|
| Делегированные (рабочая или учебная учетная запись) | TeamMember.ReadWrite.All  |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Приложение | TeamMember.ReadWrite.All   |


## <a name="http-request"></a>HTTP-запрос

Это связанное действие, чтобы добавить несколько элементов в **коллекцию conversationMember** в одном запросе.
<!-- { "blockType": "ignored" } -->

```http
POST /teams/{team-id}/members/add
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок        | Значение                     |
| :------------ | :------------------------ |
| Авторизация | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите в формате JSON представление списка производных `conversationMember`, которые необходимо добавить.

В следующей таблице указаны параметры, которые можно использовать с этим действием.

|Параметр|Тип|Описание|
|:---|:---|:---|
|values|Коллекция [conversationMember](../resources/conversationmember.md)|Список участников беседы, которых следует добавить.|


## <a name="response"></a>Отклик

В случае успеха это действие возвращает код отклика `200 OK` и коллекцию производных ресурса [actionResultPart](../resources/actionresultpart.md) в тексте отклика.

Этот API возвращает ответ, который указывает, что все поставленные члены были добавлены в команду или ответ, который указывает, что в команду были добавлены только некоторые из `200` `207` поставленных членов. Вызывающая сторона должна проверить полезные данные отклика, чтобы определить, какого участника не удалось добавить. Текст отклика является коллекцией производных ресурса [actionResultPart](../resources/actionresultpart.md).

## <a name="examples"></a>Примеры

### <a name="example-1-add-members-in-bulk-to-a-team"></a>Пример 1. Массовое добавление участников в команду

#### <a name="request"></a>Запрос

В следующем примере показан запрос на добавление нескольких участников в команду.

<!-- {
  "blockType": "request",
  "name": "bulkaddmembers_team"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/e4183b04-c9a2-417c-bde4-70e3ee46a6dc/members/add
Content-Type: application/json

{
    "values": [
        {
            "@odata.type": "microsoft.graph.aadUserConversationMember",
            "roles":[],
            "user@odata.bind": "https://graph.microsoft.com/v1.0/users('18a80140-b0fb-4489-b360-2f6efaf225a0')"
        },
        {
            "@odata.type": "microsoft.graph.aadUserConversationMember",
            "roles":["owner"],
            "user@odata.bind": "https://graph.microsoft.com/v1.0/users('86503198-b81b-43fe-81ee-ad45b8848ac9')"
        }
    ]
}
```


#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.actionResultPart",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.aadUserConversationMemberResult)",
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMemberResult",
            "userId": "18a80140-b0fb-4489-b360-2f6efaf225a0",
            "error": null
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMemberResult",
            "userId": "86503198-b81b-43fe-81ee-ad45b8848ac9",
            "error": null
        }
    ]
}
```

### <a name="example-2-add-members-in-bulk-and-encounter-partial-failure"></a>Пример 2. Массовое добавление участников с возникновением частичного сбоя

#### <a name="request"></a>Запрос

В следующем примере показан запрос на добавление нескольких участников в команду, приводящий к частичному сбою.


<!-- {
  "blockType": "request",
  "name": "bulkaddmembers_team_partial_failure"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/e4183b04-c9a2-417c-bde4-70e3ee46a6dc/members/add
Content-Type: application/json

{
    "values": [
        {
            "@odata.type": "microsoft.graph.aadUserConversationMember",
            "roles":[],
            "user@odata.bind": "https://graph.microsoft.com/v1.0/users('18a80140-b0fb-4489-b360-2f6efaf225a0')"
        },
        {
            "@odata.type": "microsoft.graph.aadUserConversationMember",
            "roles":["owner"],
            "user@odata.bind": "https://graph.microsoft.com/v1.0/users('86503198-b81b-43fe-81ee-ad45b8848ac9')"
        }
    ]
}
```


#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.actionResultPart",
  "isCollection": true
} -->

```http
HTTP/1.1 207 MULTI-STATUS
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.addConversationMemberResult)",
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMemberResult",
            "userId": "18a80140-b0fb-4489-b360-2f6efaf225a0",
            "error": {
                "code": "NotFound",
                "message": ""
            }
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMemberResult",
            "userId": "86503198-b81b-43fe-81ee-ad45b8848ac9",
            "error": null
        }
    ]
}
```


## <a name="see-also"></a>См. также

- [Добавление участника в команду](team-post-members.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add members to a team in bulk.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
