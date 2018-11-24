# <a name="calendar-resource-type"></a>Тип ресурса calendar

Календарь, служащий контейнером для сведений о событиях. Это может быть календарь для ресурса [user](user.md) или стандартный календарь для ресурса [group](group.md), представляющего группу Office 365.

> **Примечание:** Существуют небольшие отличия таким способом, который может взаимодействовать с календарей пользователей и группы календаря:

 - Их можно организовать только календарей пользователей в [calendarGroup](calendargroup.md).
 - Outlook автоматически принимает все приглашения на собрания от имени группы. Для календарей пользователей только можно [принять](../api/event_accept.md), [под вопросом принятие](../api/event_tentativelyaccept.md)или [отклонение](../api/event_decline.md) приглашения на собрания.
  - Outlook не поддерживает напоминания о событиях группы. Можно [отложить](../api/event_snoozereminder.md) или [отклонение](../api/event_dismissreminder.md) [напоминание](reminder.md) для только календарей пользователей.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список календарей](../api/user_list_calendars.md)|Коллекция [calendar](calendar.md)|Получение всех пользовательских календарей или календарей из стандартной либо другой указанной группы календарей.|
|[Создание календаря](../api/user_post_calendars.md) |[calendar](calendar.md)| Создание календаря для пользователя в стандартной либо другой указанной группе календарей.|
|[Получение календаря](../api/calendar_get.md) | [calendar](calendar.md) |Получение свойств и связей объекта **calendar**. Это может быть календарь для пользователя или стандартный календарь для группы Office 365. |
|[Обновление](../api/calendar_update.md) | [calendar](calendar.md)  |Обновление свойств объекта **calendar**. Это может быть календарь для пользователя или стандартный календарь для группы Office 365. |
|[Удаление](../api/calendar_delete.md) | Нет |Удаление объекта calendar. |
|[Список экземпляров calendarView](../api/calendar_list_calendarview.md) |Коллекция [event](event.md)| Получение в представлении календаря повторений, исключений и отдельных экземпляров событий за определенный диапазон времени, указанных в основном календаре пользователя `(../me/calendarview)` или в другом заданном календаре.|
|[Список событий](../api/calendar_list_events.md) |Коллекция [event](event.md)| Получение списка событий в календаре.  Этот список содержит собрания с одним экземпляром и образцы рядов.|
|[Создание события](../api/calendar_post_events.md) |[event](event.md)| Создайте новое событие в по умолчанию или указанного календаря.|
|[findMeetingTimes](../api/user_findmeetingtimes.md) |[meetingTimeSuggestionsResult](meetingtimesuggestionsresult.md) |Предложите совещаний и расположений на основе доступности организатора и участников и ограничения времени или расположение. |
|[Создание расширенного свойства с одним значением](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[calendar](calendar.md)  |Создание одного или нескольких расширенных свойств с одним значением в новом или существующем календаре.   |
|[Получение календаря с расширенным свойством с одним значением](../api/singlevaluelegacyextendedproperty_get.md)  | [calendar](calendar.md) | Получение календарей, которые содержат расширенное свойство с одним значением, при помощи `$expand` или `$filter`. |
|[Создание расширенного свойства с несколькими значениями](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [calendar](calendar.md) | Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем календаре.  |
|[Получение календаря с расширенным свойством с несколькими значениями](../api/multivaluelegacyextendedproperty_get.md)  | [calendar](calendar.md) | Получение календаря, который содержит расширенное свойство с несколькими значениями, при помощи `$expand`. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|canEdit |Boolean |Значение true, если пользователь может вносить изменения в календарь, в противном случае — значение false. Это свойство имеет значение true для пользователя, создавшего календарь. Это свойство также имеет значение true для пользователей, которые совместно используют календарь и имеют доступ на запись. |
|canShare |Boolean |Значение true, если у пользователя есть разрешение на совместное использование календаря, в противном случае — значение false. Только пользователь, создавший календарь, может предоставлять общий доступ к нему. |
|canViewPrivateItems |Boolean |Значение true, если пользователь может читать элементы календаря, которые были помечены как частные, в противном случае — значение false. |
|changeKey|String|Указывает версию объекта calendar. При каждом изменении календаря также меняется значение changeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта. Только для чтения.|
|color|calendarColor|Задает цветовую тему, отличающую этот календарь от других календарей в пользовательском интерфейсе. Значения свойств: LightBlue = 0, LightGreen = 1, LightOrange = 2, LightGray = 3, LightYellow = 4, LightTeal = 5, LightPink = 6, LightBrown = 7, LightRed = 8, MaxColor = 9, Auto = -1.|
|id|String|Уникальный идентификатор группы. Только для чтения.|
|name|String|Имя календаря.|
|owner |[emailAddress](emailaddress.md) | Если это свойство задано, оно указывает на пользователя, создавшего или добавившего календарь. В календаре, созданном или добавленном пользователем, свойство **owner** установлено для этого пользователя. В календаре, который используется совместно с пользователем, свойство **owner** установлено для лица, предоставившего пользователю общий доступ к этому календарю. |

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|calendarView|Коллекция [Event](event.md)|Представление календаря для календаря. Свойство навигации. Только для чтения.|
|events|Коллекция [Event](event.md)|События в календаре. Свойство навигации. Только для чтения.|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| Коллекция расширенных свойств с несколькими значениями, определенных для календаря. Только для чтения. Допускается значение null.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| Коллекция расширенных свойств с одним значением, определенных для календаря. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "calendarView",
    "events",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.calendar",
  "@odata.annotations": [
    {
      "property": "calendarView",
      "capabilities": {
        "changeTracking": true,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "events",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "navigability": "single",
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "canEdit": "boolean",
  "canShare": "boolean",
  "canViewPrivateItems": "boolean",
  "changeKey": "string",
  "color": "String",
  "id": "string (identifier)",
  "name": "string",
  "owner": {"@odata.type": "microsoft.graph.emailAddress"}
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
