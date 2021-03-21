---
title: Тип ресурса calendar
description: Календарь, служащий контейнером для сведений о событиях. Это может быть календарь для пользователя или стандартный календарь для группы Microsoft 365.
localization_priority: Priority
author: harini84
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d6d549435cd9350f9baf1136fd10f174eb1d0938
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952552"
---
# <a name="calendar-resource-type"></a>Тип ресурса calendar

Пространство имен: microsoft.graph

Календарь, служащий контейнером для сведений о событиях. Это может быть календарь для [пользователя](user.md) или стандартный календарь для [группы](group.md) Microsoft 365.

> **Примечание.** Существует несколько незначительных различий в способе взаимодействия с календарями пользователей и календарями групп:

- В ресурсе [calendarGroup](calendargroup.md) можно упорядочить только календари пользователей.
- Outlook автоматически принимает все приглашения на собрания от имени группы. Приглашения на собрания можно [принять](../api/event-accept.md), [принять под вопросом](../api/event-tentativelyaccept.md) или [отклонить](../api/event-decline.md) только в календарях пользователя.
- Outlook не поддерживает напоминания о событиях группы. [Напоминание](reminder.md) можно [отложить](../api/event-snoozereminder.md) или [отключить](../api/event-dismissreminder.md) только для календарей пользователя.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список календарей](../api/user-list-calendars.md)|Коллекция [calendar](calendar.md)|Получение всех пользовательских календарей или календарей из стандартной либо другой указанной группы календарей.|
|[Создание календаря](../api/user-post-calendars.md) |[calendar](calendar.md)| Создание календаря для пользователя в стандартной либо другой указанной группе календарей.|
|[Получение календаря](../api/calendar-get.md) | [calendar](calendar.md) |Получение свойств и связей объекта **calendar**. Это может быть календарь для пользователя или стандартный календарь для группы Microsoft 365. |
|[Обновление](../api/calendar-update.md) | [calendar](calendar.md)  |Обновление свойств объекта **calendar**. Это может быть календарь для пользователя или стандартный календарь для группы Microsoft 365. |
|[удаление](../api/calendar-delete.md); | Нет |Удаление объекта calendar. |
|[Список экземпляров calendarView](../api/calendar-list-calendarview.md) |Коллекция [event](event.md)| Получение в представлении календаря повторений, исключений и отдельных экземпляров событий за определенный диапазон времени, указанных в основном календаре пользователя `(../me/calendarview)` или в другом заданном календаре.|
|[Список событий](../api/calendar-list-events.md) |Коллекция [event](event.md)| Получение списка событий в календаре. Этот список содержит собрания с одним экземпляром и образцы рядов.|
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
|allowedOnlineMeetingProviders|Коллекция onlineMeetingProviderType| Представляет поставщиков служб собраний по сети, которых можно использовать для создания собраний в этом календаре. Возможные значения: `unknown`, `skypeForBusiness`, `skypeForConsumer`, `teamsForBusiness`.|
|canEdit |Boolean |Значение `true`, если пользователь может вносить изменения в календарь, в противном случае — значение `false`. Это свойство имеет значение `true` для пользователя, создавшего календарь. Это свойство также имеет значение `true` для пользователей, которые совместно используют календарь и имеют доступ на запись. |
|canShare |Boolean |Значение `true`, если у пользователя есть разрешение на совместное использование календаря, в противном случае — значение `false`. Только пользователь, создавший календарь, может предоставлять общий доступ к нему. |
|canViewPrivateItems |Boolean |Значение `true`, если пользователь может читать элементы календаря, которые были помечены как частные, в противном случае — значение `false`. |
|changeKey|String|Указывает версию объекта calendar. При каждом изменении календаря также меняется значение changeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта. Только для чтения.|
|color|calendarColor|Задает цветовую тему, отличающую этот календарь от других календарей в пользовательском интерфейсе. Возможные значения: `auto`, `lightBlue`, `lightGreen`, `lightOrange`, `lightGray`, `lightYellow`, `lightTeal`, `lightPink`, `lightBrown`, `lightRed`, `maxColor`.|
|defaultOnlineMeetingProvider|onlineMeetingProviderType|Стандартный поставщик для собраний по сети, отправленных из этого календаря. Возможные значения: `unknown`, `skypeForBusiness`, `skypeForConsumer`, `teamsForBusiness`.|
|hexColor |String |Цвет календаря, представленный кодом из трех шестнадцатеричных значений в диапазоне от 00 до FF, которые обозначают красный, зеленый и синий компоненты цвета в цветовом пространстве RGB. Если пользователь не задал цвет календаря явным образом, это свойство будет пустым. Только для чтения.|
|id|String|Уникальный идентификатор календаря. Только для чтения.|
|isDefaultCalendar|Boolean|Значение `true`, если это стандартный календарь, где новые события создаются по умолчанию. В противном случае — значение `false`.|
|isRemovable|Логический| Указывает, можно ли удалить этот календарь из почтового ящика пользователя.|
|isTallyingResponses|Логический|Указывает, поддерживает ли этот пользовательский календарь отслеживание ответов на приглашения на собрания. Только приглашения на собрания, отправленные из основных календарей пользователей, поддерживают отслеживание ответов на приглашения на собрания.|
|name|String|Имя календаря.|
|owner |[emailAddress](emailaddress.md) | Если это свойство задано, оно указывает на пользователя, создавшего или добавившего календарь. В календаре, созданном или добавленном пользователем, свойство **owner** установлено для этого пользователя. В календаре, который используется совместно с пользователем, свойство **owner** установлено для лица, предоставившего пользователю общий доступ к этому календарю. |

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|calendarPermissions|Коллекция [calendarPermission](calendarpermission.md)| Разрешения пользователей, которым предоставлен доступ к календарю.|
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
  "allowedOnlineMeetingProviders": ["string"],
  "canEdit": "boolean",
  "canShare": "boolean",
  "canViewPrivateItems": "boolean",
  "changeKey": "string",
  "color": "String",
  "defaultOnlineMeetingProvider": "string",
  "hexColor": "String",
  "id": "string (identifier)",
  "isDefaultCalendar": "boolean",
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

