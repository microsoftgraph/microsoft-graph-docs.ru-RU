---
title: Обновление события
description: Обновление свойств объекта event.
author: harini84
ms.localizationpriority: high
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e3d2c62644adc05e61eb11ac6ef896f8d7ec64b9
ms.sourcegitcommit: 2e94beae05043a88b389349f0767e3a657415e4c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2021
ms.locfileid: "61123455"
---
# <a name="update-event"></a>Обновление события

Пространство имен: microsoft.graph

Обновление свойств объекта [event](../resources/event.md).

<!-- markdownlint-disable MD001 -->
### <a name="notes-for-updating-specific-properties"></a>Примечания для обновления определенных свойств

Обратите внимание на следующие действия и рекомендации при обновлении соответствующих свойств.

- Свойство **attendees** и обновления собраний
  - Обновление события, которое включает только свойство **attendees** в тексте запроса, отправляет обновление собрания только измененным участникам.
  - Обновление события, которое удаляет участника, указанного в списке рассылки, отправляет обновление собрания всем участникам.

- Свойство **body** и собрания по сети

  Перед обновлением текста события, настроенного в качестве собрания по сети, сначала получите свойство **body**, примените соответствующие изменения к содержимому и сохраните BLOB-объект собрания для собрания по сети. Случайное удаление BLOB-объекта собрания из текста отключит собрание по сети.

- Свойства **end** и **start**, а также соответствующие часовые пояса

  При обновлении часового пояса начала или завершения события сначала [найдите поддерживаемые часовые пояса](outlookuser-supportedtimezones.md), чтобы устанавливать только часовые пояса, настроенные для сервера почтового ящика пользователя.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Calendars.ReadWrite                 |
| Делегированные (личная учетная запись Майкрософт) | Calendars.ReadWrite                 |
| Для приложений                            | Calendars.ReadWrite                 |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/events/{id}
PATCH /users/{id | userPrincipalName}/events/{id}
PATCH /groups/{id}/events/{id}

PATCH /me/calendar/events/{id}
PATCH /users/{id | userPrincipalName}/calendar/events/{id}
PATCH /groups/{id}/calendar/events/{id}

PATCH /me/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}/events/{id}

PATCH /me/calendargroups/{id}/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Тип   | Описание               |
|:--------------|:-------|:--------------------------|
| Authorization | string | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса

[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

| Свойство                   | Тип                                                       | Описание |
|:---------------------------|:-----------------------------------------------------------|:----|
| attendees                  | [Attendee](../resources/attendee.md)                       | Коллекция участников события. |
| body                       | [ItemBody](../resources/itembody.md)                       | Текст сообщения, связанного с событием. |
| categories                 | Коллекция String                                          | Категории, связанные с событием. |
| end                        | DateTimeTimeZone                                           | Дата, время и часовой пояс завершения события. |
| hideAttendees              | Boolean                                                    | Если присвоено значение `true`, каждый участник видит только себя в приглашении на собрание и списке собрания **Отслеживание**. Значение по умолчанию: false. |
| importance                 | String                                                     | Важность события. Допустимые значения: `low`, `normal`, `high`. |
| isAllDay                   | Boolean                                                    | Задайте значение true, если событие длится весь день. |
| isOnlineMeeting            | Boolean                                                    | `True`, если это событие содержит информацию о собраниях по сети; в противном случае — `false`. Значение по умолчанию: false. Необязательно. |
| isReminderOn               | Boolean                                                    | Задайте значение true, если установлено напоминание пользователю о событии. |
| location                   | [Location](../resources/location.md)                       | Место проведения события. |
| locations                  | Коллекция [location](../resources/location.md)            | Места проведения мероприятия или участия в нем. Свойства **location** и **locations** всегда совпадают друг с другом. Если вы обновите свойство **location**, предыдущие места в коллекции **locations** будут удалены и заменены новым значением **location**. |
| onlineMeetingProvider      | onlineMeetingProviderType                                  | Представляет поставщика службы собраний по сети. Возможные значения: `teamsForBusiness`, `skypeForBusiness` и `skypeForConsumer`. Необязательно. |
| recurrence                 | [PatternedRecurrence](../resources/patternedrecurrence.md) | Расписание повторения события. |
| reminderMinutesBeforeStart | Int32                                                      | Позволяет указать, за сколько минут до начала события появляется напоминание. |
| responseRequested          | Boolean                                                    | Задайте значение true, если отправитель желает получить сообщение о согласии участвовать в событии или отклонении соответствующего приглашения. |
| sensitivity                | String                                                     | Допустимые значения: `normal`, `personal`, `private`, `confidential`. |
| showAs                     | String                                                     | Отображаемое состояние. Допустимые значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`. |
| начать                      | DateTimeTimeZone                                           | Дата, время и часовой пояс начала события. |
| subject                    | String                                                     | Текст в строке темы сообщения о событии. |

Так как ресурс **event** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `PATCH` можно добавлять, обновлять или удалять собственные данные, касающиеся определенных приложений, в настраиваемых свойствах расширения в существующем экземпляре **event**.

Если обновляемый ресурс **event** является главным событием повторяющегося ряда, содержит несколько участников и экземпляры, обновленные отдельно, отправляется несколько сообщений электронной почты с уведомлениями: одно для главного ряда и по одному для каждого обновленного экземпляра.

## <a name="response"></a>Отклик

В случае успеха этот метод возвратит код отклика `200 OK` и обновленный объект [event](../resources/event.md) в теле отклика.

>**Примечание.** Этот метод может вернуть отклик "HTTP 400 — ошибочный запрос" с кодом ошибки `ErrorOccurrenceCrossingBoundary` и следующим сообщением об ошибке: "Измененная копия пересекается со смежной копией или перекрывает ее". Это означает, что обновление нарушает следующее ограничение Outlook для повторяющихся исключений: повторение нельзя перемещать на день предыдущего повторения или до него, а также на день следующего повторения или после него.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- markdownlint-disable MD025 -->
# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "update_event"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/me/events/{id}
Content-type: application/json

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "recurrence": null,
  "reminderMinutesBeforeStart": 99,
  "isOnlineMeeting": true,
  "onlineMeetingProvider": "teamsForBusiness",
  "isReminderOn": true,
  "hideAttendees": false,
  "categories": ["Red category"]
}
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-event-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/update-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-event-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/update-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-event-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/update-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-event-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD024 -->

##### <a name="response"></a>Отклик

Ниже представлен пример отклика. Примечание: показанный здесь объект отклика может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "recurrence": null,
  "reminderMinutesBeforeStart": 99,
  "isOnlineMeeting": true,
  "onlineMeetingProvider": "teamsForBusiness",
  "isReminderOn": true,
  "hideAttendees": false,
  "onlineMeeting": {
        "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_NzIyNzhlMGEtM2YyZC00ZmY0LTlhNzUtZmZjNWFmZGNlNzE2%40thread.v2/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22bc55b173-cff6-457d-b7a1-64bda7d7581a%22%7d",
        "conferenceId": "177513992",
        "tollNumber": "+91 22 6241 6885"
  }
}
```

## <a name="see-also"></a>См. также

- [Добавление пользовательских данных в ресурсы с помощью расширений](/graph/extensibility-overview)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](/graph/extensibility-open-users)
- [Добавление пользовательских данных в группы с помощью расширений схемы](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
