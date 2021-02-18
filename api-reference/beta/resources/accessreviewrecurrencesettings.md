---
title: Тип ресурса accessReviewRecurrenceSettings
description: Указывает, что проверка доступа повторяется с регулярными интервалами.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9a39881a7675598d12de79f2738a1e14d1c759b3
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292926"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a>Тип ресурса accessReviewRecurrenceSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

Тип ресурса **accessReviewRecurrenceSettings** используется в ресурсе [accessReviewSettings](accessreviewsettings.md) и указывает, что проверка доступа повторяется с регулярными интервалами.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
| :------- | :--- | :---------- |
| recurrenceType | String | Интервал повторения. Возможные vaules: `onetime` , , , , или `weekly` `monthly` `quarterly` `halfyearly` `annual` .                                                                   |
| recurrenceEndType | String | Как заканчивается повторение. Возможные значения: `never` , , , или `endBy` `occurrences` `recurrenceCount` . Если это так, явный конец серии `never` повторения не существует. Если это `endBy` так, то повторение завершается в определенную дату. Если это так, серия завершается после завершения `occurrences` `recurrenceCount` экземпляров проверки. |
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
