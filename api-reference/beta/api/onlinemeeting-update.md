---
title: Обновление onlineMeeting
description: Обновление свойств собрания по сети.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 6699071afe0fb8b7e6ec2183e29785558a2c5d48
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292170"
---
# <a name="update-onlinemeeting"></a>Обновление onlineMeeting

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств **startDateTime,** **endDateTime,** **участников** и темы указанного [объекта onlineMeeting.](../resources/onlinemeeting.md) 

## <a name="permissions"></a>Разрешения

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | OnlineMeetings.ReadWrite                    |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Для приложений                            | OnlineMeetings.ReadWrite.All*                |

> [!IMPORTANT]
> \*Администраторы должны [](/graph/cloud-communication-online-meeting-application-access-policy) создать политику доступа к приложениям и предоставить ее пользователю, разрешив приложению, настроенное в политике, обновлять собрание по сети от имени этого пользователя (ид пользователя, указанный в пути запроса).

## <a name="http-request"></a>HTTP-запрос
Обновление указанного onlineMeeting с помощью ИД собрания с помощью делегирования маркера:
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onlineMeetings/{meetingId}
```

Обновление указанного onlineMeeting с помощью ИД собрания с помощью маркера приложения:
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{userId}/onlineMeetings/{meetingId}
```

> **Примечания.**
> - `userId`— это ИД объекта пользователя на портале [управления пользователями Azure.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade) Дополнительные сведения [см. в политике доступа к приложениям.](/graph/cloud-communication-online-meeting-application-access-policy)
> - `meetingId`— **это ид** объекта [onlineMeeting.](../resources/onlinemeeting.md)

## <a name="request-headers"></a>Заголовки запросов
| Имя          | Описание                 |
| :------------ | :-------------------------- |
| Авторизация | Bearer {токен}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса
В тексте запроса должно быть представление объекта [onlineMeeting](../resources/onlinemeeting.md) в формате JSON. Изменять можно **только свойства startDateTime,** **endDateTime,** **участников** и темы.  **StartDateTime** и **endDateTime** должны отображаться парами.

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [onlineMeeting](../resources/onlinemeeting.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_onlinemeeting_request"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/onlineMeetings/{id}
Content-Type: application/json 

{
  "startDateTime": "2020-09-09T14:33:30.8546353-07:00",
  "endDateTime": "2020-09-09T15:03:30.8566356-07:00",
  "subject": "Patch Meeting Subject"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/patch-onlinemeeting-request-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/patch-onlinemeeting-request-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-onlinemeeting-request-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/patch-onlinemeeting-request-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "id":"{id}",
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
      "tollNumber":"number",
      "tollFreeNumber":null,
      "dialinUrl":"url"
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


