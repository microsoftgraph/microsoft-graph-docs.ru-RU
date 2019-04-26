---
title: Обновление события
description: Обновление свойств объекта Event.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: ec274fb0e850a3a18b3722e27bbe394986459cbb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329808"
---
# <a name="update-event"></a>Обновление события

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [event](../resources/event.md) .
## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Calendars.ReadWrite    |
|Делегированные (личная учетная запись Майкрософт) | Calendars.ReadWrite    |
|Для приложений | Calendars.ReadWrite |

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

PATCH /me/calendargroup/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}

PATCH /me/calendargroups/{id}/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | строка  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Тело запроса
В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство       | Тип    | Описание |
|:---------------|:--------|:------------|
| attendees|Участник|Коллекция участников события.|
| body|ItemBody|Текст сообщения, связанного с событием.|
| categories|String|Категории, связанные с событием.|
| end|DateTimeTimeZone|Дата и время завершения события.<br/><br/>По умолчанию время завершения указано в формате UTC. Можно дополнительно указать часовой пояс в элементе EndTimeZone, задать время завершения согласно этому часовому поясу и UTC-смещение. Обратите внимание, что если вы используете EndTimeZone, следует также указать значение StartTimeZone.<br/><br/>Пример указания даты (25 февраля 2015 г., 21:34 по тихоокеанскому поясному времени): "2015-02-25T21:34:00-08:00". |
| importance|String|Важность события. Возможные значения: `low`, `normal`, `high`.|
| isAllDay|Логический|Задайте значение true, если событие длится весь день.|
| isReminderOn|Boolean|Задайте значение true, если установлено напоминание пользователю о событии.|
| location|Location|Место проведения события.|
|locations|Коллекция [Location](../resources/location.md)|Места проведения события или участия в нем. Свойства **location** и **locations** всегда совпадают друг с другом. Если вы обновите свойство **location**, предыдущие места в коллекции **locations** будут удалены и заменены новым значением **location**. |
| recurrence|PatternedRecurrence|Расписание повторения события.|
| reminderMinutesBeforeStart|Int32|Позволяет указать, за сколько минут до начала события появляется напоминание.|
| responseRequested|Boolean|Задайте значение true, если отправитель желает получить сообщение о согласии участвовать в событии или отклонении соответствующего приглашения.|
| sensitivity|String| Возможные значения: `normal`, `personal`, `private`, `confidential`.|
| showAs|String|Отображаемое состояние. Возможные `free` значения:, `tentative`, `busy`, `oof`, `workingElsewhere`,. `unknown`|
| start|DateTimeTimeZone|Время начала события. <br/><br/>По умолчанию время начала указано в формате UTC. Можно дополнительно указать часовой пояс в элементе StartTimeZone, задать время завершения согласно этому часовому поясу и UTC-смещение. Обратите внимание, что если вы используете StartTimeZone, следует также указать значение EndTimeZone.<br/><br/>Пример указания даты (25 февраля 2015 г., 19:34 по тихоокеанскому поясному времени): "2015-02-25T19:34:00-08:00".  |
| subject|String|Текст в строке темы сообщения о событии.|

Так как ресурс **event** поддерживает [расширения](/graph/extensibility-overview), с помощью `PATCH` операции можно добавлять, обновлять или удалять собственные данные, зависящие от приложения, в пользовательских свойствах расширения в существующем экземпляре **события** .

Если обновляемое **событие** является главным событием повторяющейся серии, содержит несколько участников и содержит экземпляры, которые были обновлены отдельно, будет отправлено несколько сообщений с уведомлениями: один для основных рядов и один для каждого экземпляра обновлены.

## <a name="response"></a>Отклик

В случае успеха этот метод возвратит код отклика `200 OK` и обновленный объект [event](../resources/event.md) в теле отклика.

>**Примечание:** Этот метод может возвращать ответ на ошибочный запрос HTTP 400 с кодом ошибки `ErrorOccurrenceCrossingBoundary` и следующим сообщением об ошибке: "измененное вхождение" пересекает или перекрывает смежное вхождение. Это указывает на то, что обновление нарушает следующее ограничение Outlook на количество исключений повторения: событие не может быть перемещено до или до дня предыдущего события и не может быть перемещено в следующий день или после него.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "update_event"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/events/{id}
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "recurrence": null,
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

##### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "recurrence": null,
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```


## <a name="see-also"></a>См. также

- [Добавление пользовательских данных в ресурсы с помощью расширений](/graph/extensibility-overview)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)](/graph/extensibility-open-users)
- [Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
