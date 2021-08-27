---
title: Чаты списка
description: Извлечение списка чатов для пользователя.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 356b47990865ec242b2d99a40cec9a25ed030669
ms.sourcegitcommit: f99dc2b6c8b4cb6f9f74cd780dccc47a2bccfaa6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2021
ms.locfileid: "58668012"
---
# <a name="list-chats"></a>Чаты списка

Пространство имен: microsoft.graph

Извлечение списка [чатов,](../resources/chat.md) в которые входит пользователь.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Chat.ReadBasic, Chat.Read, Chat.ReadWrite |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
GET /me/chats
GET /users/{user-id | user-principal-name}/chats
GET /chats
```

## <a name="optional-query-parameters"></a>Необязательные параметры запроса

Этот метод поддерживает параметры запросов (только для свойств участников) и `$expand`  `$filter` [OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов

| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [chat](../resources/chat.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="example-1-list-all-chats"></a>Пример 1. Список всех чатов

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "list_chats"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#chats",
    "@odata.count": 3,
    "value": [
        {
            "id": "19:meeting_MjdhNjM4YzUtYzExZi00OTFkLTkzZTAtNTVlNmZmMDhkNGU2@thread.v2",
            "topic": "Meeting chat sample",
            "createdDateTime": "2020-12-08T23:53:05.801Z",
            "lastUpdatedDateTime": "2020-12-08T23:58:32.511Z",
            "chatType": "meeting"
        },
        {
            "id": "19:561082c0f3f847a58069deb8eb300807@thread.v2",
            "topic": "Group chat sample",
            "createdDateTime": "2020-12-03T19:41:07.054Z",
            "lastUpdatedDateTime": "2020-12-08T23:53:11.012Z",
            "chatType": "group"
        },
        {
            "id": "19:d74fc2ed-cb0e-4288-a219-b5c71abaf2aa_8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca@unq.gbl.spaces",
            "topic": null,
            "createdDateTime": "2020-12-04T23:10:28.51Z",
            "lastUpdatedDateTime": "2020-12-04T23:10:36.925Z",
            "chatType": "oneOnOne"
        }
    ]
}
```

### <a name="example-2-list-all-chats-along-with-the-members-of-each-chat"></a>Пример 2. Список всех чатов вместе с участниками каждого чата
#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "list_chats_expand_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats?$expand=members
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика. 

> [!NOTE]
> Идентификаторы участия, возвращаемые сервером, должны рассматриваться как непрозрачные строки. Клиент не должен пытаться разработать или сделать какие-либо предположения об этих ИД ресурсов.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#chats(members())",
    "@odata.count": 3,
    "value": [
        {
            "id": "19:meeting_MjdhNjM4YzUtYzExZi00OTFkLTkzZTAtNTVlNmZmMDhkNGU2@thread.v2",
            "topic": "Meeting chat sample",
            "createdDateTime": "2020-12-08T23:53:05.801Z",
            "lastUpdatedDateTime": "2020-12-08T23:58:32.511Z",
            "chatType": "meeting",
            "members@odata.context": "https://graph.microsoft.com/v1.0/$metadata#chats('19%3Ameeting_MjdhNjM4YzUtYzExZi00OTFkLTkzZTAtNTVlNmZmMDhkNGU2%40thread.v2')/members",
            "members": [
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkM123=",
                    "roles": [],
                    "displayName": "Tony Stark",
                    "userId": "4595d2f2-7b31-446c-84fd-9b795e63114b",
                    "email": "starkt@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMz6Jk45=",
                    "roles": [],
                    "displayName": "Peter Parker",
                    "userId": "d74fc2ed-cb0e-4288-a219-b5c71abaf2aa",
                    "email": "parkerp@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJ989kMTQ=",
                    "roles": [],
                    "displayName": "Nick Fury",
                    "userId": "8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
                    "email": "furyn@teamsgraph.onmicrosoft.com"
                }
            ]
        },
        {
            "id": "19:561082c0f3f847a58069deb8eb300807@thread.v2",
            "topic": "Group chat sample",
            "createdDateTime": "2020-12-03T19:41:07.054Z",
            "lastUpdatedDateTime": "2020-12-08T23:53:11.012Z",
            "chatType": "group",
            "members@odata.context": "https://graph.microsoft.com/v1.0/$metadata#chats('19%3A561082c0f3f847a58069deb8eb300807%40thread.v2')/members",
            "members": [
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkM123=",
                    "roles": [],
                    "displayName": "Tony Stark",
                    "userId": "4595d2f2-7b31-446c-84fd-9b795e63114b",
                    "email": "starkt@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM312ftMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkM123=",
                    "roles": [],
                    "displayName": "Bruce Banner",
                    "userId": "48bf9d52-dca7-4a5f-8398-37b95cc7bd83",
                    "email": "bannerb@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWai3MTetN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkM123=",
                    "roles": [],
                    "displayName": "TChalla",
                    "userId": "9efb1aea-4f83-4673-bdcd-d3f3c7be28c2",
                    "email": "tchalla@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwamii00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkM123=",
                    "roles": [],
                    "displayName": "Thor Odinson",
                    "userId": "976f4b31-fd01-4e0b-9178-29cc40c14438",
                    "email": "odinsont@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWopiLWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJkM123=",
                    "roles": [],
                    "displayName": "Steve Rogers",
                    "userId": "976f4b31-fd01-4e0b-9178-29cc40c14438",
                    "email": "rogerss@teamsgraph.onmicrosoft.com"
                }
            ]
        },
        {
            "id": "19:d74fc2ed-cb0e-4288-a219-b5c71abaf2aa_8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca@unq.gbl.spaces",
            "topic": null,
            "createdDateTime": "2020-12-04T23:10:28.51Z",
            "lastUpdatedDateTime": "2020-12-04T23:10:36.925Z",
            "chatType": "oneOnOne",
            "members@odata.context": "https://graph.microsoft.com/v1.0/$metadata#chats('19%3Ad74fc2ed-cb0e-4288-a219-b5c71abaf2aa_8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca%40unq.gbl.spaces')/members",
            "members": [
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMzJ989kMTQ=",
                    "roles": [],
                    "displayName": "Nick Fury",
                    "userId": "8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
                    "email": "furyn@teamsgraph.onmicrosoft.com"
                },
                {
                    "@odata.type": "#microsoft.graph.aadUserConversationMember",
                    "id": "MmFiOWM3OTYtMjkwMi00NWY4LWI3MTItN2M1YTYzY2Y0MWM0IyNlZWY5Y2IzNi0wNmRlLTQ2OWItODdjZC03MGY0Y2JlMz6Jk45=",
                    "roles": [],
                    "displayName": "Peter Parker",
                    "userId": "d74fc2ed-cb0e-4288-a219-b5c71abaf2aa",
                    "email": "parkerp@teamsgraph.onmicrosoft.com"
                }
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List chats",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
