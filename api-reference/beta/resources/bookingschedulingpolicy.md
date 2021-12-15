---
title: тип ресурса bookingSchedulingPolicy
description: Представляет набор политик, которые определяют, как следует создавать встречи в календаре Microsoft Bookings.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: c6244c573fb60e13a5419ad89cee407dfd3a497b
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526144"
---
# <a name="bookingschedulingpolicy-resource-type"></a>тип ресурса bookingSchedulingPolicy

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Представляет набор политик, которые определяют, как следует создавать встречи в календаре Microsoft Bookings.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|allowStaffSelection|Boolean|Верно, если разрешить клиентам выбирать конкретного человека для бронирования.|
|maximumAdvance|Длительность|Максимальное количество дней до того, как можно сделать бронирование. Он следует [формату ISO 8601.](https://www.iso.org/iso-8601-date-and-time-format.html)|
|minimumLeadTime|Длительность|Минимальное время, до которого необходимо сделать бронирование и отмену. Он следует [формату ISO 8601.](https://www.iso.org/iso-8601-date-and-time-format.html)|
|sendConfirmationsToOwner|Boolean| True, чтобы уведомить бизнес по электронной почте, когда бронирование создано или изменено. Используйте адрес электронной почты, указанный **в** свойстве электронной почты **объекта bookingBusiness** для бизнеса. |
|timeSlotInterval|Длительность|Длительность каждого интервала времени, обозначаемого в [формате ISO 8601.](https://www.iso.org/iso-8601-date-and-time-format.html)|

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


