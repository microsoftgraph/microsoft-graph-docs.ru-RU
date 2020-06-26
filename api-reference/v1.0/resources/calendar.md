---
title: Тип ресурса calendar
description: Календарь, служащий контейнером для сведений о событиях. Это может быть календарь пользователя или календарь по умолчанию для группы Microsoft 365.
localization_priority: Priority
author: harini84
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 47a63319efea2bdcdf11728bbac7d17903c6590a
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895708"
---
# <a name="calendar-resource-type"></a>Тип ресурса calendar

Пространство имен: microsoft.graph

Календарь, служащий контейнером для сведений о событиях. Это может быть календарь [пользователя](user.md)или календарь по умолчанию для [группы](group.md)Microsoft 365.

> **Примечание.** Существует несколько незначительных различий в способе взаимодействия с календарями пользователей и календарями групп:

- В ресурсе [calendarGroup](calendargroup.md) можно упорядочить только календари пользователей.
- Outlook автоматически принимает все приглашения на собрания от имени группы. Приглашения на собрания можно [принять](../api/event-accept.md), [принять под вопросом](../api/event-tentativelyaccept.md) или [отклонить](../api/event-decline.md) только в календарях пользователя.
- Outlook не поддерживает напоминания о событиях группы. [Напоминание](reminder.md) можно [отложить](../api/event-snoozereminder.md) или [отключить](../api/event-dismissreminder.md) только для календарей пользователя.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список календарей](../api/user-list-calendars.md)|Коллекция [calendar](calendar.md)|Получение всех пользовательских календарей или календарей из стандартной либо другой указанной группы календарей.|
|[Создание календаря](../api/user-post-calendars.md) |[calendar](calendar.md)| Создание календаря для пользователя в стандартной либо другой указанной группе календарей.|
|[Получение календаря](../api/calendar-get.md) | [calendar](calendar.md) |Получение свойств и связей объекта **calendar**. В качестве календаря может использоваться календарь пользователя или стандартный календарь группы Microsoft 365. |
|[Обновление](../api/calendar-update.md) | [calendar](calendar.md)  |Обновление свойств объекта **calendar**. В качестве календаря может использоваться календарь пользователя или стандартный календарь группы Microsoft 365. |
|[Удаление](../api/calendar-delete.md) | Нет |Удаление объекта calendar. |
|[Список экземпляров calendarView](../api/calendar-list-calendarview.md) |Коллекция [event](event.md)| Получение в представлении календаря повторений, исключений и отдельных экземпляров событий за определенный диапазон времени, указанных в основном календаре пользователя `(../me/calendarview)` или в другом заданном календаре.|
|[Список событий](../api/calendar-list-events.md) |Коллекция [event](event.md)| Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.|
|[Создание события](../api/calendar-post-events.md) |[event](event.md)| Создание события в стандартном или указанном календаре.|
|[getSchedule](../api/calendar-getschedule.md) |Коллекция [scheduleInformation](scheduleinformation.md)|Получение сведений о доступности коллекции пользователей, списков рассылки или ресурсов для определенного периода времени. |
|[findMeetingTimes](../api/user-findmeetingtimes.md) |[meetingTimeSuggestionsResult](meetingtimesuggestionsresult.md) |Предложение времени проведения собрания и местоположения с учетом доступности организатора и участников, а также ограничений по местоположению или времени. |
|[Создание однозначного расширенного свойства](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[calendar](calendar.md)  |Создание одного или нескольких расширенных свойств с одним значением в новом или существующем календаре.   |
|[Получение календаря с расширенным свойством с одним значением](../api/singlevaluelegacyextendedproperty-get.md)  | [calendar](calendar.md) | Получение календарей, которые содержат расширенное свойство с одним значением, при помощи `$expand` или `$filter`. |
|[Создание расширенного свойства с несколькими значениями](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [calendar](calendar.md) | Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем календаре.  |
|[Получение календаря с расширенным свойством с несколькими значениями](../api/multivaluelegacyextendedproperty-get.md)  | [calendar](calendar.md) | Получение календаря, который содержит расширенное свойство с несколькими значениями, при помощи `$expand`. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|allowedOnlineMeetingProviders|Коллекция строк| Представляет поставщиков служб собраний по сети, которых можно использовать для создания собраний в этом календаре. Возможные значения: `unknown`, `skypeForBusiness`, `skypeForConsumer`, `teamsForBusiness`.|
|canEdit |Boolean |True if the user can write to the calendar, false otherwise. This property is true for the user who created the calendar. This property is also true for a user who has been shared a calendar and granted write access. |
|canShare |Boolean |True if the user has the permission to share the calendar, false otherwise. Only the user who created the calendar can share it. |
|canViewPrivateItems |Boolean |Значение true, если пользователь может читать элементы календаря, которые были помечены как частные, в противном случае — значение false. |
|changeKey|String|Identifies the version of the calendar object. Every time the calendar is changed, changeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.|
|color|calendarColor|Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1|
|defaultOnlineMeetingProvider|onlineMeetingProviderType|Стандартный поставщик для собраний по сети, отправленных из этого календаря. Возможные значения: `unknown`, `skypeForBusiness`, `skypeForConsumer`, `teamsForBusiness`.|
|id|String|The calendar's unique identifier. Read-only.|
|isRemovable|Логический| Указывает, можно ли удалить этот календарь из почтового ящика пользователя.|
|isTallyingResponses|Логический|Указывает, поддерживает ли этот пользовательский календарь отслеживание ответов на приглашения на собрания. Только приглашения на собрания, отправленные из основных календарей пользователей, поддерживают отслеживание ответов на приглашения на собрания.|
|name|String|Имя календаря.|
|owner |[emailAddress](emailaddress.md) | If set, this represents the user who created or added the calendar. For a calendar that the user created or added, the **owner** property is set to the user. For a calendar shared with the user, the **owner** property is set to the person who shared that calendar with the user. |

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|calendarPermissions|Коллекция [calendarPermission](calendarpermission.md)| Разрешения пользователей, которым предоставлен доступ к календарю.|
|calendarView|Коллекция [Event](event.md)|The calendar view for the calendar. Navigation property. Read-only.|
|events|Коллекция [Event](event.md)|The events in the calendar. Navigation property. Read-only.|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| The collection of multi-value extended properties defined for the calendar. Read-only. Nullable.|
|singleValueExtendedProperties|Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| The collection of single-value extended properties defined for the calendar. Read-only. Nullable.|

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
  "allowedOnlineMeetingProviders": ["string"],
  "canEdit": "boolean",
  "canShare": "boolean",
  "canViewPrivateItems": "boolean",
  "changeKey": "string",
  "color": "String",
  "defaultOnlineMeetingProvider": "string",
  "id": "string (identifier)",
  "isRemovable": "boolean",
  "isTallyingResponses": "boolean",
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
