---
title: Тип ресурса Каллактивитистатистикс
description: Представляет сведения о действиях звонка для пользователей.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 8d7eb23fc0ed148b38f3cb7adb29d8af49fa7400
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071575"
---
# <a name="callactivitystatistics-resource-type"></a>Тип ресурса Каллактивитистатистикс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет данные о времени, затраченном пользователем на действия звонка в Microsoft Teams или Skype для бизнеса. Это основано на [активитистатистикс](../resources/activitystatistics.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|activity|аналитиксактивититипе| Действие Call, для которого возвращается статистика.|
|duration|Длительность|Общее количество часов, потраченных на звонки. Значение представляется в формате ISO 8601 для длительности.|
|endDate|Date|Дата завершения действия звонка. Значение представлено в формате ISO 8601 для календарных дат. Например, значение свойства может иметь значение "2019-07-04", которое соответствует формату ГГГГ – MM – DD.|
|id|String| Идентификатор, предназначенный только для чтения, для действия Call.|
|startDate|Date|Дата начала действия звонка. Значение представлено в формате ISO 8601 для календарных дат. Например, значение свойства может иметь значение "2019-07-03", которое соответствует формату ГГГГ – MM – DD.|
|тимезонеусед|String|Для вычисления используется часовой пояс, который пользователь задает в календаре Microsoft Outlook. Например, значение свойства может быть "тихоокеанское стандартное время".|
|афтерхаурс|Длительность|Время, затраченное на вызовы в нерабочее время, которое основано на параметре календаря пользователя Outlook для рабочих часов. Значение представляется в формате ISO 8601 для длительности. |

## <a name="relationships"></a>Отношения

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.activityStatistics",
  "keyProperty": "id", 
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.callActivityStatistics"
}--> 

```json
{
  "activity": "string",
  "duration": "String (ISO 8601 duration)",
  "endDate": "String (ISO 8601)",
  "id": "String (identifier)",
  "startDate": "String (ISO 8601)",
  "timeZoneUsed": "String",
  "afterHours": "String (ISO 8601 duration)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "callActivityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

