---
title: Тип ресурса Емаилактивитистатистикс
description: Представляет дополнительные сведения о действиях электронной почты для пользователей
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: af0fbc4247e7ffc9c8285409789d0437d8e09cb5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055514"
---
# <a name="emailactivitystatistics-resource-type"></a>Тип ресурса Емаилактивитистатистикс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет данные о времени, затраченном пользователем на действия с электронной почтой, в Microsoft Outlook. Это основано на [активитистатистикс](../resources/activitystatistics.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|activity|аналитиксактивититипе| Действия электронной почты, для которых возвращается статистика.|
|duration|Длительность|Общее количество часов, потраченных на электронную почту. Значение представляется в формате ISO 8601 для длительности.|
|endDate|Date|Дата окончания действия электронной почты. Значение представлено в формате ISO 8601 для календарных дат. Например, значение свойства может иметь значение "2019-07-04", которое соответствует формату ГГГГ – MM – DD.|
|id|String| Идентификатор, предназначенный только для чтения, для действия электронной почты.|
|startDate|Date|Дата начала действия электронной почты. Значение представлено в формате ISO 8601 для календарных дат. Например, значение свойства может иметь значение "2019-07-03", которое соответствует формату ГГГГ – MM – DD.|
|тимезонеусед|String|Часовой пояс, который пользователь задает в календаре Outlook для вычисления. Например, значение свойства может быть "тихоокеанское стандартное время".|
|афтерхаурс|Длительность|Общее количество часов, потраченных на электронную почту за прев рабочее время, которая основана на параметре календаря пользователя Outlook для рабочих часов. Значение представляется в формате ISO 8601 для длительности. |
|реадемаил|Длительность|Общее количество часов, потраченных на чтение электронной почты. Значение представляется в формате ISO 8601 для длительности.|
|сентемаил|Длительность|Общее количество часов, потраченных на запись и отправку электронной почты. Значение представляется в формате ISO 8601 для длительности.|

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

