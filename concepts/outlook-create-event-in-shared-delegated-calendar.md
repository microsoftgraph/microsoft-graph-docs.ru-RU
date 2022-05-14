---
title: Создание событий Outlook в общем или делегированном календаре
description: В Outlook клиенты могут поделиться календарем с другими пользователями и позволить им просматривать или изменять события в этом календаре. Клиенты также могут предоставить делегату право выполнять действия от их имени, получать приглашения на собрания или отвечать на них, а также создавать или изменять элементы в календаре.
author: juforan
ms.localizationpriority: high
ms.prod: outlook
ms.openlocfilehash: 77534a6b1fad8392df01c33f91e0db321767007c
ms.sourcegitcommit: 3a8f6a77dd01a50adf543aaedbf6ec5a202abf93
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/12/2022
ms.locfileid: "65366081"
---
# <a name="create-outlook-events-in-a-shared-or-delegated-calendar"></a>Создание событий Outlook в общем или делегированном календаре

В Outlook клиенты могут поделиться календарем с другими пользователями и позволить им просматривать, создавать или изменять события в этом календаре. Клиенты также могут предоставить делегату право выполнять действия от их имени, получать приглашения на собрания или отвечать на них, а также создавать или изменять элементы в календаре.

Что касается программного кода, Microsoft Graph поддерживает чтение и запись событий в календарях, доступ к которым был предоставлен другими пользователями, а также чтение общих календарей и обновление их имен для получателей общего доступа. Поддержка также относится к делегированным календарям. Далее в этой статье рассматривается создание собрания как нового события в общем или делегированном календаре. Сведения о получении событий см. в статье [Получение событий Outlook из общего или делегированного календаря](outlook-get-shared-events-calendars.md).

Приведенное ниже руководство содержит пример сценария, в котором Артем делегировал свой основной календарь Анне в Outlook и сохранил параметр почтового ящика Outlook по умолчанию, позволяющий направлять приглашения на собрание и ответы только делегатам. (Этот параметр соответствует свойству **delegateMeetingMessageDeliveryOptions** в [mailboxSettings](/graph/api/resources/mailboxsettings)Алекса, установленному в качестве значения по умолчанию `sendToDelegateOnly`.) 

