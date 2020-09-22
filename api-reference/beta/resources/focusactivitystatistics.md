---
title: Тип ресурса Фокусактивитистатистикс
description: Представляет сведения об индивидуальных трудозатратах для пользователей
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 3da2dc2719f24bfd986d5a3df550b4635b734131
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052886"
---
# <a name="focusactivitystatistics-resource-type"></a>Тип ресурса Фокусактивитистатистикс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет данные о времени, доступном пользователю, для работы с фокусом. Это основано на [активитистатистикс](../resources/activitystatistics.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|activity|аналитиксактивититипе| Действие фокуса, для которого возвращается статистика.|
|duration|Длительность|Общая сумма количества часов в фокусе, равная всем блокам времени по крайней мере в два последовательных часа, в календаре Microsoft Outlook пользователя без собрания с другими людьми в рабочем времени пользователя. Значение представляется в формате ISO 8601 для длительности.|
|endDate|Date|Дата окончания действия фокуса. Значение представлено в формате ISO 8601 для календарных дат. Например, значение свойства может иметь значение "2019-07-04", которое соответствует формату ГГГГ – MM – DD.|
|id|String| Идентификатор, предназначенный только для чтения, для действия Focus.|
|startDate|Date|Дата начала действия фокуса. Значение представлено в формате ISO 8601 для календарных дат. Например, значение свойства может иметь значение "2019-07-03", которое соответствует формату ГГГГ – MM – DD.|
|тимезонеусед|String|Часовой пояс, который пользователь задает в календаре Outlook для вычисления. Например, значение свойства может быть "тихоокеанское стандартное время".|

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
  "@odata.type": "microsoft.graph.focusActivityStatistics"
}--> 

```json
{
  "activity": "string",
  "duration": "String (ISO 8601 duration)",
  "endDate": "String (ISO 8601)",
  "id": "String (identifier)",
  "startDate": "String (ISO 8601)",
  "timeZoneUsed": "String"
  }
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "focusActivityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

