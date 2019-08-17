---
title: Тип ресурса Каллактивитистатистикс
description: Представляет сведения о действиях звонка для пользователей.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 014cec3f8adab9f8d41b9f3062b38898b9956bb6
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450815"
---
# <a name="callactivitystatistics-resource-type"></a>Тип ресурса Каллактивитистатистикс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет данные о времени, затраченном пользователем на действия звонка в Microsoft Teams или Skype для бизнеса. Это основано на [активитистатистикс](../resources/activitystatistics.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|activity|аналитиксактивититипе| Действие Call, для которого возвращается статистика.|
|duration|Duration (Длительность)|Общее количество часов, потраченных на звонки. Значение представляется в формате ISO 8601 для длительности.|
|endDate|Date|Дата завершения действия звонка. Значение представлено в формате ISO 8601 для календарных дат. Например, значение свойства может иметь значение "2019-07-04", которое соответствует формату ГГГГ – MM – DD.|
|id|String| Идентификатор, предназначенный только для чтения, для действия Call.|
|startDate|Дата|Дата начала действия звонка. Значение представлено в формате ISO 8601 для календарных дат. Например, значение свойства может иметь значение "2019-07-03", которое соответствует формату ГГГГ – MM – DD.|
|тимезонеусед|String|Для вычисления используется часовой пояс, который пользователь задает в календаре Microsoft Outlook. Например, значение свойства может быть "тихоокеанское стандартное время".|
|афтерхаурс|Duration (Длительность)|Время, затраченное на вызовы в нерабочее время, которое основано на параметре календаря пользователя Outlook для рабочих часов. Значение представляется в формате ISO 8601 для длительности. |

## <a name="relationships"></a>Отношения

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
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