В этом руководстве описано несколько последующих шагов.
1. [Анна получает календарь, делегированный Артемом](#step-1-adele-gets-the-delegated-calendar).
2. [Анна отправляет приглашение на собрание Алене и Марте от имени Артема](#step-2-adele-creates-and-sends-an-invitation-on-alex-behalf). 
3. [Алена получает приглашение на собрание и изучает соответствующее событие в своем календаре](#step-3-christie-receives-meeting-request-and-inspects-the-associated-event-in-her-calendar).
4. [Алена помечает приглашение "Под вопросом"](#step-4-christie-responds-to-the-meeting-request).
5. [Анна получает ответное сообщение Алены](#step-5-adele-receives-the-response-message).
6. [Артем проверяет ответы участников в рамках события](#step-6-alex-accesses-responses-as-part-of-the-event).

Если Артем предоставил общий доступ, но не делегировал свой календарь Анне:

- При выполнении входа от имени Анны приложение может [получить календарь, которым Артем поделился с Анной](outlook-get-shared-events-calendars.md#sharee-get-shared-custom-calendar-or-its-events-from-sharees-mailbox).
- Приложение может использовать приглашения и ответы в шагах 2–4 для общего календаря так же, как и для делегированного календаря.
- На шаге 5 приложение может выполнить вход под именем Артема вместо Анны и получить ответное сообщение Алены. 

## <a name="step-1-adele-gets-the-delegated-calendar"></a>Шаг 1. Анна получает делегированный календарь

Войдя в систему под именем Анны, получите календари, к которым у нее есть доступ, и определите, какой календарь делегирован Артемом, чтобы создать в нем событие на следующем шаге. 

**Разрешения Microsoft Graph**

Для этой операции необходимо использовать подходящее разрешение делегирования, `Calendars.Read.Shared`. Дополнительные сведения см. в разделе [Разрешения календаря](permissions-reference.md#calendars-permissions).

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_Adele_calendars"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendars
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-adele-calendars-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-adele-calendars-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-adele-calendars-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-adele-calendars-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


Обратите внимание, что успешный отклик включает код ответа HTTP 200, основной календарь Анны, а также копию календаря, делегированного Артемом, в ее почтовом ящике со следующими свойствами:

- **canShare** имеет значение "false", так как Анна является делегатом, а не владельцем календаря.
- **canEdit** имеет значение "true", так как в качестве делегата Анна имеет доступ с правами записи к событиям, не являющимся частными, в делегированном календаре.
- **owner** имеет значение `Alex Wilber`, которое показывает, что это календарь Артема.

<!-- {
  "blockType": "response",
  "name": "get_Adele_calendars",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69')/calendars",
    "value": [
        {
            "id": "AQMkADGkAAAJMjAAAAA==",
            "name": "Calendar",
            "color": "auto",
            "changeKey": "NDznl+Uh50WkanaCOKHkaQAAAAACXQ==",
            "canShare": true,
            "canViewPrivateItems": true,
            "canEdit": true,
            "owner": {
                "name": "Adele Vance",
                "address": "AdeleV@contoso.OnMicrosoft.com"
            }
        },
        {
            "id": "AAMkADRpAABf0JlzAAA=",
            "name": "Alex Wilber",
            "color": "auto",
            "changeKey": "NDznl+Uh50WkanaCOKHkaQAAX8m4eQ==",
            "canShare": false,
            "canViewPrivateItems": false,
            "canEdit": true,
            "owner": {
                "name": "Alex Wilber",
                "address": "AlexW@contoso.OnMicrosoft.com"
            }
        }
    ]
}
```

> **ПРИМЕЧАНИЕ** Войдя в систему под именем Анны, вы также можете получить делегированный календарь непосредственно из почтового ящика Артема, указав идентификатор Артема и ярлык `calendar` в соответствии с `GET https://graph.microsoft.com/v1.0/users/AlexW@contoso.OnMicrosoft.com/calendar`. Возвращенный код календаря соответствует почтовому ящику Артема. 

## <a name="step-2-adele-creates-and-sends-an-invitation-on-alex-behalf"></a>Шаг 2. Анна создает и отправляет приглашение от имени Артема

Войдя в систему под именем Анны, используйте код календаря, полученный на шаге 1, чтобы создать [событие](/graph/api/resources/event) в делегированном календаре и отправить его Алене и Марте от имени Артема.

**Разрешения Microsoft Graph**

Для этой операции необходимо использовать подходящее разрешение делегирования, `Calendars.ReadWrite.Shared`. Дополнительные сведения см. в разделе [Разрешения календаря](permissions-reference.md#calendars-permissions).

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADRpAABf0JlzAAA="],
  "name": "create_send_invitation"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendars/AAMkADRpAABf0JlzAAA=/events

Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json

{
  "subject": "Christmas dinner",
  "body": {
    "contentType": "HTML",
    "content": "Happy holidays!"
  },
  "start": {
      "dateTime": "2019-12-25T18:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2019-12-25T22:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "location":{
      "displayName":"Alex' home"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"meganb@contoso.onmicrosoft.com",
        "name": "Megan Bowen"
      },
      "type": "required"
    },
    {
      "emailAddress": {
        "address":"ChristieC@contoso.onmicrosoft.com",
        "name": "Christie Cline"
      },
      "type": "required"
    }
  ]
}
```

Обратите внимание, что успешный ответ включает код HTTP 201, а также следующие свойства [события](/graph/api/resources/event):

- **isOrganizer** имеет значение "true". Это свойство обычно имеет значение "true", если владелец календаря (Артем) является организатором собрания. Это также применимо, если делегат (Анна) организовала собрание от имени владельца. 
- В коллекции **attendees** указаны Алена и Марта.
- **organizer** имеет значение "Артем", так как приглашение было отправлено делегатом Артема (Анной) для его основного календаря.
- Ни в коллекции **attendees**, ни в свойстве **organizer** не указан делегат (Анна).

<!-- {
  "blockType": "response",
  "name": "create_send_invitation",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69')/calendars('AAMkADRpAABf0JlzAAA%3D')/events/$entity",
    "@odata.etag": "W/\"NDznl+Uh50WkanaCOKHkaQAAX8m47Q==\"",
    "id": "AAMkADI4oeRpAABf0LrcAAA=",
    "createdDateTime": "2019-12-21T04:59:01.9766929Z",
    "lastModifiedDateTime": "2019-12-21T04:59:02.0214967Z",
    "changeKey": "NDznl+Uh50WkanaCOKHkaQAAX8m47Q==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "iCalUId": "040000008200FEFE0BA532444B5FD89BDE22BA103",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": false,
    "hasAttachments": false,
    "subject": "Christmas dinner",
    "bodyPreview": "Happy holidays!",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADI4oeRpAABf0LrcAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "recurrence": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nHappy holidays!\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2019-12-25T18:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "end": {
        "dateTime": "2019-12-25T22:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "location": {
        "displayName": "Alex' home",
        "locationType": "default",
        "uniqueId": "Alex' home",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Alex' home",
            "locationType": "default",
            "uniqueId": "Alex' home",
            "uniqueIdType": "private"
        }
    ],
    "attendees": [
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Megan Bowen",
                "address": "MeganB@contoso.OnMicrosoft.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Christie Cline",
                "address": "ChristieC@contoso.OnMicrosoft.com"
            }
        }
    ],
    "organizer": {
        "emailAddress": {
            "name": "Alex Wilber",
            "address": "AlexW@contoso.OnMicrosoft.com"
        }
    }
}
```


## <a name="step-3-christie-receives-meeting-request-and-inspects-the-associated-event-in-her-calendar"></a>Шаг 3. Алена получает приглашение на собрание и изучает соответствующее событие в своем календаре

Доставив приглашение на собрание, Outlook автоматически создает [событие](/graph/api/resources/event) под вопросом в календаре Алены.

Войдя в систему под именем Алены, получите [eventMessage](/graph/api/resources/eventmessage) и **event**, связанные с приглашением на собрание на шаге 2.

**Разрешения Microsoft Graph**

Воспользуйтесь делегированным разрешением с минимальными правами `Mail.Read` и `Calendar.Read.Shared`. Дополнительные сведения см. в разделе [Разрешения почты](permissions-reference.md#mail-permissions) и [Разрешения календаря](permissions-reference.md#calendars-permissions).


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADADVj3fyAABZ5hYdAAA="],
  "name": "get_eventmessage_and_event"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADADVj3fyAABZ5hYdAAA=?$expand=microsoft.graph.eventMessage/event
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-eventmessage-and-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-eventmessage-and-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-eventmessage-and-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-eventmessage-and-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


Обратите внимание, что успешный отклик включает код ответа HTTP 200, а также следующие свойства [eventMessage](/graph/api/resources/eventmessage):

- **meetingMessageType** определяет это сообщение как `meetingRequest`.
- **sender** — Анна.
- **from** — Артем.
- **toRecipients** — Марта и Алена.

[Событие](/graph/api/resources/event) имеет следующие свойства:

- **attendees** — Артем, Марта и Алена.
- **organizer** — Артем.

Идентификатор Анны указывается только в свойстве **sender** **eventMessage** и не указывается в связанном с ним **событии**.

<!-- {
  "blockType": "response",
  "name": "get_message",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventmessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('662b947c-d9a1-4064-926c-eba1316d4462')/messages(microsoft.graph.eventMessage/event())/$entity",
    "@odata.type": "#microsoft.graph.eventMessage",
    "@odata.etag": "W/\"CwAAABYAAADK82uJYVo4RrFV3ADVj3fyAABZ378h\"",
    "id": "AAMkADADVj3fyAABZ5hYdAAA=",
    "createdDateTime": "2019-12-21T04:59:03Z",
    "lastModifiedDateTime": "2019-12-21T04:59:04Z",
    "changeKey": "CwAAABYAAADK82uJYVo4RrFV3ADVj3fyAABZ378h",
    "categories": [],
    "receivedDateTime": "2019-12-21T04:59:03Z",
    "sentDateTime": "2019-12-21T04:59:01Z",
    "hasAttachments": false,
    "internetMessageId": "<DM6PR17MB3593711A1C0A098167F5A977A12C0@DM6PR17MB3593.namprd17.prod.outlook.com>",
    "subject": "Christmas dinner",
    "bodyPreview": "Happy holidays!",
    "importance": "normal",
    "parentFolderId": "AQMkADIAAAIBDAAAAA==",
    "conversationId": "AAQkADNqQlzYAM8jQM=",
    "conversationIndex": "AdW3u1xx5S7TYrbluE2pCXNgAzyNAw==",
    "isDeliveryReceiptRequested": null,
    "isReadReceiptRequested": false,
    "isRead": true,
    "isDraft": false,
    "webLink": "https://outlook.office365.com/owa/?ItemID=AAMkADADVj3fyAABZ5hYdAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification": "focused",
    "meetingMessageType": "meetingRequest",
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nHappy holidays!\r\n</body>\r\n</html>\r\n"
    },
    "sender": {
        "emailAddress": {
            "name": "Adele Vance",
            "address": "AdeleV@contoso.OnMicrosoft.com"
        }
    },
    "from": {
        "emailAddress": {
            "name": "Alex Wilber",
            "address": "AlexW@contoso.OnMicrosoft.com"
        }
    },
    "toRecipients": [
        {
            "emailAddress": {
                "name": "Megan Bowen",
                "address": "MeganB@contoso.OnMicrosoft.com"
            }
        },
        {
            "emailAddress": {
                "name": "Christie Cline",
                "address": "ChristieC@contoso.OnMicrosoft.com"
            }
        }
    ],
    "ccRecipients": [],
    "bccRecipients": [],
    "replyTo": [],
    "flag": {
        "flagStatus": "notFlagged"
    },
    "event": {
        "@odata.etag": "W/\"yvNriWFaOEaxVdwA1Y938gAAX+T7Jg==\"",
        "id": "AAMkADADVj3fyAABZ5ieyAAA=",
        "createdDateTime": "2019-12-21T04:59:03.4336242Z",
        "lastModifiedDateTime": "2019-12-27T01:38:32.3766961Z",
        "changeKey": "yvNriWFaOEaxVdwA1Y938gAAX+T7Jg==",
        "categories": [],
        "originalStartTimeZone": "Pacific Standard Time",
        "originalEndTimeZone": "Pacific Standard Time",
        "iCalUId": "040000008200FEFE0BA532444B5FD89BDE22BA103",
        "reminderMinutesBeforeStart": 15,
        "isReminderOn": true,
        "hasAttachments": false,
        "subject": "Christmas dinner",
        "bodyPreview": "Happy holidays!",
        "importance": "normal",
        "sensitivity": "normal",
        "isAllDay": false,
        "isCancelled": false,
        "isOrganizer": false,
        "responseRequested": true,
        "seriesMasterId": null,
        "showAs": "tentative",
        "type": "singleInstance",
        "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADADVj3fyAABZ5ieyAAA%3D&exvsurl=1&path=/calendar/item",
        "onlineMeetingUrl": null,
        "recurrence": null,
        "responseStatus": {
            "response": "none",
            "time": "2019-12-21T05:16:48.8931825Z"
        },
        "body": {
            "contentType": "html",
            "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nHappy holidays!\r\n</body>\r\n</html>\r\n"
        },
        "start": {
            "dateTime": "2019-12-26T02:00:00.0000000",
            "timeZone": "UTC"
        },
        "end": {
            "dateTime": "2019-12-26T06:00:00.0000000",
            "timeZone": "UTC"
        },
        "location": {
            "displayName": "Alex' home",
            "locationType": "default",
            "uniqueId": "Alex' home",
            "uniqueIdType": "private"
        },
        "locations": [
            {
                "displayName": "Alex' home",
                "locationType": "default",
                "uniqueId": "1396aaf3-e344-4567-a4e3-797557ec24c8",
                "uniqueIdType": "locationStore"
            }
        ],
        "attendees": [
            {
                "type": "required",
                "status": {
                    "response": "none",
                    "time": "0001-01-01T00:00:00Z"
                },
                "emailAddress": {
                    "name": "Alex Wilber",
                    "address": "AlexW@contoso.OnMicrosoft.com"
                }
            },
            {
                "type": "required",
                "status": {
                    "response": "none",
                    "time": "0001-01-01T00:00:00Z"
                },
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.OnMicrosoft.com"
                }
            },
            {
                "type": "required",
                "status": {
                    "response": "none",
                    "time": "0001-01-01T00:00:00Z"
                },
                "emailAddress": {
                    "name": "Christie Cline",
                    "address": "ChristieC@contoso.OnMicrosoft.com"
                }
            }
        ],
        "organizer": {
            "emailAddress": {
                "name": "Alex Wilber",
                "address": "AlexW@contoso.OnMicrosoft.com"
            }
        }
    }
}
```


## <a name="step-4-christie-responds-to-the-meeting-request"></a>Шаг 4. Алена отвечает на приглашение на собрание

Войдя в учетную запись под именем Алены, ответьте на **событие** как "Под вопросом" и включите в отклик ответное сообщение.

**Разрешения Microsoft Graph**

Для этой операции необходимо использовать подходящее разрешение делегирования, `Calendars.ReadWrite.Shared`. Дополнительные сведения см. в разделе [Разрешения календаря](permissions-reference.md#calendars-permissions).

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADADVj3fyAABZ5ieyAAA="],
  "name": "event_reply_tentativelyaccept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/AAMkADADVj3fyAABZ5ieyAAA=/tentativelyAccept
Content-type: application/json

{
  "comment": "I will probably be able to make it.",
  "sendResponse": true
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-reply-tentativelyaccept-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-reply-tentativelyaccept-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-reply-tentativelyaccept-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-reply-tentativelyaccept-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


Успешный отклик возвращает код HTTP 202 Принято.

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```


## <a name="step-5-adele-receives-the-response-message"></a>Шаг 5. Анна получает ответное сообщение

Анна является делегатом для основного календаря Артема, поэтому она получает все ответы на приглашения на собрание для этого календаря от имени Артема.

Войдя в систему под именем Анны, получите объект [eventMessage](/graph/api/resources/eventmessage), представляющий ответ Алены на шаге 4.

**Разрешения Microsoft Graph**

Для этой операции необходимо использовать подходящее разрешение делегирования, `Mail.Read.Shared`. Дополнительные сведения см. в разделе [Разрешения почты](permissions-reference.md#mail-permissions).


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADI4oeRpAABf0HJUAAA="],
  "name": "message_get_reply"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADI4oeRpAABf0HJUAAA=
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-get-reply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-get-reply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-get-reply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-get-reply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


Обратите внимание, что успешный отклик включает код ответа HTTP 200, а также следующие свойства [eventMessage](/graph/api/resources/eventmessage):

- **meetingMessageType** имеет значение `meetingTenativelyAccepted`.
- **from** — Алена.
- **toRecipients** включает Анну, но не включает владельца календаря, Артема. Это связано с тем, что Артем сохранил значение по умолчанию, позволяющее Outlook направлять все ответы на приглашения на собрание только делегатам.

<!-- {
  "blockType": "response",
  "name": "message_get_reply",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventmessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69')/messages/$entity",
    "@odata.type": "#microsoft.graph.eventMessage",
    "@odata.etag": "W/\"DAAAABYAAAA0POeX5SHnRaRqdoI4oeRpAABfybkT\"",
    "id": "AAMkADI4oeRpAABf0HJUAAA=",
    "createdDateTime": "2019-12-21T05:16:55Z",
    "lastModifiedDateTime": "2019-12-21T05:16:57Z",
    "changeKey": "DAAAABYAAAA0POeX5SHnRaRqdoI4oeRpAABfybkT",
    "categories": [],
    "receivedDateTime": "2019-12-21T05:16:56Z",
    "sentDateTime": "2019-12-21T05:16:49Z",
    "hasAttachments": false,
    "internetMessageId": "<86880ccb8ec64184996e46eaddaed279@DM6PR17MB3593.namprd17.prod.outlook.com>",
    "subject": "Tentative: Christmas dinner",
    "bodyPreview": "I will probably be able to make it.",
    "importance": "normal",
    "parentFolderId": "AQMkAD5GkAAAIBDAAAAA==",
    "conversationId": "AAQkADK25bhNqQlzYAM8jQM=",
    "conversationIndex": "AdW3u1xx5S7TYrbluE2pCXNgAzyNAwAAoBoZ",
    "isDeliveryReceiptRequested": null,
    "isReadReceiptRequested": false,
    "isRead": false,
    "isDraft": false,
    "webLink": "https://outlook.office365.com/owa/?ItemID=AAMkADI4oeRpAABf0HJUAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification": "focused",
    "meetingMessageType": "meetingTenativelyAccepted",
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nI will probably be able to make it.\r\n</body>\r\n</html>\r\n"
    },
    "sender": {
        "emailAddress": {
            "name": "Christie Cline",
            "address": "ChristieC@contoso.OnMicrosoft.com"
        }
    },
    "from": {
        "emailAddress": {
            "name": "Christie Cline",
            "address": "ChristieC@contoso.OnMicrosoft.com"
        }
    },
    "toRecipients": [
        {
            "emailAddress": {
                "name": "Adele Vance",
                "address": "AdeleV@contoso.OnMicrosoft.com"
            }
        }
    ],
    "ccRecipients": [],
    "bccRecipients": [],
    "replyTo": [],
    "flag": {
        "flagStatus": "notFlagged"
    }
}
```

## <a name="step-6-alex-accesses-responses-as-part-of-the-event"></a>Шаг 6. Артем получает доступ к ответам в рамках события

Артем сохранил значение по умолчанию, позволяющее Outlook направлять все приглашения на собрание и ответы только делегатам, поэтому он не получает ответ Алены на шаге 4. Однако он может получить ответ с помощью [события](/graph/api/resources/event) в своем основном календаре.

Войдя в систему под именем Артема, получите [событие](/graph/api/resources/event), созданное Анной на шаге 2, а также отклики свойства **attendees**.

**Разрешения Microsoft Graph**

Для этой операции необходимо использовать подходящее разрешение делегирования, `Calendars.Read`. Дополнительные сведения см. в разделе [Разрешения календаря](permissions-reference.md#calendars-permissions).


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADJXJGu0AABf02qwAAA="],
  "name": "event_get_responses"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendar/events/AAMkADJXJGu0AABf02qwAAA=
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-get-responses-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-get-responses-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-get-responses-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-get-responses-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


Обратите внимание, что успешный отклик включает код ответа HTTP 200, а также следующие свойства [события](/graph/api/resources/event):

- **isOrganizer** имеет значение "true".
- **attendees** — только Марта и Алена.
- В свойстве **status** каждого экземпляра **attendee** указан ответ участника.
  - Ответ Марты — `none`.
  - Ответ Алены — `tentativelyAccepted`.
- **organizer** — Артем.
- В свойствах возвращенного **события** не указывается делегат, Анна.

<!-- {
  "blockType": "response",
  "name": "event_get_responses",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/calendars('AQMkADAw7QAAAJfygAAAA%3D%3D')/events/$entity",
    "@odata.etag": "W/\"NEXywgsVrkeNsFsyVyRrtAAAX8xuhA==\"",
    "id": "AAMkADJXJGu0AABf02qwAAA=",
    "createdDateTime": "2019-12-21T04:59:01.4435895Z",
    "lastModifiedDateTime": "2019-12-21T05:16:54.689345Z",
    "changeKey": "NEXywgsVrkeNsFsyVyRrtAAAX8xuhA==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "iCalUId": "040000008200FEFE0BA532444B5FD89BDE22BA103",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Christmas dinner",
    "bodyPreview": "Happy holidays!",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADJXJGu0AABf02qwAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "recurrence": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nHappy holidays!\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2019-12-26T02:00:00.0000000",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2019-12-26T06:00:00.0000000",
        "timeZone": "UTC"
    },
    "location": {
        "displayName": "Alex' home",
        "locationType": "default",
        "uniqueId": "Alex' home",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Alex' home",
            "locationType": "default",
            "uniqueId": "Alex' home",
            "uniqueIdType": "private"
        }
    ],
    "attendees": [
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Megan Bowen",
                "address": "MeganB@contoso.OnMicrosoft.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "tentativelyAccepted",
                "time": "2019-12-21T05:16:48.8931825Z"
            },
            "emailAddress": {
                "name": "Christie Cline",
                "address": "ChristieC@contoso.OnMicrosoft.com"
            }
        }
    ],
    "organizer": {
        "emailAddress": {
            "name": "Alex Wilber",
            "address": "AlexW@contoso.OnMicrosoft.com"
        }
    }
}
```


## <a name="next-steps"></a>Дальнейшие действия

Дополнительные сведения:

- [Получение событий Outlook из общего или делегированного календаря](outlook-get-shared-events-calendars.md)
- [Предоставление общего доступа к календарю или его делегирование в Outlook (предварительная версия)](outlook-share-or-delegate-calendar.md)
- [Зачем выполнять интеграцию с Календарем Outlook?](outlook-calendar-concept-overview.md)
- [API календаря](/graph/api/resources/calendar) в Microsoft Graph 1.0
