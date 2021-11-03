---
title: Тип ресурса bookingService
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: f75bca271ffd33b36b7e0a1f5ed726ae417d4a0c
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694913"
---
# <a name="bookingservice-resource-type"></a>Тип ресурса bookingService

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Представляет сведения о конкретной службе, предоставляемой [bookingBusiness,](bookingbusiness.md)например имя службы, цена и персонал, который обычно предоставляет такую услугу.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Службы списка](../api/bookingbusiness-list-services.md) | [коллекция bookingService](bookingservice.md) | Получите список объектов **bookingService** в указанном [bookingbusiness.](../resources/bookingbusiness.md)|
|[Создание bookingService](../api/bookingbusiness-post-services.md) | [bookingService](bookingservice.md) | Создайте **bookingService** для указанного [bookingbusiness.](../resources/bookingbusiness.md) |
|[Получить bookingService](../api/bookingservice-get.md) | [bookingService](bookingservice.md) |Получите свойства и связи объекта **bookingService** в указанном [bookingbusiness.](../resources/bookingbusiness.md)|
|[Обновление](../api/bookingservice-update.md) | [bookingService](bookingservice.md)    |Обновление объекта **bookingService** в указанном [bookingbusiness](../resources/bookingbusiness.md). |
|[Удаление](../api/bookingservice-delete.md) | Нет |Удаление объекта **bookingService** в указанном [bookingbusiness](../resources/bookingbusiness.md). |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|defaultDuration|Длительность|Длина службы по умолчанию, представленная в числах дней, часов, минут и секунд. Например, P11D23H59M59.999999999999S. |
|defaultLocation|[location](location.md)|Физическое расположение службы по умолчанию.|
|defaultPrice|Double|Денежная цена по умолчанию для службы.|
|defaultPriceType|string|Способ заряжания службы по умолчанию. Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.|
|defaultReminders|[коллекция bookingReminder](bookingreminder.md)|Набор напоминаний по умолчанию для назначения этой службы. Значение этого свойства доступно только при чтении этого **bookingService** по его ID.|
|description|String|Текстовое описание службы.|
|displayName|String|Имя службы.|
|emailAddress|String|Адрес электронной почты|
|id|String|ID этой службы в формате GUID. Только для чтения.|
|isHiddenFromCustomers|Логический|True означает, что эта служба недоступна клиентам для бронирования.|
|isLocationOnline|Логический|True указывает, что встречи для службы будут проводиться онлайн. Значение по умолчанию − ложь.|
|notes|String|Дополнительные сведения об этой службе.|
|postBuffer|Длительность|Время буферизации после назначения для этой службы заканчивается, и до следующей встречи клиента можно заказать.|
|preBuffer|Длительность|Время буферизации перед назначением для этой службы может начаться.|
|schedulingPolicy|[bookingSchedulingPolicy](bookingschedulingpolicy.md)|Набор политик, которые определяют, как следует создавать и управлять встречами для этого типа службы.|
|smsNotificationsEnabled|Логический|True указывает, что sms-уведомления можно отправить клиентам для назначения службы. Значение по умолчанию − ложь.|
|staffMemberIds|Коллекция строк|Представляет тех [сотрудников,](bookingstaffmember.md) которые предоставляют эту службу. |
|webUrl|String|URL-адрес, который клиент использует для доступа к службе.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingService"
}-->

```json
{
  "defaultDuration": "String (timestamp)",
  "defaultLocation": {"@odata.type": "microsoft.graph.location"},
  "defaultPrice": 1024,
  "defaultPriceType": "string",
  "defaultReminders": [{"@odata.type": "microsoft.graph.bookingReminder"}],
  "description": "String",
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)",
  "isHiddenFromCustomers": true,
  "isLocationOnline": "Boolean",
  "notes": "String",
  "postBuffer": "String (timestamp)",
  "preBuffer": "String (timestamp)",
  "schedulingPolicy": {"@odata.type": "microsoft.graph.bookingSchedulingPolicy"},
  "smsNotificationsEnabled": "Boolean",
  "staffMemberIds": ["String"],
  "webUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingService resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


