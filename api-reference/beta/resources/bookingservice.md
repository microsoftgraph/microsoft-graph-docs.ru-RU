---
title: Тип ресурса bookingService
description: Представляет сведения о конкретной службе, предоставляемой bookingBusiness, например имя службы, цену и персонал, который обычно предоставляет такую услугу.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: d8c8fb849bbc452d343cb37b86e8cfae925606ae
ms.sourcegitcommit: 8253b79a9fdfea723899860492219eaeb9f74e3d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2022
ms.locfileid: "66160708"
---
# <a name="bookingservice-resource-type"></a>Тип ресурса bookingService

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Представляет сведения о конкретной службе, предоставляемой [bookingBusiness](bookingbusiness.md), например имя службы, цену и персонал, который обычно предоставляет такую услугу.

Наследуется от [bookingNamedEntity](bookingNamedEntity.md).

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Перечисление служб](../api/bookingbusiness-list-services.md) | [Коллекция bookingService](bookingservice.md) | Получение списка объектов **bookingService** в указанном [bookingbusiness](../resources/bookingbusiness.md).|
|[Создание bookingService](../api/bookingbusiness-post-services.md) | [bookingService](bookingservice.md) | Создайте **bookingService** для указанного [bookingbusiness](../resources/bookingbusiness.md). |
|[Получение bookingService](../api/bookingservice-get.md) | [bookingService](bookingservice.md) |Получение свойств и связей объекта **bookingService** в указанном [bookingbusiness](../resources/bookingbusiness.md).|
|[Обновление](../api/bookingservice-update.md) | Нет   |Обновите **объект bookingService** в указанном [bookingbusiness](../resources/bookingbusiness.md). |
|[Удаление](../api/bookingservice-delete.md) | Нет |Удаление объекта **bookingService** в указанном [bookingbusiness](../resources/bookingbusiness.md). |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|additionalInformation|Строка|Дополнительные сведения, отправляемые клиенту при подтверждении встречи.|
|customQuestions|[Коллекция bookingQuestionAssignment](../resources/bookingquestionassignment.md)| Содержит набор пользовательских вопросов, связанных с определенной службой. |
|defaultDuration|Длительность|Длина службы по умолчанию, представленная в числах дней, часов, минут и секунд. Например, P11D23H59M59.999999999999S. |
|defaultLocation|[location](location.md)|Физическое расположение службы по умолчанию.|
|defaultPrice|Двойное с плавающей точкой|Денежное значение по умолчанию для службы.|
|defaultPriceType|bookingPriceType|Способ оплаты службы по умолчанию. Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`, `unknownFutureValue`.|
|defaultReminders|[Коллекция bookingReminder](bookingreminder.md)|Набор напоминаний по умолчанию для встречи этой службы. Значение этого свойства доступно только при чтении этой **службы bookingService** по его идентификатору.|
|description|Строка|Текстовое описание службы.|
|displayName|Строка|Имя службы.|
|id|Строка|Идентификатор этой службы в формате GUID. Только для чтения.|
|isAnonymousJoinEnabled|Boolean|`True` Значение , если для встречи, заданной для этой службы, будет создан anonymousJoinWebUrl(webrtcUrl).
|isHiddenFromCustomers|Boolean|Значение true означает, что эта служба недоступна клиентам для резервирования.|
|isLocationOnline|Boolean|Значение true указывает, что встречи для службы будут храниться в сети. Значение по умолчанию − ложь.|
|languageTag|Строка|Язык страницы самостоятельного резервирования.
|maximumAttendeesCount|Int32|Максимальное число клиентов, разрешенных в службе. Если **значение maximumAttendeesCount** службы больше 1, передайте допустимые идентификаторы клиентов при создании или обновлении встречи.  Чтобы создать клиента, используйте операцию [Create bookingCustomer](../api/bookingbusiness-post-customers.md) .  |
|notes|String|Дополнительные сведения об этой службе.|
|postBuffer|Длительность|Время буферизации после окончания встречи для этой службы и до того, как можно будет заказать следующую встречу клиента.|
|preBuffer|Длительность|Время буферизации до начала встречи для этой службы.|
|schedulingPolicy|[bookingSchedulingPolicy](bookingschedulingpolicy.md)|Набор политик, определяющий способ создания и управления встречами для этого типа службы.|
|smsNotificationsEnabled|Boolean|Значение true SMS, что клиенты могут отправлять уведомления о встрече службы. Значение по умолчанию − ложь.|
|staffMemberIds|Коллекция String|Представляет сотрудников [, предоставляющих](bookingstaffmember.md) эту службу. |
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
  "languageTag": "String",
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
  "isAnonymousJoinEnabled": "Boolean",
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


