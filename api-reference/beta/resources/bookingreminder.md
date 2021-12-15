---
title: тип ресурса bookingReminder
description: Представляет, когда и кому отправлять напоминание по электронной почте.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 51dde51c25064edb0c6548676bb7921b7705dcf2
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2021
ms.locfileid: "61524681"
---
# <a name="bookingreminder-resource-type"></a>тип ресурса bookingReminder

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Представляет, когда и кому отправлять напоминание по электронной почте.


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|message|String|Сообщение в напоминаниях.|
|смещение|Длительность|Время, за которое необходимо отправить напоминание перед началом встречи. Он обозначается в [формате ISO 8601.](https://www.iso.org/iso-8601-date-and-time-format.html)|
|recipients|bookingReminderRecipients| Лица, которые должны получать напоминание. Возможные значения: `allAttendees` , `staff` и `customer` `unknownFutureValue` .|

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
  "recipients": {"@odata.type": "microsoft.graph.bookingReminderRecipients"}
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


