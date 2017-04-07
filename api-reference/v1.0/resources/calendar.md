# <a name="calendar-resource-type"></a>Тип ресурса calendar

Календарь, служащий контейнером для сведений о событиях.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список календарей](../api/user_list_calendars.md)|Коллекция [calendar](calendar.md)|Получение всех пользовательских календарей или календарей из стандартной либо другой указанной группы календарей.|
|[Создание календаря](../api/user_post_calendars.md) |[calendar](calendar.md)| Создание календаря в стандартной либо другой указанной группе календарей.|
|[Получение календаря](../api/calendar_get.md) | [calendar](calendar.md) |Считывание свойств и отношений объекта calendar.|
|[Обновление](../api/calendar_update.md) | [calendar](calendar.md)  |Обновление объекта calendar. |
|[Удаление](../api/calendar_delete.md) | Нет |Удаление объекта calendar. |
|[Список экземпляров calendarView](../api/calendar_list_calendarview.md) |Коллекция [Event](event.md)| Получение в представлении календаря повторений, исключений и отдельных экземпляров событий за определенный диапазон времени, указанных в основном календаре пользователя `(../me/calendarview)` или в другом заданном календаре.|
|[Список событий](../api/calendar_list_events.md) |Коллекция [Event](event.md)| Получение списка событий в календаре.  В этом списке указаны единичные собрания и главные собрания в соответствующих сериях.|
|[Создание события](../api/calendar_post_events.md) |[Event](event.md)| Создание события в стандартном или указанном календаре.|
|[Создание расширенного свойства с одним значением](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[calendar](calendar.md)  |Создание одного или нескольких расширенных свойств с одним значением в новом или существующем календаре.   |
|[Получение календаря с расширенным свойством с одним значением](../api/singlevaluelegacyextendedproperty_get.md)  | [calendar](calendar.md) | Получение календарей, которые содержат расширенное свойство с одним значением, при помощи `$expand` или `$filter`. |
|[Создание расширенного свойства с несколькими значениями](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [calendar](calendar.md) | Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем календаре.  |
|[Получение календаря с расширенным свойством с несколькими значениями](../api/multivaluelegacyextendedproperty_get.md)  | [calendar](calendar.md) | Получение календаря, который содержит расширенное свойство с несколькими значениями, при помощи `$expand`. |


## <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
|name|String|Имя календаря.|
|changeKey|String|Указывает версию объекта calendar. При каждом изменении календаря также меняется значение ChangeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта. Только для чтения.|
|color|String|Задает цветовую тему, отличающую этот календарь от других календарей в пользовательском интерфейсе. Значения свойств: LightBlue = 0, LightGreen = 1, LightOrange = 2, LightGray = 3, LightYellow = 4, LightTeal = 5, LightPink = 6, LightBrown = 7, LightRed = 8, MaxColor = 9, Auto = -1.|
|id|Строка|Уникальный идентификатор группы. Только для чтения.|

## <a name="relationships"></a>Связи
| Связь | Тип    |Описание|
|:---------------|:--------|:----------|
|calendarView|Коллекция [Event](event.md)|Представление календаря для календаря. Свойство навигации. Только для чтения.|
|события|Коллекция [Event](event.md)|События в календаре. Свойство навигации. Только для чтения.|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Коллекция расширенных свойств с несколькими значениями, определенных для календаря. Только для чтения. Допускается значение null.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Коллекция расширенных свойств с одним значением, определенных для календаря. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "calendarView",
    "events",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.calendar"
}-->

```json
{
  "changeKey": "string",
  "color": "String",
  "id": "string (identifier)",
  "name": "string"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "calendar resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
