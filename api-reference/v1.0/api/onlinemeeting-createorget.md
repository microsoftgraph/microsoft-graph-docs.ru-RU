---
title: 'onlineMeeting: createOrGet'
description: Создайте онлайн-собрание с пользовательским внешним ИД. Если внешний ID уже существует, этот API возвращает **объект onlineMeeting** с этим внешним ИД.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 27e68b078b22380638047d9a0827459f90e3c5da
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516166"
---
# <a name="onlinemeeting-createorget"></a>onlineMeeting: createOrGet

Пространство имен: microsoft.graph

Создайте [объект onlineMeeting](../resources/onlinemeeting.md) с пользовательским внешним ИД. Если внешний ID уже существует, этот API возвращает [объект onlineMeeting](../resources/onlinemeeting.md) с этим внешним ИД. 

> **Примечание.** Собрание не отображается в календаре пользователя.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | OnlineMeetings.ReadWrite                    |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                               |
| Для приложений                            | OnlineMeetings.ReadWrite.All*                |

> [!IMPORTANT]
> \*Администраторы должны [](/graph/concepts/cloud-communication-online-meeting-application-access-policy.md) создать политику доступа к приложениям и предоставить ее пользователю, уполномочив приложение, настроенного в политике, создать или получить онлайн-встречу с внешним ИД от имени этого пользователя (пользовательский ID, указанный в пути запроса).

## <a name="http-request"></a>HTTP-запрос
Вызов **API createOrGet** с делегированным маркером:
<!-- { "blockType": "ignored" } -->
```http
POST /me/onlineMeetings/createOrGet
```

Вызов **API createOrGet** с помощью маркера приложения:
<!-- { "blockType": "ignored" } -->
```http
POST /users/{userId}/onlineMeetings/createOrGet
```

> **Примечание.** `userId` — это идентификатор объекта пользователя на [портале управления пользователями Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade). Дополнительные сведения см. в статье [Политики доступа для приложений](/graph/cloud-communication-online-meeting-application-access-policy).

## <a name="request-headers"></a>Заголовки запросов
| Имя          | Описание               |
|:--------------|:--------------------------|
| Авторизация | Bearer {токен}. Обязательный. |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса
В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр        | Тип                                     |Описание                                                                                                                                    |
|:-----------------|:-----------------------------------------|:--------------------------------------------------------------------------|
| endDateTime      | DateTime                                 | Время окончания собрания в UTC. |
| externalId       | String                                   | Внешний ID. Пользовательский ID. (Обязательно) |
| participants     | [meetingParticipants](../resources/meetingparticipants.md)          | Участники, связанные с онлайн-собранием.  Это включает организатора и участников. |
| startDateTime    | DateTime                                 | Время начала собрания в UTC. |
| subject          | String                                   | Тема собрания в Интернете. |

> **Примечания.**
>
> - Если **startDateTime** и **endDateTime** не предоставлены, по умолчанию **startDateTime** будет по умолчанию по текущему значению dateTime, а **значение endDateTime** равно **значению startDateTime** + 1 час.
>
> - Если **предоставляется startDateTime,** а **endDateTime** — нет, значение **endDateTime** будет равно **значению startDateTime** + 1 час.
>
> - Ошибка будет выброшена, если **endDateTime** предоставляется без **startDateTime** или если **endDateTime** является более ранним, чем **startDateTime.**

## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код ответа, если создается новое собрание, или код ответа при извлечении `201 Created` `200 OK` существующего собрания. В обоих случаях [объект onlineMeeting](../resources/onlinemeeting.md) возвращается в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

В следующем примере показано, как создать или получить собрание в Интернете с внешним ИД.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-or-get-onlinemeeting"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/onlineMeetings/createOrGet
Content-Type: application/json

{
    "startDateTime": "2020-02-06T01:49:21.3524945+00:00",
    "endDateTime": "2020-02-06T02:19:21.3524945+00:00",
    "subject": "Create a meeting with customId provided",
    "externalId": "7eb8263f-d0e0-4149-bb1c-1f0476083c56",
    "participants": {
        "attendees": [
            {
                "identity": {
                    "user": {
                        "id": "1f35f2e6-9cab-44ad-8d5a-b74c14720000"
                    }
                },
                "upn": "test1@contoso.com"
            }
        ]
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-or-get-onlinemeeting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-or-get-onlinemeeting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-or-get-onlinemeeting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-or-get-onlinemeeting-java-snippets.md)]
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
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "(redacted)",
    "creationDateTime": "2020-09-11T06:30:18.1909168Z",
    "startDateTime": "2020-09-11T06:30:18.0615989Z",
    "endDateTime": "2020-09-11T07:30:18.0615989Z",
    "joinWebUrl": "(redacted)",
    "subject": "Create a meeting with customId provided",
    "isBroadcast": false,
    "autoAdmittedUsers": "EveryoneInCompany",
    "isEntryExitAnnounced": true,
    "allowedPresenters": "everyone",
    "videoTeleconferenceId": "(redacted)",
    "externalId": "7eb8263f-d0e0-4149-bb1c-1f0476083c56",
    "participants": {
        "organizer": {
            "upn": "(redacted)",
            "role": "presenter",
            "identity": {
                "user": {
                    "id": "(redacted)",
                }
            }
        },
        "attendees": [
            {
                "upn": "test1@contoso.com",
                "role": null,
                "identity": {
                    "user": {
                        "id": "1f35f2e6-9cab-44ad-8d5a-b74c14720000",
                    }
                }
            }
        ],
        "producers": [],
        "contributors": []
    },
    "lobbyBypassSettings": {
        "scope": "organization",
        "isDialInBypassEnabled": false
    },
    "audioConferencing": {
        "conferenceId": "(redacted)",
        "tollNumber": "+1 206-485-3005",
        "tollFreeNumber": null,
        "dialinUrl": "https://dialin.teams.microsoft.com/0e73a853-1cc2-436c-b18c-9f53e0a97c24?id=(redacted)"
    },
    "chatInfo": {
        "threadId": "19:7ebda77322dd4505ac4dedb5b67df076@thread.tacv2",
        "messageId": "0",
        "replyChainMessageId": null
    },
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

