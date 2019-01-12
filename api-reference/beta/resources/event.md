---
title: Тип ресурса event
description: Событие в календаре.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 3a42bd4c87b6c4d8cb26160ae3c36bc7d6380b79
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981149"
---
# <a name="event-resource-type"></a>Тип ресурса event

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Событие в календаре [пользователя](user.md) или календаря по умолчанию для [группы](group.md)с Office 365.

Этот ресурс поддерживает:

- Добавление настраиваемых свойств данные как [расширения](/graph/extensibility-overview).
- Подписка на [уведомления об изменении](/graph/webhooks).
- отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/event-delta.md)).

> **Примечание:** Существуют небольшие отличия таким способом, который может взаимодействовать с календарей пользователей, группы календарей и их событий:

 - Их можно организовать только календарей пользователей в [calendarGroup](calendargroup.md).
 - Outlook автоматически принимает все приглашения на собрания от имени группы. Для календарей _пользователей_ только можно [принять](../api/event-accept.md), [под вопросом принятие](../api/event-tentativelyaccept.md)или [отклонение](../api/event-decline.md) приглашения на собрания.
  - Outlook не поддерживает напоминания о событиях группы. Можно [отложить](../api/event-snoozereminder.md) или [отклонение](../api/event-dismissreminder.md) [напоминание](reminder.md) для только календарей _пользователей_ .

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "calendar",
    "extensions",
    "instances",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "@odata.type": "microsoft.graph.event"
}-->

