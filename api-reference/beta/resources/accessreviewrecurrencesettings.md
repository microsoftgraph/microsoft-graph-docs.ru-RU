---
title: Тип ресурса Акцессревиеврекурренцесеттингс
description: Указывает, что проверка доступа повторяется через регулярные промежутки времени.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3ca66a818059efac84903f763e6be3c8a3b5c05a
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330181"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a>Тип ресурса Акцессревиеврекурренцесеттингс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Тип ресурса **акцессревиеврекурренцесеттингс** используется в ресурсе [акцессревиевсеттингс](accessreviewsettings.md) и указывает, что проверка доступа повторяется через регулярные промежутки времени.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
| :------- | :--- | :---------- |
| recurrenceType | Строка | Интервал повторения. Возможные ваулес: `onetime` , `weekly` , `monthly` , `quarterly` , `halfyearly` или `annual` .                                                                   |
| рекурренцеендтипе | Строка | Завершение повторения. Возможные значения: `never` , `endBy` , `occurrences` , или `recurrenceCount` . Если это так `never` , то отсутствует явный конец ряда повторений. Если это так `endBy` , повторение оканчивается на определенную дату. Если это так `occurrences` , ряд завершается после `recurrenceCount` завершения экземпляров проверки. |
| дуратиониндайс | Int32 | Продолжительность повторения в днях. |
| рекурренцекаунт | Int32 | Количество повторений, если значение параметра **рекурренцеендтипе** равно `occurrences` или 0 в противном случае. |

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