---
title: Тип ресурса event
description: Событие в календаре.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 2604a56097635f8211824527dc031483d5c2e42a
ms.sourcegitcommit: 23aa2941cfb8bd744d8d59e8bba9d2c5f57f8e29
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/29/2019
ms.locfileid: "36667514"
---
# <a name="event-resource-type"></a>Тип ресурса event

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Событие в календаре ресурса [user](user.md) или стандартный календарь для ресурса [group](group.md), представляющего группу Office 365.

Максимальное количество участников в ресурсе **event** и максимальное количество получателей в ресурсе [eventMessage](eventmessage.md), отправленном из почтового ящика Exchange Online, составляют 500. Дополнительные сведения см. в разделе [Ограничения на отправку](https://docs.microsoft.com/ru-RU/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#sending-limits).

Этот ресурс поддерживает:

- добавление собственных данных к настраиваемым свойствам в виде [расширений](/graph/extensibility-overview);
- подписку на [уведомления об изменениях](/graph/webhooks);
- отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/event-delta.md)).

> **Примечание.** Существует несколько незначительных различий в способе взаимодействия с календарями пользователей, календарями групп и их событиями:

- В ресурсе [calendarGroup](calendargroup.md) можно упорядочить только календари пользователей.
- Outlook автоматически принимает все приглашения на собрания от имени группы. Приглашения на собрания можно [принять](../api/event-accept.md), [принять под вопросом](../api/event-tentativelyaccept.md) или [отклонить](../api/event-decline.md) только в календарях _пользователя_.
- Outlook не поддерживает напоминания о событиях группы. [Напоминание](reminder.md) можно [отложить](../api/event-snoozereminder.md) или [отключить](../api/event-dismissreminder.md) только для календарей _пользователя_.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
   "keyProperty": "id",
  "optionalProperties": [
    "attachments",
    "calendar",
    "extensions",
    "instances",
    "singleValueExtendedProperties",
    "multiValueExtendedProperties"
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
  "uid": "string",
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
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }]
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|attendees|Коллекция [Attendee](attendee.md)|Коллекция участников события.|
|body|[ItemBody](itembody.md)|Текст сообщения, связанного с событием. В формате HTML или текстовом формате.|
|bodyPreview|String|Предварительный просмотр сообщения, связанного с событием. В текстовом формате.|
|categories|Коллекция String|Категории, связанные с событием. Каждая категория соответствует свойству **displayName** объекта [outlookCategory](outlookcategory.md), определенного для пользователя.|
|changeKey|String|Указывает версию объекта события. При каждом изменении события также меняется значение ChangeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|end|[DateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс завершения события. По умолчанию время завершения указано в формате UTC.|
|hasAttachments|Boolean|Задайте значение true, если у события есть вложения.|
|id|String| Уникальный идентификатор события. [!INCLUDE [outlook-beta-id](../../includes/outlook-beta-id.md)] Только для чтения. |
|importance|String|Важность события. Возможные значения: `low`, `normal`, `high`.|
|isAllDay|Boolean|Задайте значение true, если событие длится весь день.|
|isCancelled|Boolean|Задайте значение true, если событие отменено.|
|isOrganizer|Boolean|Задайте значение true, если отправитель сообщения также является его организатором.|
|isReminderOn|Boolean|Задайте значение true, если установлено напоминание пользователю о событии.|
|lastModifiedDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|location|[Location](location.md)|Место проведения события.|
|locations|Коллекция [Location](location.md)|Места проведения события или участия в нем. Свойства **location** и **locations** всегда совпадают друг с другом. Если вы обновите свойство **location**, предыдущие места в коллекции **locations** будут удалены и заменены новым значением **location**. |
|onlineMeetingUrl|String|URL-адрес для собрания по сети. Свойство установлено только в том случае, если организатор определяет событие как собрание по сети, например в Skype. Только для чтения.|
|organizer|[Recipient](recipient.md)|Организатор события.|
|originalEndTimeZone|String|Часовой пояс завершения, указанный при создании события. Значение `tzone://Microsoft/Custom` указывает, что традиционный часовой пояс был задан в классическом приложении Outlook.|
|originalStart|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|originalStartTimeZone|String|Часовой пояс начала события, указанный при его создании. Значение `tzone://Microsoft/Custom` указывает, что в классическом приложении Outlook задан традиционный пользовательский часовой пояс.|
|recurrence|[PatternedRecurrence](patternedrecurrence.md)|Расписание повторения события.|
|reminderMinutesBeforeStart|Int32|Позволяет указать, за сколько минут до начала события появляется напоминание.|
|responseRequested|Boolean|Задайте значение true, если отправитель желает получить сообщение о согласии участвовать в событии или отклонении соответствующего приглашения.|
|responseStatus|[ResponseStatus](responsestatus.md)|Указывает тип отклика, отправленного в ответ на сообщение о событии.|
|sensitivity|String| Возможные значения: `normal`, `personal`, `private`, `confidential`.|
|seriesMasterId|String|Идентификатор для элемента образца повторяющегося ряда, если это событие входит в повторяющийся ряд.|
|showAs|String|Отображаемое состояние. Возможные значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.|
|start|[DateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс начала события. По умолчанию время начала указано в формате UTC.|
|subject|String|Текст в строке темы сообщения о событии.|
|type|String|Тип события. Возможные значения: `singleInstance`, `occurrence`, `exception`, `seriesMaster`. Только для чтения|
|uid|String|Уникальный идентификатор, совместно используемый всеми экземплярами события в разных календарях. **Примечание.** Предназначение этого свойства совпадает с предназначением свойства `iCalUid` для [ресурса события](/graph/api/resources/event?view=graph-rest-1.0) в конечной точке версии 1.0, но не гарантирует получение такого же значения.|
|webLink|String|URL-адрес для открытия события в Outlook в Интернете.<br/><br/>Outlook в Интернете открывает это событие в браузере, если выполнен вход в почтовый ящик. В противном случае Outlook в Интернете предлагает выполнить вход.<br/><br/>Доступ к этому URL-адресу можно получить из объекта iFrame.|

> [!NOTE]
> Свойство **webLink** указывает URL-адрес, по которому можно открыть событие только в более ранних версиях Outlook в Интернете. Ниже представлен формат URL-адреса, где _{event-id}_  — это зашифрованное в виде URL-адреса значение свойства **id**.
>
> `https://outlook.office365.com/owa/?itemid={event-id}&exvsurl=1&path=/calendar/item`
>
> Чтобы открыть URL-адрес в текущей версии Outlook в Интернете, преобразуйте его в следующий формат:
>
> `https://outlook.office365.com/calendar/item/{event-id}`


## <a name="relationships"></a>Отношения
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|attachments|Коллекция [Attachment](attachment.md)|Коллекция вложений [FileAttachment](fileattachment.md), [ItemAttachment](itemattachment.md) и [referenceAttachment](referenceattachment.md) для события. Свойство навигации. Только для чтения. Допускается значение null.|
|calendar|[Calendar](calendar.md)|Календарь, который содержит событие. Свойство навигации. Только для чтения.|
|extensions|Коллекция [extension](extension.md)|Коллекция открытых расширений, определенных для события. Допускается значение null.|
|instances|Коллекция [Event](event.md)|Экземпляры события. Свойство навигации. Только для чтения. Допускается значение null.|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Коллекция расширенных свойств с несколькими значениями, определенных для события. Только для чтения. Допускается значение null.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Коллекция расширенных свойств с одним значением, определенных для события. Только для чтения. Допускается значение null.|

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление событий](../api/user-list-events.md)|Коллекция [Event](event.md) |Получение списка объектов [event](../resources/event.md) в почтовом ящике пользователя. В этом списке указаны единичные собрания и главные собрания в соответствующих рядах.|
|[Создание события](../api/user-post-events.md) |[event](event.md)| Создание события путем записи в коллекцию экземпляров.|
|[Получение события](../api/event-get.md) | [event](event.md) |Считывание свойств и отношений объекта event.|
|[Обновление](../api/event-update.md) | [event](event.md)   |Обновление объекта event. |
|[Удаление](../api/event-delete.md) | Нет |Удаление объекта event. |
|[cancel](../api/event-cancel.md) | Нет | Отправка сообщения об отмене от организатора всем участникам и отмена указанного собрания. |
|[accept](../api/event-accept.md)|Нет|Принятие указанного события в календаре пользователя.|
|[tentativelyAccept](../api/event-tentativelyaccept.md)|Нет|Принятие под вопросом указанного события в календаре пользователя.|
|[decline](../api/event-decline.md)|Нет|Отклонение приглашения на указанное событие в календаре пользователя.|
|[forward](../api/event-forward.md)|Нет|Позволяет организатору или участнику собрания пересылать приглашение на собрание новому получателю.|
|[delta](../api/event-delta.md)|Коллекция объектов [event](event.md)|Получение списка событий, которые были добавлены в **calendarView** (диапазон событий) основного календаря пользователя, обновлены в нем или удалены из него.|
|[dismissReminder](../api/event-dismissreminder.md)|Нет|Отключение напоминания для указанного события в календаре пользователя.|
|[snoozeReminder](../api/event-snoozereminder.md)|Нет|Откладывание напоминания для указанного события в календаре пользователя на другое время.|
|[Перечисление экземпляров](../api/event-list-instances.md) |Коллекция [Event](event.md)| Получение коллекции объектов Event.|
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
<!--
{
  "type": "#page.annotation",
  "description": "event resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