```json
{
  "attendees": [{"@odata.type": "microsoft.graph.attendee"}],
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "bodyPreview": "string",
  "categories": ["string"],
  "changeKey": "string",
  "createdDateTime": "String (timestamp)",
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "hasAttachments": true,
  "iud": "string",
  "id": "string (identifier)",
  "importance": "String",
  "isAllDay": true,
  "isCancelled": true,
  "isOrganizer": true,
  "isReminderOn": true,
  "lastModifiedDateTime": "String (timestamp)",
  "location": {"@odata.type": "microsoft.graph.location"},
  "locations": [{"@odata.type": "microsoft.graph.location"}],
  "onlineMeetingUrl": "string",
  "organizer": {"@odata.type": "microsoft.graph.recipient"},
  "originalEndTimeZone": "string",
  "originalStart": "String (timestamp)",
  "originalStartTimeZone": "string",
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "reminderMinutesBeforeStart": 1024,
  "responseRequested": true,
  "responseStatus": {"@odata.type": "microsoft.graph.responseStatus"},
  "sensitivity": "String",
  "seriesMasterId": "string",
  "showAs": "String",
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "subject": "string",
  "type": "String",
  "webLink": "string",
  
  "attachments": [ { "@odata.type": "microsoft.graph.attachment" } ],
  "calendar": { "@odata.type": "microsoft.graph.calendar" },
  "extensions": [ { "@odata.type": "microsoft.graph.extension" } ],
  "instances": [ { "@odata.type": "microsoft.graph.event" }],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|attendees|Коллекция [ATTENDEE](attendee.md)|Коллекция участников события.|
|body|[ItemBody](itembody.md)|Текст сообщения, связанного с событием. В формате HTML или текстовом формате.|
|bodyPreview|Строка|Предварительный просмотр сообщения, связанного с событием. В текстовом формате.|
|categories|Коллекция String|Категории, связанные с событием. Каждой категории соответствует свойству **displayName** [outlookCategory](outlookcategory.md) , определенные для этого пользователя.|
|changeKey|String|Указывает версию объекта события. При каждом изменении события также меняется значение ChangeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|end|[DateTimeTimeZone](datetimetimezone.md)|Дата и время завершения события.|
|hasAttachments|Boolean|Задайте значение true, если у события есть вложения.|
|id|Строка| Только для чтения.|
|importance|String|Важность события. Возможные значения: `low`, `normal`, `high`.|
|isAllDay|Boolean|Задайте значение true, если событие длится весь день.|
|isCancelled|Boolean|Задайте значение true, если событие отменено.|
|isOrganizer|Boolean|Задайте значение true, если отправитель сообщения также является его организатором.|
|isReminderOn|Boolean|Задайте значение true, если установлено напоминание пользователю о событии.|
|lastModifiedDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|location|[Location](location.md)|Место проведения события.|
|locations|[Расположение](location.md) семейства сайтов|Места проведения мероприятия или участия в нем. Свойства **location** и **locations** всегда совпадают друг с другом. Если вы обновите свойство **location**, предыдущие места в коллекции **locations** будут удалены и заменены новым значением **location**. |
|onlineMeetingUrl|String|URL-адрес для собрания по сети. Свойство имеет значение только в том случае, когда инициатора задает событие как собрание, такие как Скайп. Только для чтения.|
|organizer|[Recipient](recipient.md)|Организатор события.|
|originalEndTimeZone|String|Часовой пояс завершения, указанный при создании события. Значение `tzone://Microsoft/Custom` указывает, что традиционный часовой пояс был задан в классическом приложении Outlook.|
|originalStart|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|originalStartTimeZone|Строка|Часовой пояс начала события, указанный при его создании. Значение `tzone://Microsoft/Custom` указывает, что в классическом приложении Outlook задан традиционный пользовательский часовой пояс.|
|recurrence|[PatternedRecurrence](patternedrecurrence.md)|Расписание повторения события.|
|reminderMinutesBeforeStart|Int32|Позволяет указать, за сколько минут до начала события появляется напоминание.|
|responseRequested|Boolean|Задайте значение true, если отправитель желает получить сообщение о согласии участвовать в событии или отклонении соответствующего приглашения.|
|responseStatus|[ResponseStatus](responsestatus.md)|Указывает тип отклика, отправленного в ответ на сообщение о событии.|
|sensitivity|String| Возможные значения: `normal`, `personal`, `private`, `confidential`.|
|seriesMasterId|String|Идентификатор для повторяющихся серии главных элемента, если это событие является частью серии повторяющихся.|
|showAs|String|Отображаемое состояние. Возможные значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.|
|start|[DateTimeTimeZone](datetimetimezone.md)|Время начала события.|
|subject|String|Текст в строке темы сообщения о событии.|
|type|String|Тип события. Возможные значения: `singleInstance`, `occurrence`, `exception`, `seriesMaster`. Только для чтения|
|ИД пользователя|String|Уникальный идентификатор, совместно используемый всеми экземплярами события в разных календарях. **Примечание:** это свойство выполняет те же функции, как `iCalUid` свойства [событий ресурсов](/graph/api/resources/event?view=graph-rest-1.0) на конечной версии 1.0, но не обязательно имеют одинаковые значения.|
|webLink|String|URL-адрес для открытия события в Outlook Web App.<br/><br/>Событие откроется в браузере, если вы вошли в свой почтовый ящик с помощью Outlook Web App. Если вход с помощью браузера еще не выполнен, вам будет предложено войти.<br/><br/>Доступ к этому URL-адресу можно получить из объекта iFrame.|

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|attachments|Коллекция объектов [attachment](attachment.md)|Коллекция [FileAttachment](fileattachment.md), [ItemAttachment](itemattachment.md)и [referenceAttachment](referenceattachment.md) вложений для события. Свойство навигации. Только для чтения. Допускается значение null.|
|calendar|[Calendar](calendar.md)|Календарь, который содержит событие. Свойство навигации. Только для чтения.|
|extensions|Коллекция [extension](extension.md)|Коллекция open расширения, определенные для события. Допускается значение null.|
|instances|Коллекция [Event](event.md)|Экземпляры события. Свойство навигации. Только для чтения. Допускается значение null.|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Коллекция расширенных свойств с несколькими значениями, определенных для события. Только для чтения. Допускается значение null.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Коллекция расширенных свойств с одним значением, определенных для события. Только для чтения. Допускается значение null.|

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список событий](../api/user-list-events.md)|Коллекция [Event](event.md) |Получение списка объектов [event](../resources/event.md) в почтовом ящике пользователя. В этом списке указаны единичные собрания и главные собрания в соответствующих сериях.|
|[Создание события](../api/user-post-events.md) |[event](event.md)| Создание события путем записи в коллекцию экземпляров.|
|[Получение события](../api/event-get.md) | [event](event.md) |Считывание свойств и отношений объекта event.|
|[Обновление](../api/event-update.md) | [event](event.md)   |Обновление объекта event. |
|[Удаление](../api/event-delete.md) | Нет |Удаление объекта event. |
|[cancel](../api/event-cancel.md) | Нет | Отправить сообщение об отмене из организатора для всех участников и Отмена указанного собрания. |
|[accept](../api/event-accept.md)|Нет|Примите события, указанного в календаре пользователя.|
|[tentativelyAccept](../api/event-tentativelyaccept.md)|Нет|Примите под вопросом события, указанного в календаре пользователя.|
|[decline](../api/event-decline.md)|Нет|Отклонить приглашение на события, указанного в календаре пользователя.|
|[forward](../api/event-forward.md)|Нет|Позволяет Организатор или участник собрания события пересылать запрос на собрание на нового получателя.|
|[delta](../api/event-delta.md)|Коллекция объектов [event](event.md)|Получение списка событий, которые были добавлены в **calendarView** (диапазон событий) основного календаря пользователя, обновлены в нем или удалены из него.|
|[dismissReminder](../api/event-dismissreminder.md)|Нет|Отклонение напоминание для указанного события в календаре пользователя.|
|[snoozeReminder](../api/event-snoozereminder.md)|Нет|Отложить напоминание для указанного события в календаре пользователя до нового времени.|
|[Список экземпляров](../api/event-list-instances.md) |Коллекция [Event](event.md)| Получение коллекции объектов Event.|
|**Вложения**| | |
|[Список вложений](../api/event-list-attachments.md) |Коллекция [Attachment](attachment.md)| Получение всех вложений, добавленных к данным о событии.|
|[Добавление вложения](../api/event-post-attachments.md) |[Attachment](attachment.md)| Добавление нового вложения к данным о событии путем публикации в коллекции вложений.|
|**Открытые расширения**| | |
|[Создание открытого расширения](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Создание открытого расширения и добавление настраиваемых свойств в новый или существующий ресурс.|
|[Получение открытого расширения](../api/opentypeextension-get.md) |Коллекция объектов [openTypeExtension](opentypeextension.md)| Получение открытого расширения, определяемого именем расширения.|
|**Расширения схемы**| | |
|[Добавление значений расширений для схемы](/graph/extensibility-schema-groups) || Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.|
|**Расширенные свойства**| | |
|[Создание расширенного свойства с одним значением](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[event](event.md)  |Создание одного или нескольких расширенных свойств с одним значением в новом или существующем событии.   |
|[Получение события с расширенным свойством с одним значением](../api/singlevaluelegacyextendedproperty-get.md)  | [event](event.md) | Получение событий, которые содержат расширенное свойство с одним значением, с помощью параметра `$expand` или `$filter`. |
|[Создание расширенного свойства с несколькими значениями](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [event](event.md) | Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем событии.  |
|[Получение события с расширенным свойством с несколькими значениями](../api/multivaluelegacyextendedproperty-get.md)  | [event](event.md) | Получение события, которое содержит расширенное свойство с несколькими значениями, с помощью параметра `$expand`. |

## <a name="see-also"></a>См. также

- [Отслеживание изменений данных Microsoft Graph с помощью запроса изменений](/graph/delta-query-overview)
- [Получение добавочных изменений для событий в папке](/graph/delta-query-events)
- [Добавление пользовательских данных в ресурсы с помощью расширений](/graph/extensibility-overview)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](/graph/extensibility-open-users)
- [Добавление пользовательских данных в группы с помощью расширений схемы](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
