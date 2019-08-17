---
title: Тип ресурса Митингактивитистатистикс
description: Представляет сведения о действиях с собраниями для пользователей.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: aa0e4b12ed260c0f6660544e7f48cfe1ca9cd3dc
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450811"
---
# <a name="meetingactivitystatistics-resource-type"></a>Тип ресурса Митингактивитистатистикс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет данные о времени пользователя, затраченного на собрания в Microsoft Outlook, Microsoft Teams или Skype для бизнеса. Это основано на [активитистатистикс](../resources/activitystatistics.md).
<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get meetingActivityStatistics](../api/meetingactivitystatistics-get.md) | [meetingActivityStatistics](meetingactivitystatistics.md) | Read properties and relationships of meetingActivityStatistics object; name of the activity for which statistics are returned as “meeting.” |
-->
## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|activity|аналитиксактивититипе| Действия собраний, для которых возвращается статистика.|
|duration|Duration (Длительность)|Общее количество часов, потраченных на собрания. Значение представляется в формате ISO 8601 для длительности.|
|endDate|Date|Дата завершения действия собрания. Значение представлено в формате ISO 8601 для календарных дат. Например, значение свойства может иметь значение "2019-07-04", которое соответствует формату ГГГГ – MM – DD.|
|id|String| Идентификатор, предназначенный только для чтения, для действия собрания.|
|startDate|Дата|Дата начала действия собрания. Значение представлено в формате ISO 8601 для календарных дат. Например, значение свойства может иметь значение "2019-07-03", которое соответствует формату ГГГГ – MM – DD.|
|тимезонеусед|String|Для вычисления используется часовой пояс Outlook, который пользователь задает в календаре Outlook. Например, значение свойства может быть "тихоокеанское стандартное время".|
|афтерхаурс|Duration (Длительность)|Время, затраченное на собрания в нерабочее время, которое основано на параметре календаря пользователя Outlook для рабочих часов. Значение представляется в формате ISO 8601 для длительности.|
|конфликтующие|Duration (Длительность)|Время, затраченное на конфликтующие собрания (собрания, перекрывающиеся с другими собраниями, которые он принял, и состоянием "занято"). Значение представляется в формате ISO 8601 для длительности.|
|long|Duration (Длительность)|Время, затраченное на длительные собрания (более часа в течение длительного времени). Значение представляется в формате ISO 8601 для длительности.|
|многозадачность|Duration (Длительность)|Время, затраченное на собрания, в которых пользователь выполнял многозадачность (чтение и отправка превышает минимальное количество сообщений электронной почты и/или отправляет больше минимального количества сообщений в Teams или Skype для бизнеса). Значение представляется в формате ISO 8601 для длительности.|
|распределяют|Duration (Длительность)|Время, затраченное на собрания, организованные пользователем. Значение представляется в формате ISO 8601 для длительности.|
|повторяющихся|Duration (Длительность)|Время, затраченное на повторяющиеся собрания. Значение представляется в формате ISO 8601 для длительности.|

## <a name="relationships"></a>Отношения

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingActivityStatistics"
}--> 

```json
{
  "activity": "string",
  "duration": "String (ISO 8601 duration)",
  "endDate": "String (ISO 8601)",
  "id": "String (identifier)",
  "startDate": "String (ISO 8601)",
  "timeZoneUsed": "String",
  "afterHours": "String (ISO 8601 duration)",
  "conflicting": "String (ISO 8601 duration)",
  "long": "String (ISO 8601 duration)",
  "multitasking": "String (ISO 8601 duration)",
  "organized": "String (ISO 8601 duration)",
  "recurring": "String (ISO 8601 duration)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingActivityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->