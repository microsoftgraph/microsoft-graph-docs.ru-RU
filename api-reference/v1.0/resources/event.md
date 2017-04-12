# <a name="event-resource-type"></a>Тип ресурса event

Событие в календаре.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список событий](../api/user_list_events.md)|Коллекция [event](event.md) |Получение списка объектов [event](../resources/event.md) в почтовом ящике пользователя. В этом списке указаны единичные собрания и главные собрания в соответствующих сериях.|
|[Создание события](../api/user_post_events.md) |[event](event.md)| Создание события путем записи в коллекцию экземпляров.|
|[Получение события](../api/event_get.md) | [event](event.md) |Считывание свойств и отношений объекта event.|
|[Обновление](../api/event_update.md) | [event](event.md) |Обновление объекта event. |
|[Удаление](../api/event_delete.md) | Нет |Удаление объекта event. |
|[accept](../api/event_accept.md)|Нет|Принятие указанного события.|
|[tentativelyAccept](../api/event_tentativelyaccept.md)|Нет|Предварительное принятие указанного события.|
|[decline](../api/event_decline.md)|Нет|Отклонение приглашения на указанное событие.|
|[dismissReminder](../api/event_dismissreminder.md)|Нет|Отключение напоминания для указанного события.|
|[snoozeReminder](../api/event_snoozereminder.md)|Нет|Отложить напоминание для указанного события.|
|[Список экземпляров](../api/event_list_instances.md) |Коллекция [event](event.md)| Получение экземпляров (повторов) события для заданного диапазона времени. Если событие относится к типу `SeriesMaster`, возвращаются экземпляры и исключения события для указанного диапазона времени.|
|**Вложения**| | |
|[Список вложений](../api/event_list_attachments.md) |Коллекция [attachment](attachment.md) | Получение всех вложений, добавленных к данным о событии.|
|[Добавление вложения](../api/event_post_attachments.md) |[attachment](attachment.md)| Добавление нового вложения к данным о событии путем публикации в коллекции вложений.|
|**Открытые расширения**| | |
|[Создание открытого расширения](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Создание открытого расширения и добавление настраиваемых свойств в новый или существующий экземпляр ресурса.|
|[Получение открытого расширения](../api/opentypeextension_get.md) |Коллекция [openTypeExtension](opentypeextension.md)| Получение объекта или объектов открытого расширения, которые определяются по имени или полному имени.|
|**Расширенные свойства**| | |
|[Создание расширенного свойства с одним значением](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[event](event.md)  |Создание одного или нескольких расширенных свойств с одним значением в новом или существующем событии.   |
|[Получение события с расширенным свойством с одним значением](../api/singlevaluelegacyextendedproperty_get.md)  | [event](event.md) | Получение событий, которые содержат расширенное свойство с одним значением, с помощью параметра `$expand` или `$filter`. |
|[Создание расширенного свойства с несколькими значениями](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [event](event.md) | Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем событии.  |
|[Получение события с расширенным свойством с несколькими значениями](../api/multivaluelegacyextendedproperty_get.md)  | [event](event.md) | Получение события, которое содержит расширенное свойство с несколькими значениями, с помощью параметра `$expand`. |



## <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
|attendees|Коллекция объектов [attendee](attendee.md)|Коллекция участников события.|
|body|[itemBody](itembody.md)|Текст сообщения, связанного с событием. В формате HTML или текстовом формате.|
|bodyPreview|String|Предварительный просмотр сообщения, связанного с событием. В текстовом формате.|
|categories|Коллекция String|Категории, связанные с событием.|
|changeKey|String|Указывает версию объекта события. При каждом изменении события также меняется значение ChangeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта.|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|end|[dateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс завершения события.|
|hasAttachments|Boolean|Задайте значение true, если у события есть вложения.|
|iCalUId|String|Уникальный идентификатор, совместно используемый всеми экземплярами события в разных календарях.|
|id|String| Только для чтения.|
|importance|String|Важность события. Low = 0, Normal = 1, High = 2. Возможные значения: `Low`, `Normal`, `High`.|
|isAllDay|Boolean|Задайте значение true, если событие длится весь день.|
|isCancelled|Boolean|Задайте значение true, если событие отменено.|
|isOrganizer|Boolean|Задайте значение true, если отправитель сообщения также является его организатором.|
|isReminderOn|Boolean|Задайте значение true, если установлено напоминание пользователю о событии.|
|lastModifiedDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|location|[location](location.md)|Место проведения события.|
|onlineMeetingUrl|String|URL-адрес для собрания по сети.|
|organizer|[recipient](recipient.md)|Организатор события.|
|originalEndTimeZone|String|Часовой пояс завершения события, указанный при его создании. Значение `tzone://Microsoft/Custom` указывает, что в классическом приложении Outlook задан традиционный пользовательский часовой пояс.|
|originalStart|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|originalStartTimeZone|Строка|Часовой пояс начала события, указанный при его создании. Значение `tzone://Microsoft/Custom` указывает, что в классическом приложении Outlook задан традиционный пользовательский часовой пояс. |
|recurrence|[patternedRecurrence](patternedrecurrence.md)|Расписание повторения события.|
|reminderMinutesBeforeStart|Int32|Позволяет указать, за сколько минут до начала события появляется напоминание.|
|responseRequested|Boolean|Задайте значение true, если отправитель желает получить сообщение о согласии участвовать в событии или отклонении соответствующего приглашения.|
|responseStatus|[responseStatus](responsestatus.md)|Указывает тип отклика, отправленного в ответ на сообщение о событии.|
|sensitivity|String| Возможные значения: `Normal`, `Personal`, `Private`, `Confidential`.|
|seriesMasterId|String|Категории, назначенные элементу.|
|showAs|String|Отображаемое состояние. Free = 0, Tentative = 1, Busy = 2, Oof = 3, WorkingElsewhere = 4, Unknown = -1. Возможные значения: `Free`, `Tentative`, `Busy`, `Oof`, `WorkingElsewhere`, `Unknown`.|
|start|[dateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс начала события.|
|subject|String|Текст в строке темы сообщения о событии.|
|type|String|Тип события: SingleInstance = 0, Occurrence = 1, Exception = 2, SeriesMaster = 3. Возможные значения: `SingleInstance`, `Occurrence`, `Exception`, `SeriesMaster`.|
|webLink|String|URL-адрес для открытия события в Outlook Web App.<br/><br/>Событие откроется в браузере, если вы вошли в свой почтовый ящик с помощью Outlook Web App. Если вход с помощью браузера еще не выполнен, вам будет предложено войти.<br/><br/>Доступ к этому URL-адресу можно получить из объекта iFrame.|

## <a name="relationships"></a>Отношения
| Связь | Тип    |Описание|
|:---------------|:--------|:----------|
|attachments|Коллекция [attachment](attachment.md) |Коллекция вложений [fileAttachment](fileAttachment.md) и [itemAttachment](itemAttachment.md) для события. Свойство навигации. Только для чтения. Допускается значение null.|
|календарь|[calendar](calendar.md)|Календарь, который содержит событие. Свойство навигации. Только для чтения.|
|extensions|Коллекция [extension](extension.md)|Коллекция открытых расширений, определенных для события. Только для чтения. Допускается значение null.|
|instances|Коллекция [event](event.md)|Экземпляры события. Свойство навигации. Только для чтения. Допускается значение null.|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Коллекция расширенных свойств с несколькими значениями, определенных для события. Только для чтения. Допускается значение null.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Коллекция расширенных свойств с одним значением, определенных для события. Только для чтения. Допускается значение null.|


## <a name="json-representation"></a>Представление JSON

Ниже этот ресурс представлен в формате JSON.

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
  "keyProperty": "id",
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
  "iCalUId": "string",
  "id": "string (identifier)",
  "importance": "String",
  "isAllDay": true,
  "isCancelled": true,
  "isOrganizer": true,
  "isReminderOn": true,
  "lastModifiedDateTime": "String (timestamp)",
  "location": {"@odata.type": "microsoft.graph.location"},
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
  "instances": [ { "@odata.type": "microsoft.graph.event" }]

}

```


## <a name="see-also"></a>См. также

- [Добавление пользовательских данных в ресурсы с помощью расширений](../../../concepts/extensibility_overview.md)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)](../../../concepts/extensibility_open_users.md)
- [Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
