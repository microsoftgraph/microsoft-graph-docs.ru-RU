---
title: Тип ресурса accessReviewRecurrenceSettings (не рекомендуется)
description: Указывает, что проверка доступа выполняется через регулярные интервалы.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9fa6fb47c541094c85778621289d1abb6d71f727
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65821213"
---
# <a name="accessreviewrecurrencesettings-resource-type-deprecated"></a>Тип ресурса accessReviewRecurrenceSettings (не рекомендуется)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

Тип **ресурса accessReviewRecurrenceSettings** используется в ресурсе [accessReviewSettings](accessreviewsettings.md) и указывает, что проверка доступа выполняется через регулярные интервалы.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
| :------- | :--- | :---------- |
| recurrenceType | Строка | Интервал повторения. Возможные vaules: , , , , или `annual``quarterly``halfyearly` . `monthly``weekly``onetime`                                                                   |
| recurrenceEndType | Строка | Как заканчивается повторение. Возможные значения: `never`, `endBy`, или `occurrences``recurrenceCount`. Если это так `never`, то явный конец ряда повторений отсутствует. Если это так `endBy`, то повторение заканчивается в определенную дату. Если это так `occurrences`, то ряд завершается `recurrenceCount` после завершения экземпляров проверки. |
| durationInDays | Int32 | Длительность повторения в днях. |
| recurrenceCount | Int32 | Количество повторений, если значение **recurrenceEndType** равно `occurrences`или иным `0` образом. |

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
