---
title: Тип ресурса bookingReminder
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: 1f1708d4ac9606ad5c862cb9b1bc73e1ddcfec4a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853867"
---
# <a name="bookingreminder-resource-type"></a>Тип ресурса bookingReminder

 > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.
 
Представляет при и к которым следует отправить по электронной почте напоминания.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|message|String|Сообщение в напоминания.|
|Смещение|Продолжительность|Количество времени до начала встречи, на который будут отправляться напоминания. Отображаются в формате [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|recipients|Строка| Лиц, которые shouold получать оповещение. Возможные значения: `allAttendees`, `staff`, `customer`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingReminder"
}-->

```json
{
  "message": "String",
  "offset": "String (timestamp)",
  "recipients": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingReminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
