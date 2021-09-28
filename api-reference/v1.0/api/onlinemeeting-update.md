---
title: Обновление onlineMeeting
description: Обновление свойств собрания в Интернете.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: ce8131340ffd07b61fedcf189af90911a322925f
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979385"
---
# <a name="update-onlinemeeting"></a>Обновление onlineMeeting

Пространство имен: microsoft.graph

Обновление свойств указанного [объекта onlineMeeting.](../resources/onlinemeeting.md)

См. [раздел Запрос](#request-body) тела для списка свойств, которые поддерживают обновление.

## <a name="permissions"></a>Разрешения

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | OnlineMeetings.ReadWrite                    |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Для приложений                            | OnlineMeetings.ReadWrite.All                |

Чтобы использовать разрешение приложения для этого API, [](/graph/cloud-communication-online-meeting-application-access-policy) администраторы клиентов должны создать политику доступа к приложениям и предоставить ее пользователю для авторизации приложения, настроенного в политике, для получения артефактов собраний в Интернете от имени этого пользователя (с пользовательским ИД, указанным в пути запроса).

## <a name="http-request"></a>HTTP-запрос

Обновление указанного **onlineMeeting** с помощью ID собрания с делегированием () и разрешением `/me` приложения `/users/{userId}/` () :
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onlineMeetings/{meetingId}
PATCH /users/{userId}/onlineMeetings/{meetingId}
```

> [!NOTE]
>
> - `userId` — это идентификатор объекта пользователя на [портале управления пользователями Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade). Дополнительные сведения см. в [политике доступа к приложениям.](/graph/cloud-communication-online-meeting-application-access-policy)
> - `meetingId`является **id** объекта [onlineMeeting.](../resources/onlinemeeting.md)

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание                 |
| :------------ | :-------------------------- |
| Авторизация | Bearer {токен}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В следующей таблице перечислены свойства, которые можно обновить. В орган запроса включаем только свойства, которые требуют обновления, за следующими исключениями:

- Для настройки даты начала или окончания собрания в интернете всегда требуются свойства **startDateTime** и **endDateTime** в теле запроса.
- Поле **организатора** **свойства участников** не может быть обновлено. Организатор собрания не может быть изменен после создания собрания.
- Для настройки **поля** участников  свойства участников, например добавления или удаления участника собрания, всегда требуется полный список участников в теле запроса.

Последний столбец указывает, будет ли обновление этого свойства вступает в силу для выполнения собрания.

| Свойство                    | Тип                                                       | Описание                                                                         | Применяется к на ходу собраний?    |
|-----------------------------|------------------------------------------------------------|-------------------------------------------------------------------------------------|------------------------------|
| startDateTime               | Даты и время                                                   | Время начала собрания в UTC.                                                      | Нет                           |
| endDateTime                 | Даты и время                                                   | Время окончания собрания в UTC.                                                        | Нет                           |
| subject                     | String                                                     | Тема собрания в Интернете.                                                  | Нет                           |
| participants                | [meetingParticipants](../resources/meetingparticipants.md) | Участники, связанные с онлайн-собранием. Обновления могут быть только у участников. | Нет                           |
| isEntryExitAnnounced        | Логический                                                    | Следует ли объявлять о том, когда звонители присоединяются или уходят.                              | Да                          |
| lobbyBypassSettings         | [lobbyBypassSettings](../resources/lobbyBypassSettings.md) | Указывает, какие участники могут обойти вестибюль собрания.                          | Да                          |
| allowedPresenters           | onlineMeetingPresenters                                    | Указывает, кто может быть презентовщиком на собрании.                                      | Да |
| allowAttendeeToEnableCamera | Логический                                                    | Указывает, могут ли участники включить камеру.                               | Да                          |
| allowAttendeeToEnableMic    | Логический                                                    | Указывает, могут ли участники включить микрофон.                           | Да                          |
| allowMeetingChat            | meetingChatMode                                            | Указывает режим чата собраний.                                                 | Да                          |
| allowTeamworkReactions      | Логический                                                    | Указывает, Teams для собрания включены ли Teams реакции.                      | Да                          |

> [!NOTE]
>
>- Список возможных значений для **allowedPresenters** и **allowMeetingChat** см. [в onlineMeeting.](../resources/onlinemeeting.md)
>- При обновлении значения **allowedPresenters** включай полный список участников с заданными участниками роли, заданными в `roleIsPresenter`   `presenter` тексте запроса.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект onlineMeeting](../resources/onlinemeeting.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-update-the-startdatetime-enddatetime-and-subject"></a>Пример 1. Обновление startDateTime, endDateTime и субъекта

#### <a name="request"></a>Запрос

> **Примечание:** Для читаемости был сокращен ID собрания.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi"],
  "name": "update_start_end_subject"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi
Content-Type: application/json 

{
  "startDateTime": "2020-09-09T14:33:30.8546353-07:00",
  "endDateTime": "2020-09-09T15:03:30.8566356-07:00",
  "subject": "Patch Meeting Subject"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-start-end-subject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-start-end-subject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-start-end-subject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-start-end-subject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "id":"MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi",
   "creationDateTime":"2020-07-03T00:23:39.444642Z",
   "startDateTime":"2020-09-09T21:33:30.8546353Z",
   "endDateTime":"2020-09-09T22:03:30.8566356Z",
   "joinWebUrl":"url",
   "subject":"Patch Meeting Subject",
   "isBroadcast":false,
   "autoAdmittedUsers":"EveryoneInCompany",
   "outerMeetingAutoAdmittedUsers":null,
   "participants":{
      "organizer":{
         "upn":"upn",
         "role": "presenter",
         "identity":{
            "azureApplicationInstance":null,
            "applicationInstance":null,
            "application":null,
            "device":null,
            "user":{
               "id":"8716745d-77a9-4be3-afff-009e4b81658e",
               "displayName":null,
               "tenantId":"0823831b-1f1b-424b-b90a-1caa345a742a",
               "identityProvider":"AAD"
            }
         }
      }
   },
   "audioConferencing":{
      "conferenceId":"id",
      "tollNumber":"+1-900-555-0100",
      "tollFreeNumber":"+1-800-555-0100",
      "dialinUrl":"url"
   }
}
```

#### <a name="example-2-update-the-lobbybypasssettings"></a>Пример 2. Обновление lobbyBypassSettings
> **Примечание:** Для читаемости был сокращен ID собрания.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi"],
  "name": "update_lobbyBypassSettings"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi
Content-Type: application/json 

{
  "lobbyBypassSettings": {
      "isDialInBypassEnabled": true
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-lobbybypasssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-lobbybypasssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-lobbybypasssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-lobbybypasssettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi",
    "creationDateTime":"2020-07-03T00:23:39.444642Z",
    "startDateTime":"2020-09-09T21:33:30.8546353Z",
    "endDateTime":"2020-09-09T22:03:30.8566356Z",
    "joinWebUrl":"(redacted)",
    "subject":"Patch Meeting Subject",
    "autoAdmittedUsers": "EveryoneInCompany",
    "isEntryExitAnnounced": true,
    "allowedPresenters": "everyone",
    "videoTeleconferenceId": "(redacted)",
    "participants": {
        "organizer": {
            "upn": "(redacted)",
            "role": "presenter",
            "identity": {
                "user": {
                    "id": "dc17674c-81d9-4adb-bfb2-8f6a442e4622",
                    "displayName": null,
                    "tenantId": "909c6581-5130-43e9-88f3-fcb3582cde38",
                    "identityProvider": "AAD"
                }
            }
        },
        "attendees": [],
    },
    "lobbyBypassSettings": {
        "scope": "organization",
        "isDialInBypassEnabled": true
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2020-7-16 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Patch online meeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


