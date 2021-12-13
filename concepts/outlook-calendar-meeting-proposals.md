---
title: Предложение нового времени собрания в Outlook
description: В Outlook организатор собрания может разрешить приглашенным предлагать другое время собрания.
author: harini84
ms.localizationpriority: high
ms.prod: outlook
ms.openlocfilehash: 75eb225da1cc1ea337b20e07a8429e9acdd32748
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424618"
---
# <a name="propose-new-meeting-times-in-outlook"></a>Предложение нового времени собрания в Outlook

В Outlook организатор собрания может разрешить приглашенным предлагать другое время собрания, если им не подходит исходное время и дата и они отклоняют или принимают приглашение под вопросом. Организатор может принять предложение, изменив время собрания соответствующим образом.

## <a name="example-attendee-responds-tentative-and-suggests-a-different-datetime"></a>Пример: участник принимает приглашение под вопросом и предлагает другую дату и время
Ниже приведен пример, в котором Алекс (Alex) приглашает Адель (Adele) на обед, Адель принимает приглашение под вопросом и предлагает другую дату и время, а Алекс принимает предложение, изменяя собрание соответствующим образом:

1. Алекс в качестве организатора отправляет Адель приглашение на собрание. Он присваивает свойству **allowNewTimeProposals** объекта [event](/graph/api/resources/event) значение `true`, чтобы разрешить Адель предложить другое время при необходимости.

    <!-- {
      "blockType": "request",
      "name": "create_event"
    }-->
    ```http
    POST https://graph.microsoft.com/v1.0/me/events
    Prefer: outlook.timezone="Pacific Standard Time"
    Content-type: application/json

    {
      "subject": "Let's go for lunch",
      "body": {
        "contentType": "HTML",
        "content": "Does noon work for you?"
      },
      "start": {
          "dateTime": "2019-08-15T12:00:00",
          "timeZone": "Pacific Standard Time"
      },
      "end": {
          "dateTime": "2019-08-15T14:00:00",
          "timeZone": "Pacific Standard Time"
      },
      "allowNewTimeProposals": true,
      "location":{
          "displayName":"Harry's Bar"
      },
      "attendees": [
        {
          "emailAddress": {
          "address":"AdeleV@contoso.OnMicrosoft.com",
          "name": "Adele Vance"
          },
          "type": "required"
        }
      ]
    }
    ```

    Алекс получает следующий ответ: 
    <!-- {
      "blockType": "response",
      "name": "create_event",
      "truncated": true,
      "@odata.type": "microsoft.graph.event"
    } -->
    ```http
    HTTP/1.1 201 Created
    Content-type: application/json

    {
      "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/events/$entity",
      "@odata.etag": "W/\"NEXywgsVrkeNsFsyVyRrtAAAAhBhkg==\"",
      "id": "AAMkADAwJXJGu0AAACEhWOAAA=",
      "createdDateTime": "2019-08-01T06:41:07.805128Z",
      "lastModifiedDateTime": "2019-08-01T06:41:08.3298275Z",
      "changeKey": "NEXywgsVrkeNsFsyVyRrtAAAAhBhkg==",
      "categories": [],
      "originalStartTimeZone": "Pacific Standard Time",
      "originalEndTimeZone": "Pacific Standard Time",
      "reminderMinutesBeforeStart": 15,
      "isReminderOn": true,
      "hasAttachments": false,
      "subject": "Let's go for lunch",
      "bodyPreview": "Does noon work for you?",
      "importance": "normal",
      "sensitivity": "normal",
      "isAllDay": false,
      "isCancelled": false,
      "isOrganizer": true,
      "responseRequested": true,
      "seriesMasterId": null,
      "showAs": "busy",
      "type": "singleInstance",
      "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADAwJXJGu0AAACEhWOAAA%3D&exvsurl=1&path=/calendar/item",
      "onlineMeetingUrl": null,
      "allowNewTimeProposals": true,
      "recurrence": null,
      "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
      },
      "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes late morning work for you?\r\n</body>\r\n</html>\r\n"
      },
      "start": {
        "dateTime": "2019-08-15T12:00:00.0000000",
        "timeZone": "Pacific Standard Time"
      },
      "end": {
        "dateTime": "2019-08-15T14:00:00.0000000",
        "timeZone": "Pacific Standard Time"
      },
      "location": {
        "displayName": "Harry's Bar",
        "locationType": "default",
        "uniqueId": "Harry's Bar",
        "uniqueIdType": "private"
      },
     "locations": [
        {
            "displayName": "Harry's Bar",
            "locationType": "default",
            "uniqueId": "Harry's Bar",
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
                "name": "Adele Vance",
                "address": "AdeleV@contoso.OnMicrosoft.com"
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

2. Адель получает приглашение в папке "Входящие" в виде объекта [eventMessageRequest](/graph/api/resources/eventmessagerequest). Она замечает, что настроено свойство **allowNewTimeProposals**. [Используя объект **event**, связанный](/graph/api/eventmessage-get#example-2) с этим ресурсом **eventMessageRequest**, она принимает приглашение под вопросом и предлагает такое же время на следующий день в параметре текста **proposedNewTime**. Она также присваивает параметру **sendResponse** значение true.

    <!-- {
      "blockType": "request",
      "name": "event_tentativelyaccept"
    }-->
    ```http
    POST https://graph.microsoft.com/v1.0/me/events/AAMkADU5NRaRqdoI4oeRpAAAB_woNAAA=/tentativelyAccept
    Content-type: application/json

    { 
      "comment": "Can you make the next day instead?", 
      "sendResponse": "true", 
      "proposedNewTime": {
         "Start": { 
              "DateTime": "2019-08-16T12:00:00", 
              "TimeZone": "Pacific Standard Time" 
         }, 
         "End": { 
              "DateTime": "2019-08-16T14:00:00", 
              "TimeZone": "Pacific Standard Time" 
         }
      }
    } 
    ```

    Ответ Адель успешно отправляется, и она получает следующий отклик:

    <!-- {
      "blockType": "response",
      "name": "event_tentativelyaccept"
      "truncated": true
    } -->
    ```http
    HTTP/1.1 202 Accepted
    ```

3. Алекс получает письмо типа [eventMessageResponse](/graph/api/resources/eventmessageresponse). Он замечает следующее:

   - Тема содержит префикс и фразу "Предложено новое время: Давайте пообедаем"
   - Отправитель — Адель Вэнс (Adele Vance)
   - Свойству **responseType** присвоено значение `tentativelyAccepted`
   - Предложение Адель указывается в свойстве **proposedNewTime** объекта **eventMessageResponse**

    <!-- {
      "blockType": "request",
      "name": "get_messages"
    }-->
    ```http
    GET https://graph.microsoft.com/v1.0/me/messages?$top=1
    Prefer: outlook.timezone="Pacific Standard Time"
    ```

    Для наглядности предположим, что ответ Адель является последним сообщением в почтовом ящике Алекса, и Алекс может просто запросить это последнее сообщение.

    <!-- {
      "blockType": "response",
      "name": "get_messages",
      "truncated": true,
      "@odata.type": "microsoft.graph.message",
      "isCollection": true
    } -->
    ```http
    HTTP/1.1 200 OK
    Content-type: application/json
    Preference-Applied: outlook.timezone="Pacific Standard Time"

    {
       "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/messages",
       "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/messages?$top=1&$skip=4"",
       "value": [
          {
            "@odata.type": "#microsoft.graph.eventMessageResponse",
            "@odata.etag": "W/\"DAAAABYAAAA0RfLCCxWuR42wWzJXJGu0AAACEGHC\"",
            "id": "AAMkADAwJXJGu0AAACEiVAAAA=",
            "createdDateTime": "2019-08-01T07:06:27Z",
            "lastModifiedDateTime": "2019-08-01T07:06:28Z",
            "changeKey": "DAAAABYAAAA0RfLCCxWuR42wWzJXJGu0AAACEGHC",
            "categories": [],
            "receivedDateTime": "2019-08-01T07:06:28Z",
            "sentDateTime": "2019-08-01T07:06:24Z",
            "hasAttachments": false,
            "internetMessageId": "<BY5PR17MB38759D33B8925D525A476F33D9DE0@contoso.outlook.com>",
            "subject": "New Time Proposed: Let's go for lunch",
            "bodyPreview": "Can you make the next day instead?",
            "importance": "normal",
            "parentFolderId": "AQMkADAwQAAAIBDAAAAA==",
            "conversationId": "AAQkADAwQAQAMkh89RO3QpBiUCETTtVbIo=",
            "conversationIndex": "AdVINBlgySHz1E7dCkGJQIRNO1VsigAA4n6R",
            "isDeliveryReceiptRequested": null,
            "isReadReceiptRequested": false,
            "isRead": false,
            "isDraft": false,
            "webLink": "https://outlook.office365.com/owa/?ItemID=AAMkADAwJXJGu0AAACEiVAAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
            "inferenceClassification": "focused",
            "unsubscribeData": [],
            "unsubscribeEnabled": false,
            "meetingMessageType": "meetingTentativelyAccepted",
            "type": "singleInstance",
            "isOutOfDate": false,
            "isAllDay": false,
            "isDelegated": false,
            "responseType": "tentativelyAccepted",
            "recurrence": null,
            "body": {
                "contentType": "html",
                "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nCan you make the next day instead?\r\n</body>\r\n</html>\r\n"
            },
            "sender": {
                "emailAddress": {
                    "name": "Adele Vance",
                    "address": "AdeleV@contoso.OnMicrosoft.com"
                }
            },
            "from": {
                "emailAddress": {
                    "name": "Adele Vance",
                    "address": "AdeleV@contoso.OnMicrosoft.com"
                }
            },
            "toRecipients": [
                {
                    "emailAddress": {
                        "name": "Alex Wilber",
                        "address": "AlexW@contoso.OnMicrosoft.com"
                    }
                }
            ],
            "ccRecipients": [],
            "bccRecipients": [],
            "replyTo": [],
            "flag": {
                "flagStatus": "notFlagged"
            },
            "startDateTime": {
                "dateTime": "2019-08-15T12:00:00.0000000",
                "timeZone": "Pacific Standard Time"
            },
            "endDateTime": {
                "dateTime": "2019-08-15T14:00:00.0000000",
                "timeZone": "Pacific Standard Time"
            },
            "location": {
                "displayName": "Harry's Bar",
                "locationType": "default",
                "uniqueIdType": "unknown"
            },
            "proposedNewTime": {
                "start": {
                    "dateTime": "2019-08-16T12:00:00", 
                    "timeZone": "Pacific Standard Time"
                },
                "end": {
                    "dateTime": "2019-08-16T14:00:00", 
                    "timeZone": "Pacific Standard Time"
                }
            }
         }
        ]
    }
    ```

4. Алекс также замечает, что **событие** для обеда теперь включает свойство **proposedNewTime**, содержащее предложение Адель. Это свойство представлено в составе экземпляра [attendee](/graph/api/resources/attendee), только если соответствующий участник предложил другое время собрания. 

    <!-- {
      "blockType": "request",
      "name": "event_get"
    }-->
    ```http
    GET https://graph.microsoft.com/v1.0/me/events/AAMkADAwJXJGu0AAACEhWOAAA=?$select=subject,allowNewTimeProposals,start,end,attendees,organizer
    Prefer: outlook.timezone="Pacific Standard Time"
    ```

    <!-- {
      "blockType": "response",
      "name": "event_get",
      "truncated": true,
      "@odata.type": "microsoft.graph.event"
    } -->
    ```http
    HTTP/1.1 200 Ok

    {
        "@odata.context": "https://graph.microsoft.com/testexchangev1.0/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/events(subject,allowNewTimeProposals,start,end,attendees,organizer)/$entity",
        "@odata.etag": "W/\"NEXywgsVrkeNsFsyVyRrtAAAAhEDMA==\"",
        "id": "AAMkADAwJXJGu0AAACEhWOAAA=",
        "subject": "Let's go for lunch",
        "allowNewTimeProposals": true,
        "start": {
            "dateTime": "2019-08-15T12:00:00.0000000",
            "timeZone": "Pacific Standard Time"
        },
        "end": {
            "dateTime": "2019-08-15T14:00:00.0000000",
            "timeZone": "Pacific Standard Time"
        },
        "attendees": [
            {
                "type": "required",
                "status": {
                    "response": "tentativelyAccepted",
                    "time": "2019-08-01T07:06:24.5046431Z"
                },
                "proposedNewTime": {
                    "start": {
                        "dateTime": "2019-08-16T12:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    },
                    "end": {
                        "dateTime": "2019-08-16T14:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    }
                },
                "emailAddress": {
                    "name": "Adele Vance",
                    "address": "AdeleV@contoso.OnMicrosoft.com"
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


5. Алекс решает принять предложение Адель, обновив **событие** с использованием предложенной даты и времени **начала** и **окончания**.

    <!-- {
      "blockType": "request",
      "name": "event_update"
    }-->
    ```http
    PATCH https://graph.microsoft.com/v1.0/me/events/AAMkADAwJXJGu0AAACEhWOAAA=
    Prefer: outlook.timezone="Pacific Standard Time"
    Content-type: application/json

    {
        "start": {
            "dateTime": "2019-08-16T12:00:00.0000000",
            "timeZone": "Pacific Standard Time"
        },
        "end": {
            "dateTime": "2019-08-16T14:00:00.0000000",
            "timeZone": "Pacific Standard Time"
        }
    }
    ```

    Обновление Алекса успешно выполняется, и он получает следующий отклик.

    <!-- {
      "blockType": "response",
      "name": "event_update",
      "truncated": true,
      "@odata.type": "microsoft.graph.event"
    } -->
    ```http
    HTTP/1.1 200 Ok

    {
      "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/events/$entity",
      "@odata.etag": "W/\"NEXywgsVrkeNsFsyVyRrtAAAAhBizA==\"",
      "id": "AAMkADAwJXJGu0AAACEhWOAAA=",
      "createdDateTime": "2019-08-01T06:41:07.805128Z",
      "lastModifiedDateTime": "2019-08-01T08:21:43.5696529Z",
      "changeKey": "NEXywgsVrkeNsFsyVyRrtAAAAhBizA==",
      "categories": [],
      "originalStartTimeZone": "Pacific Standard Time",
      "originalEndTimeZone": "Pacific Standard Time",
      "reminderMinutesBeforeStart": 15,
      "isReminderOn": true,
      "hasAttachments": false,
      "subject": "Let's go for lunch",
      "bodyPreview": "Does noon work for you?",
      "importance": "normal",
      "sensitivity": "normal",
      "isAllDay": false,
      "isCancelled": false,
      "isOrganizer": true,
      "responseRequested": true,
      "seriesMasterId": null,
      "showAs": "busy",
      "type": "singleInstance",
      "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADAwJXJGu0AAACEhWOAAA%3D&exvsurl=1&path=/calendar/item",
      "onlineMeetingUrl": null,
      "allowNewTimeProposals": true,
      "recurrence": null,
      "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
      },
      "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes noon work for you?\r\n</body>\r\n</html>\r\n"
      },
      "start": {
        "dateTime": "2019-08-16T12:00:00.0000000",
        "timeZone": "Pacific Standard Time"
      },
      "end": {
        "dateTime": "2019-08-16T14:00:00.0000000",
        "timeZone": "Pacific Standard Time"
      },
      "location": {
        "displayName": "Harry's Bar",
        "locationType": "default",
        "uniqueId": "Harry's Bar",
        "uniqueIdType": "private"
      },
      "locations": [
        {
            "displayName": "Harry's Bar",
            "locationType": "default",
            "uniqueId": "Harry's Bar",
            "uniqueIdType": "private"
        }
      ],
      "attendees": [
        {
            "type": "required",
            "status": {
                "response": "notResponded",
                "time": "4501-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Adele Vance",
                "address": "AdeleV@contoso.OnMicrosoft.com"
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


## <a name="no-attendee-proposes-alternative-time"></a>Участники не предлагают другое время

На шаге 2, если Адель отклонила или приняла приглашение под вопросом и не предложила другое время и дату, произойдет следующее:

- На шаге 3 Алекс получит объект **eventMessageResponse** со значением `tentativelyAccepted` свойства **responseType** (или значением `decline`, если Адель отклонила приглашение). Алекс не обнаружит свойство **proposedNewTime** в этом экземпляре объекта **eventMessageResponse**.
- На шаге 4 Алекс также не обнаружит свойство **proposedNewTime** в связанном объекте **event**.

## <a name="see-also"></a>См. также
- [Поиск времени для проведения собрания в календаре Outlook](findmeetingtimes-example.md)
- [Получение расписания доступности пользователей и ресурсов](outlook-get-free-busy-schedule.md)
- [Планирование повторных встреч в качестве повторяющихся мероприятий в Outlook](outlook-schedule-recurring-events.md)
