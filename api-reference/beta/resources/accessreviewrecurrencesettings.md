---
title: тип ресурса accessReviewRecurrenceSettings
description: Указывает, что обзор доступа повторяется через регулярные промежутки времени.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: cb2a05589bfa92331a213a489bfb2a5129850065
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755660"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a>тип ресурса accessReviewRecurrenceSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

Тип **ресурса accessReviewRecurrenceSettings** используется в [ресурсе accessReviewSettings](accessreviewsettings.md) и указывает, что обзор доступа повторяется регулярно.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
| :------- | :--- | :---------- |
| recurrenceType | String | Интервал повторяемости. Возможные vaules: `onetime` , , , , или `weekly` `monthly` `quarterly` `halfyearly` `annual` .                                                                   |
| recurrenceEndType | String | Как заканчивается повторение. Возможные значения: `never` `endBy` , , или `occurrences` `recurrenceCount` . Если это так, то явный конец серии рецидивов `never` не существует. Если это `endBy` так, то повторение заканчивается в определенный срок. Если это так, то серия заканчивается после завершения экземпляров `occurrences` `recurrenceCount` проверки. |
| durationInDays | Int32 | Продолжительность в днях для повторения. |
| recurrenceCount | Int32 | Количество повторерений, если значение **recurrenceEndType** является `occurrences` или `0` иным образом. |

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
