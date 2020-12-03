---
title: Получение беседы 1:1 между указанным пользователем и приложением Teams
description: Получение одного сеанса разговора между указанным пользователем и приложением Teams.
author: AkJo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cff82e2368b829b6ba6f8f0bfdd24b15563d375e
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49564093"
---
# <a name="get-one-on-one-chat-between-the-specified-user-and-teams-app"></a>Получение одного сеанса разговора между указанным пользователем и приложением Teams

Пространство имен: microsoft.graph

Получение [чата](../resources/chat.md) для указанного [пользователя](../resources/user.md) и [приложения Teams](../resources/teamsapp.md).

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id}/teamwork/installedApps/{id}/chat
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает `$select` [параметр запроса OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов

| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и экземпляр объекта [Chat](../resources/chat.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-list-one-on-one-chats-between-the-specified-user-and-the-teams-app"></a>Пример 1: список бесед одного пользователя между указанным пользователем и приложением Teams

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "user_chat_teamsApps"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id}/teamwork/installedApps/{id}/chat
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "name": "user_chat_teamsApps",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats/$entity",
   "id": "19:0de69e5e-2da8-4cf2-821f-5e6585b2c65b_f32b83bb-4fc8-4db7-b7f5-76cdbbb8aa1c@unq.gbl.spaces"
 }
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User chat teamsAppInstallations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
