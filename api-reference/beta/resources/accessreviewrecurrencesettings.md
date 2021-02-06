---
title: Тип ресурса accessReviewRecurrenceSettings
description: Указывает, что проверка доступа повторяется с регулярными интервалами.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 208d3e8f8c73c8de98a34aadbd616dc9f268925c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136656"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a>Тип ресурса accessReviewRecurrenceSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Тип ресурса **accessReviewRecurrenceSettings** используется в ресурсе [accessReviewSettings](accessreviewsettings.md) и указывает, что проверка доступа повторяется с регулярными интервалами.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
| :------- | :--- | :---------- |
| recurrenceType | Строка | Интервал повторения. Возможные vaules: `onetime` , , , , или `weekly` `monthly` `quarterly` `halfyearly` `annual` .                                                                   |
| recurrenceEndType | Строка | Как заканчивается повторение. Возможные значения: `never` , , , или `endBy` `occurrences` `recurrenceCount` . Если это так, явный конец серии повторения `never` не существует. Если это `endBy` так, то повторение завершается в определенную дату. Если это так, серия завершается после завершения `occurrences` `recurrenceCount` экземпляров проверки. |
| durationInDays | Int32 | Продолжительность повторения в днях. |
| recurrenceCount | Int32 | Количество повторерений, если значение **recurrenceEndType** — `occurrences` или 0 в противном случае. |

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewRecurrenceSettings"
}-->
```json
{
  "recurrenceType": "string",
  "recurrenceEndType": "string",
  "durationInDays": 1024,
  "recurrenceCount": 1024
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "accessReviewRecurrenceSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
