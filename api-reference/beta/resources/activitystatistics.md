---
title: Тип ресурса Активитистатистикс
description: Представляет время, затраченное на рабочие действия, включая электронную почту, собрания, фокусы, разговоры и звонки.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 3d2e626535d579b77c27125500d7247401f26915
ms.sourcegitcommit: d419565add1f731be50c9b5911eb1310fa007097
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2020
ms.locfileid: "42280619"
---
# <a name="activitystatistics-resource-type"></a>Тип ресурса Активитистатистикс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет время, затраченное пользователем на выполнение различных действий в течение и за пределами рабочего времени, для указанного диапазона времени в запросе, в котором используется период агрегирования за один день.

Следующие типы статистики являются производными от **активитистатистикс**:

* [Call](callactivitystatistics.md)
* [Отображаются](chatactivitystatistics.md)
* [Электронная почта](emailactivitystatistics.md)
* [Фокус](focusactivitystatistics.md)
* [Назначить](meetingactivitystatistics.md)

<!--  removing per Mathew 2/6/2020   ### Activity id property

In an HTTP request, to get a specific type of activity statistics within a date range, you can express this information as an ID to the user's collection of activityStatistics in the following format, where `{startdate}` and `{enddate}` are expressed in ISO 8601 calendar date format and `{activity}` can be "call", "chat", "email", "focus", or "meeting":

```
{activity}_{startdate}_{enddate}
```

For example, the ID "email_2019-08-10_2019-08-12" represents the emailActivityStatistics for the specified user between August 10, 2019 and August 12, 2019.
-->
## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список Активитистатистикс](../api/activitystatistics-list.md) | [активитистатистикс](activitystatistics.md) | Получение свойств для коллекции статистики действий пользователя за последнюю полную неделю. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|activity |аналитиксактивититипе |Тип действия, для которого возвращается статистика. Возможные значения: `call`, `chat`, `email`, `focus`и. `meeting` |
|duration |Длительность |Общее количество часов, потраченных на действие. Значение представляется в формате ISO 8601 для длительности. |
|endDate |Date |Дата завершения действия, выраженная в формате ISO 8601 для календарных дат. Например, значение свойства может иметь значение "2019-07-03", которое соответствует формату ГГГГ – MM – DD. |
|id |String |Идентификатор действия, предназначенный только для чтения. Не проанализируйте и не настраивайте значение для своих сценариев. |
|startDate |Дата |Дата начала действия, выраженная в формате ISO 8601 для календарных дат. Например, значение свойства может иметь значение "2019-07-04", которое соответствует формату ГГГГ – MM – DD. |
|тимезонеусед |String |Часовой пояс, который пользователь задает в Microsoft Outlook для вычисления. Например, значение свойства может быть "тихоокеанское стандартное время". |

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- { 
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.activityStatistics",
  "keyProperty": "id"
}-->

```json
{
  "activity": "String",
  "duration": "String (ISO 8601 duration)",
  "endDate": "String (ISO 8601 format)",
  "id": "String (identifier)",
  "startDate": "String (ISO 8601 format)",
  "timeZoneUsed": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "activityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}--> 