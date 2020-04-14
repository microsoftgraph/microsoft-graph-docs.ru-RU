---
title: Тип ресурса Букингсчедулингполици
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 59884eaf1fa3227214b00936298a4adee5a7491f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448376"
---
# <a name="bookingschedulingpolicy-resource-type"></a>Тип ресурса Букингсчедулингполици

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Представляет набор политик, определяющих, как будут создаваться встречи в календаре Microsoft Books.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|алловстаффселектион|Логическое|Значение true, если необходимо разрешить клиентам выбирать определенного человека для резервирования.|
|максимумадванце|Длительность|Максимальное количество дней, в течение которых можно выполнить резервирование. Он соответствует формату [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|минимумлеадтиме|Длительность|Минимальное время, по истечении которого должны выполняться резервирования и отмены. Он соответствует формату [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|сендконфирматионстувнер|Логическое| Значение true, чтобы уведомить бизнес по электронной почте при создании или изменении резервирования. Используйте адрес электронной почты, указанный в свойстве **Email** объекта **букингбусинесс** для бизнеса. |
|тимеслотинтервал|Длительность|Продолжительность каждого интервала времени, обозначенного в формате [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|

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
