---
title: Тип ресурса Емаилактивитистатистикс
description: Представляет дополнительные сведения о действиях электронной почты для пользователей
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: ff75545b7f591a920ed4a1ffd65bff40cff8439b
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450813"
---
# <a name="emailactivitystatistics-resource-type"></a>Тип ресурса Емаилактивитистатистикс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет данные о времени, затраченном пользователем на действия с электронной почтой, в Microsoft Outlook. Это основано на [активитистатистикс](../resources/activitystatistics.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|activity|аналитиксактивититипе| Действия электронной почты, для которых возвращается статистика.|
|duration|Duration (Длительность)|Общее количество часов, потраченных на электронную почту. Значение представляется в формате ISO 8601 для длительности.|
|endDate|Date|Дата окончания действия электронной почты. Значение представлено в формате ISO 8601 для календарных дат. Например, значение свойства может иметь значение "2019-07-04", которое соответствует формату ГГГГ – MM – DD.|
|id|String| Идентификатор, предназначенный только для чтения, для действия электронной почты.|
|startDate|Дата|Дата начала действия электронной почты. Значение представлено в формате ISO 8601 для календарных дат. Например, значение свойства может иметь значение "2019-07-03", которое соответствует формату ГГГГ – MM – DD.|
|тимезонеусед|String|Часовой пояс, который пользователь задает в календаре Outlook для вычисления. Например, значение свойства может быть "тихоокеанское стандартное время".|
|афтерхаурс|Duration (Длительность)|Общее количество часов, потраченных на электронную почту за прев рабочее время, которая основана на параметре календаря пользователя Outlook для рабочих часов. Значение представляется в формате ISO 8601 для длительности. |
|реадемаил|Duration (Длительность)|Общее количество часов, потраченных на чтение электронной почты. Значение представляется в формате ISO 8601 для длительности.|
|сентемаил|Duration (Длительность)|Общее количество часов, потраченных на запись и отправку электронной почты. Значение представляется в формате ISO 8601 для длительности.|

## <a name="relationships"></a>Отношения

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailActivityStatistics"
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
  "readEmail": "String (ISO 8601 duration)",
  "sentEmail": "String (ISO 8601 duration)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailActivityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->