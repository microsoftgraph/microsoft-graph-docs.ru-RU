---
title: Тип ресурса Букингсчедулингполици
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 77b1cf812edd334197c268c92bb982954fb11b12
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974124"
---
# <a name="bookingschedulingpolicy-resource-type"></a>Тип ресурса Букингсчедулингполици

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Представляет набор политик, определяющих, как будут создаваться встречи в календаре Microsoft Books.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Алловстаффселектион|Boolean|Значение true, если необходимо разрешить клиентам выбирать определенного человека для резервирования.|
|Максимумадванце|Duration (Длительность)|Максимальное количество дней, в течение которых можно выполнить резервирование. Он соответствует формату [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|Минимумлеадтиме|Duration (Длительность)|Минимальное время, по истечении которого должны выполняться резервирования и отмены. Он соответствует формату [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|Сендконфирматионстувнер|Boolean| Значение true, чтобы уведомить бизнес по электронной почте при создании или изменении резервирования. Используйте адрес электронной почты, указанный в свойстве **Email** объекта **букингбусинесс** для бизнеса. |
|Тимеслотинтервал|Duration (Длительность)|Продолжительность каждого интервала времени, обозначенного в формате [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingSchedulingPolicy"
}-->

```json
{
  "allowStaffSelection": true,
  "maximumAdvance": "String (timestamp)",
  "minimumLeadTime": "String (timestamp)",
  "sendConfirmationsToOwner": true,
  "timeSlotInterval": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingSchedulingPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
