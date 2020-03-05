---
title: Создание объекта onlineMeeting
description: Создание собрания по сети от имени пользователя, указанного в тексте запроса.
author: ananmishr
localization_priority: Priority
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: f3195f55532713ee4bc359623b8fed241b799f3f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441475"
---
# <a name="create-onlinemeeting"></a>Создание объекта onlineMeeting

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание собрания по сети от имени пользователя с помощью ИД объекта (OID) в маркере пользователя.

> **Примечание.** Собрание не отображается в календаре пользователя.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | OnlineMeetings.ReadWrite                    |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается                               |
| Для приложений                            | OnlineMeetings.ReadWrite.All*  |

> \* **Примечание.** Поддержка разрешений приложений прекращается, и они будут удалены в апреле 2020 г.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /app/onlineMeetings
POST /communications/onlineMeetings
POST /me/onlineMeetings
```
> **Примечание.** Путь `/app` является устаревшим. В дальнейшем используйте путь `/communications`.

## <a name="request-headers"></a>Заголовки запросов
| Имя          | Описание               |
|:--------------|:--------------------------|
| Авторизация | Bearer {токен}. Обязательный. |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Основной текст запроса
В тексте запроса должно быть представление объекта [onlineMeeting](../resources/onlinemeeting.md) в формате JSON.

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [onlineMeeting](../resources/onlinemeeting.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-create-an-online-meeting-with-application-token"></a>Пример 1. Создание собрания по сети с помощью маркера приложения

#### <a name="request"></a>Запрос

> [!Note]
> Создание собрания по сети с помощью маркера приложения является устаревшим способом, и его поддержка будет прекращена в апреле 2020 г. В дальнейшем используйте путь /me с маркером пользователя, чтобы создавать собрания по сети.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-onlinemeeting-app-token"
}-->
```http
POST https://graph.microsoft.com/beta/communications/onlineMeetings
Content-Type: application/json

{
  "startDateTime":"2019-09-09T14:33:30.8546353-07:00",
  "endDateTime":"2019-09-09T15:03:30.8566356-07:00",
  "subject":"Application Token Meeting",
  "participants": {
    "organizer": {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f"
        }
      }
    }
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-onlinemeeting-app-token-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onlinemeeting-app-token-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onlinemeeting-app-token-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


В тексте запроса должно быть представление объекта [onlineMeeting](../resources/onlinemeeting.md) в формате JSON.

#### <a name="response"></a>Отклик

>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.onlineMeeting",
  "autoAdmittedUsers": "everyone",
  "audioConferencing": {
    "tollNumber": "+12525634478",
    "tollFreeNumber": "+18666390588",
    "ConferenceId": "2425999",
    "dialinUrl": "https://dialin.teams.microsoft.com/22f12fa0-499f-435b-bc69-b8de580ba330?id=2425999"
  },
  "chatInfo": {
    "threadId": "19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
    "messageId": "0",
    "replyChainMessageId": "0"
  },
  "creationDateTime": "2019-07-11T02:17:17.6491364Z",
  "startDateTime": "2019-07-11T02:17:17.6491364Z",
  "endDateTime": "2019-07-11T02:47:17.651138Z",
  "id": "550fae72-d251-43ec-868c-373732c2704f_19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
  "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz%40thread.skype/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22550fae72-d251-43ec-868c-373732c2704f%22%7d",
  "participants": {
    "organizer": {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "upn": "upn-value"
    }
  },
  "subject": "Application Token Meeting"
}
```

### <a name="example-2-create-an-online-meeting-with-user-token"></a>Пример 2. Создание собрания по сети с помощью маркера пользователя

#### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-onlinemeeting-user-token"
}-->
```http
POST https://graph.microsoft.com/beta/me/onlineMeetings
Content-Type: application/json

{
  "startDateTime":"2019-07-12T14:30:34.2444915-07:00",
  "endDateTime":"2019-07-12T15:00:34.2464912-07:00",
  "subject":"User Token Meeting"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-onlinemeeting-user-token-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onlinemeeting-user-token-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onlinemeeting-user-token-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.onlineMeeting",
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('f4053f86-17cc-42e7-85f4-f0389ac980d6')/onlineMeetings/$entity",
  "audioConferencing": {
    "tollNumber": "+12525634478",
    "tollFreeNumber": "+18666390588",
    "ConferenceId": "2425999",
    "dialinUrl": "https://dialin.teams.microsoft.com/22f12fa0-499f-435b-bc69-b8de580ba330?id=2425999"
  },
  "chatInfo": {
    "threadId": "19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
    "messageId": "0",
    "replyChainMessageId": "0"
  },
  "creationDateTime": "2019-07-11T02:17:17.6491364Z",
  "startDateTime": "2019-07-11T02:17:17.6491364Z",
  "endDateTime": "2019-07-11T02:47:17.651138Z",
  "id": "550fae72-d251-43ec-868c-373732c2704f_19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
  "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz%40thread.skype/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22550fae72-d251-43ec-868c-373732c2704f%22%7d",
  "participants": {
    "organizer": {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "upn": "upn-value"
    }
  },
  "subject": "User Token Meeting"
}
```

### <a name="example-3-create-an-online-meeting-in-a-microsoft-teams-channel-with-a-user-token"></a>Пример 3. Создание собрания по сети в канале Microsoft Teams с помощью маркера пользователя

#### <a name="request"></a>Запрос
>**Примечание.** Идентификатор объекта переданного маркера пользователя должен быть элементом канала, представленного с помощью threadid в полезных данных.

```http
POST https://graph.microsoft.com/beta/me/onlineMeetings
Content-Type: application/json

{
  "startDateTime":"2019-07-12T14:30:34.2444915-07:00",
  "endDateTime":"2019-07-12T15:00:34.2464912-07:00",
  "subject":"User meeting in Microsoft Teams channel.",
  "chatInfo": {
    "threadId":"19%3A3b52398f3c524556894b776357c1dd79%40thread.skype"
  }
}
```
#### <a name="response"></a>Отклик

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "example",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('f4053f86-17cc-42e7-85f4-f0389ac980d6')/onlineMeetings/$entity",
  "audioConferencing": {
    "tollNumber": "+12525634478",
    "tollFreeNumber": "+18666390588",
    "ConferenceId": "2425999",
    "dialinUrl": "https://dialin.teams.microsoft.com/22f12fa0-499f-435b-bc69-b8de580ba330?id=2425999"
  },
  "chatInfo": {
    "threadId": "19%3A3b52398f3c524556894b776357c1dd79%40thread.skype",
    "messageId": "1563302249053",
    "replyChainMessageId": null
  },
  "creationDateTime": "2019-07-11T02:17:17.6491364Z",
  "startDateTime": "2019-07-11T02:17:17.6491364Z",
  "endDateTime": "2019-07-11T02:47:17.651138Z",
  "id": "550fae72-d251-43ec-868c-373732c2704f_19%3A3b52398f3c524556894b776357c1dd79%40thread.skype",
  "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz%40thread.skype/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22550fae72-d251-43ec-868c-373732c2704f%22%7d",
  "participants": {
    "organizer": {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "upn": "upn-value"
    }
  },
  "subject": "User meeting in Microsoft Teams channel."
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create onlineMeeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
