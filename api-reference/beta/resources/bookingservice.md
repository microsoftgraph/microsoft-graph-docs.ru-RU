---
title: Тип ресурса bookingService
description: Представляет сведения о конкретной службе, предоставляемой bookingBusiness, например имя службы, цена и персонал, который обычно предоставляет такую услугу.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 8d547ea9870642ebf56f2f7c07608b17a5639dce
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63368233"
---
# <a name="bookingservice-resource-type"></a>Тип ресурса bookingService

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Представляет сведения о конкретной службе, предоставляемой [bookingBusiness](bookingbusiness.md), например имя службы, цена и персонал, который обычно предоставляет такую услугу.

Наследует от [bookingNamedEntity](bookingNamedEntity.md).

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Службы списка](../api/bookingbusiness-list-services.md) | [коллекция bookingService](bookingservice.md) | Получите список объектов **bookingService** в указанном [bookingbusiness](../resources/bookingbusiness.md).|
|[Создание bookingService](../api/bookingbusiness-post-services.md) | [bookingService](bookingservice.md) | Создайте **bookingService** для указанного [bookingbusiness](../resources/bookingbusiness.md). |
|[Получить bookingService](../api/bookingservice-get.md) | [bookingService](bookingservice.md) |Получите свойства и связи объекта **bookingService** в указанном [bookingbusiness](../resources/bookingbusiness.md).|
|[Обновление](../api/bookingservice-update.md) | [bookingService](bookingservice.md)    |Обновление объекта **bookingService** в указанном [bookingbusiness](../resources/bookingbusiness.md). |
|[удаление](../api/bookingservice-delete.md); | Нет |Удаление объекта **bookingService** в указанном [bookingbusiness](../resources/bookingbusiness.md). |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|additionalInformation|Строка|Дополнительные сведения, которые отправляются клиенту при подтверждении встречи.|
|customQuestions|[коллекция bookingQuestionAssignment](../resources/bookingquestionassignment.md)| Содержит набор пользовательских вопросов, связанных с определенной службой. |
|defaultDuration|Длительность|Длина службы по умолчанию, представленная в числах дней, часов, минут и секунд. Например, P11D23H59M59.999999999999S. |
|defaultLocation|[location](location.md)|Физическое расположение службы по умолчанию.|
|defaultPrice|Double|Денежная цена по умолчанию для службы.|
|defaultPriceType|bookingPriceType|Способ заряжания службы по умолчанию. Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`, `unknownFutureValue`.|
|defaultReminders|[коллекция bookingReminder](bookingreminder.md)|Набор напоминаний по умолчанию для назначения этой службы. Значение этого свойства доступно только при чтении этого **bookingService** по его ID.|
|description|Строка|Текстовое описание службы.|
|displayName|String|Имя службы.|
|id|Строка|ID этой службы в формате GUID. Только для чтения.|
|isHiddenFromCustomers|Boolean|True означает, что эта служба недоступна клиентам для бронирования.|
|isLocationOnline|Boolean|True указывает, что встречи для службы будут проводиться онлайн. Значение по умолчанию − ложь.|
|maximumAttendeesCount|Int32|Максимальное число клиентов, разрешенных в службе. Если **значение maximumAttendeesCount** службы превышает 1, передай действительные удостоверения клиентов при создании или обновлении встречи.  Чтобы создать клиента, используйте операцию [Create bookingCustomer](../api/bookingbusiness-post-customers.md) .  |
|notes|String|Дополнительные сведения об этой службе.|
|postBuffer|Длительность|Время буферизации после назначения для этой службы заканчивается, и до следующей встречи клиента можно заказать.|
|preBuffer|Длительность|Время буферизации перед назначением для этой службы может начаться.|
|schedulingPolicy|[bookingSchedulingPolicy](bookingschedulingpolicy.md)|Набор политик, которые определяют, как следует создавать и управлять встречами для этого типа службы.|
|smsNotificationsEnabled|Boolean|True указывает, что sms-уведомления можно отправить клиентам для назначения службы. Значение по умолчанию − ложь.|
|staffMemberIds|Коллекция String|Представляет тех [сотрудников,](bookingstaffmember.md) которые предоставляют эту службу. |
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
  "additionalInformation": "String",
  "defaultDuration": "String (timestamp)",
  "defaultLocation": {"@odata.type": "microsoft.graph.location"},
  "defaultPrice": 1024,
  "defaultPriceType": {"@odata.type": "microsoft.graph.bookingPriceType"},
  "defaultReminders": [{"@odata.type": "microsoft.graph.bookingReminder"}],
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isHiddenFromCustomers": true,
  "isLocationOnline": "Boolean",
  "notes": "String",
  "postBuffer": "String (timestamp)",
  "preBuffer": "String (timestamp)",
  "schedulingPolicy": {"@odata.type": "microsoft.graph.bookingSchedulingPolicy"},
  "smsNotificationsEnabled": "Boolean",
  "staffMemberIds": ["String"],
  "customQuestions": [
    {
      "@odata.type": "microsoft.graph.bookingQuestionAssignment"
    }
  ],
  "maximumAttendeesCount": "Integer",
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


