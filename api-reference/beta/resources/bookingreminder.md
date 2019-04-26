---
title: Тип ресурса Букингреминдер
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 18265a9d9e86b79706b6a268df3b8512b7b65111
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328208"
---
# <a name="bookingreminder-resource-type"></a>Тип ресурса Букингреминдер

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Указывает, когда и кому отправлять напоминания по электронной почте.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|message|String|Сообщение в памятке.|
|корреспондирующей|Duration (Длительность)|Количество времени до начала встречи, в которое будет отправлено напоминание. Он отмечен в формате [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|recipients|String| Лица, шауолд получать напоминание. Возможные значения: `allAttendees`, `staff`, `customer`.|

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
<!--
{
  "type": "#page.annotation",
  "description": "bookingReminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
