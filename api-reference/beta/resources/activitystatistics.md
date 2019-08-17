---
title: Тип ресурса Активитистатистикс
description: Представляет время, затраченное на рабочие действия, включая электронную почту, собрания, фокусы, разговоры и звонки.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 5cee94c1ff36bf30d977b7eb97d77f11d4d2ff5e
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450809"
---
# <a name="activitystatistics-resource-type"></a>Тип ресурса Активитистатистикс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет время, затраченное пользователем на выполнение различных действий в течение и за пределами рабочего времени, для указанного диапазона времени в запросе, в котором используется период агрегирования за один день.

Следующие типы статистики являются производными от **активитистатистикс**:

* [Call](callactivitystatistics.md)
* [Чат](chatactivitystatistics.md)
* [Email](emailactivitystatistics.md)
* [Фокус](focusactivitystatistics.md)
* [Назначить](meetingactivitystatistics.md)

### <a name="activity-id-property"></a>Свойство идентификатора действия

В HTTP-запросе для получения определенного типа статистики действий в диапазоне дат можно выразить эту информацию как идентификатор коллекции пользователей Активитистатистикс в следующем формате, где `{startdate}` и `{enddate}` в календаре ISO 8601. формат даты и `{activity}` может иметь следующий вид: "Call", "Chat", "Email", "Focus" или "Meeting".

```
{activity}_{startdate}_{enddate}
```

Например, идентификатор "email_2019 – 08 -10 _2019 – 08 – 12" представляет Емаилактивитистатистикс для указанного пользователя между 10 августа 2019 и 12 августа 2019.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение Активитистатистикс](../api/activitystatistics-get.md) | [активитистатистикс](activitystatistics.md) | Получение свойств для статистики указанного действия пользователя за указанный диапазон времени. |
| [Список Активитистатистикс](../api/activitystatistics-list.md) | [активитистатистикс](activitystatistics.md) | Получение свойств для коллекции статистики действий пользователя за последнюю полную неделю.|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|activity|аналитиксактивититипе| Тип действия, для которого возвращается статистика. Возможные значения: `call`, `chat`, `email`, `focus`и. `meeting`|
|duration|Duration (Длительность)|Общее количество часов, потраченных на действие. Значение представляется в формате ISO 8601 для длительности.|
|endDate|Date|Дата завершения действия, выраженная в формате ISO 8601 для календарных дат. Например, значение свойства может иметь значение "2019-07-03", которое соответствует формату ГГГГ – MM – DD.|
|id|String| Идентификатор для операции, который представляется `{activity}_{startdate}_{enddate}`только для чтения.|
|startDate|Дата|Дата начала действия, выраженная в формате ISO 8601 для календарных дат. Например, значение свойства может иметь значение "2019-07-04", которое соответствует формату ГГГГ – MM – DD.|
|тимезонеусед|String|Часовой пояс, который пользователь задает в Microsoft Outlook для вычисления. Например, значение свойства может быть "тихоокеанское стандартное время".|

## <a name="relationships"></a>Отношения

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