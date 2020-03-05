---
title: Тип ресурса Букингсчедулингполици
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: edc456aaa03cc54bd7b385bc97d37eb657ea53b2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507910"
---
# <a name="bookingschedulingpolicy-resource-type"></a>Тип ресурса Букингсчедулингполици

Пространство имен: Microsoft. Graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Представляет набор политик, определяющих, как будут создаваться встречи в календаре Microsoft Books.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|алловстаффселектион|Логический|Значение true, если необходимо разрешить клиентам выбирать определенного человека для резервирования.|
|максимумадванце|Длительность|Максимальное количество дней, в течение которых можно выполнить резервирование. Он соответствует формату [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|минимумлеадтиме|Длительность|Минимальное время, по истечении которого должны выполняться резервирования и отмены. Он соответствует формату [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|сендконфирматионстувнер|Логический| Значение true, чтобы уведомить бизнес по электронной почте при создании или изменении резервирования. Используйте адрес электронной почты, указанный в свойстве **Email** объекта **букингбусинесс** для бизнеса. |
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
