---
title: Тип ресурса Митингактивитистатистикс
description: Представляет сведения о действиях с собраниями для пользователей.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 3d1f9c7ad147b6aa3f4d52c314931d5c40af2b47
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971694"
---
# <a name="meetingactivitystatistics-resource-type"></a>Тип ресурса Митингактивитистатистикс

Пространство имен: microsoft.graph

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
|duration|Длительность|Общее количество часов, потраченных на собрания. Значение представляется в формате ISO 8601 для длительности.|
|endDate|Date|Дата завершения действия собрания. Значение представлено в формате ISO 8601 для календарных дат. Например, значение свойства может иметь значение "2019-07-04", которое соответствует формату ГГГГ – MM – DD.|
|id|String| Идентификатор, предназначенный только для чтения, для действия собрания.|
|startDate|Date|Дата начала действия собрания. Значение представлено в формате ISO 8601 для календарных дат. Например, значение свойства может иметь значение "2019-07-03", которое соответствует формату ГГГГ – MM – DD.|
|тимезонеусед|String|Для вычисления используется часовой пояс Outlook, который пользователь задает в календаре Outlook. Например, значение свойства может быть "тихоокеанское стандартное время".|
|афтерхаурс|Длительность|Время, затраченное на собрания в нерабочее время, которое основано на параметре календаря пользователя Outlook для рабочих часов. Значение представляется в формате ISO 8601 для длительности.|
|конфликтующие|Длительность|Время, затраченное на конфликтующие собрания (собрания, перекрывающиеся с другими собраниями, которые он принял, и состоянием "занято"). Значение представляется в формате ISO 8601 для длительности.|
|long|Длительность|Время, затраченное на длительные собрания (более часа в течение длительного времени). Значение представляется в формате ISO 8601 для длительности.|
|многозадачность|Длительность|Время, затраченное на собрания, в которых пользователь выполнял многозадачность (чтение и отправка превышает минимальное количество сообщений электронной почты и/или отправляет больше минимального количества сообщений в Teams или Skype для бизнеса). Значение представляется в формате ISO 8601 для длительности.|
|распределяют|Длительность|Время, затраченное на собрания, организованные пользователем. Значение представляется в формате ISO 8601 для длительности.|
|повторяющихся|Длительность|Время, затраченное на повторяющиеся собрания. Значение представляется в формате ISO 8601 для длительности.|

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.activityStatistics",
  "keyProperty": "id",
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

