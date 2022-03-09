---
title: тип ресурса bookingAppointment
description: Представляет назначение клиента для bookingService, выполняемого набором сотрудников, предоставляемым бизнесом Microsoft Bookings.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: c5e301d6ef48015feb417bf663709fd4024a3c4e
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63367617"
---
# <a name="bookingappointment-resource-type"></a>тип ресурса bookingAppointment

Пространство имен: microsoft.graph
 
Представляет назначение клиента для [bookingService](bookingservice.md), выполняемого набором сотрудников, предоставляемым бизнесом Microsoft Bookings.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список встреч](../api/bookingbusiness-list-appointments.md) |  [коллекция bookingAppointment](bookingappointment.md) | Получите список объектов **bookingAppointment** в указанном [bookingBusiness](../resources/bookingbusiness.md). |
|[Создание bookingAppointment](../api/bookingbusiness-post-appointments.md) |  [bookingAppointment](bookingappointment.md) | Создайте **новое bookingAppointment** для указанного [bookingBusiness](../resources/bookingbusiness.md). |
|[Получить bookingAppointment](../api/bookingappointment-get.md) | [bookingAppointment](bookingappointment.md) |Ознакомьтесь с свойствами и отношениями **объекта bookingAppointment** .|
|[Обновление](../api/bookingappointment-update.md) | [bookingAppointment](bookingappointment.md)    |Обновление объекта **bookingAppointment** . |
|[удаление](../api/bookingappointment-delete.md); | Нет |Удаление **объекта bookingAppointment** . |
|[Отмена](../api/bookingappointment-cancel.md)|Нет| Отмена **объекта bookingAppointment** .|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|additionalInformation|Строка|Дополнительные сведения, которые отправляются клиенту при подтверждении встречи.|
|клиенты|[коллекция bookingCustomerInformation](../resources/bookingcustomerinformation.md)|В нем перечислены свойства клиента для встречи. Встреча будет содержать список сведений о клиентах, и каждое подразделение будет указывать свойства клиента, который является частью этого назначения. Необязательное свойство.|
|customerTimeZone|Строка|Часовой пояс клиента. Список возможных значений см. в [списке dateTimeTimeZone](datetimetimezone.md).|
|duration|Длительность|Продолжительность встречи, обозначаемая в [формате ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|endDateTime|[dateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс, которые заканчивается встреча.|
|filledAttendeesCount|Int32|Текущее число клиентов в приеме |
|id|String| ID **bookingAppointment**. Только для чтения.|
|isLocationOnline|Boolean|Если `true`, указывает, что встреча будет проходить в Интернете. Значение по умолчанию — `false`.|
|joinWebUrl|String|URL-адрес собрания в Интернете для встречи.|
|maximumAttendeesCount|Int32|Максимальное число клиентов, разрешенных при встрече. Если **значение maximumAttendeesCount** службы превышает 1, передай действительные удостоверения клиентов при создании или обновлении встречи. Чтобы создать клиента, используйте операцию [Create bookingCustomer](../api/bookingbusiness-post-customers.md) . |
|optOutOfCustomerEmail|Boolean|Если `true` указывает, что [bookingCustomer](bookingcustomer.md) для этого назначения не желает получать подтверждение для этого назначения.|
|postBuffer|Длительность|Количество времени, необходимое для резерва после окончания встречи, для очистки в качестве примера. Значение выражается в [формате ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|preBuffer|Длительность|Количество времени, необходимое для резерва перед началом встречи, для подготовки в качестве примера. Значение выражается в [формате ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|цена|Double|Обычная цена встречи для указанного [bookingService](bookingservice.md).|
|priceType|bookingPriceType| Параметр, который обеспечивает гибкость структуры ценообразования служб. Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`, `unknownFutureValue`.|
|напоминания|[коллекция bookingReminder](bookingreminder.md)|Коллекция напоминаний клиентов, отправленных для этого назначения. Значение этого свойства доступно только при чтении этого **bookingAppointment** по его ID.|
|selfServiceAppointmentId|Строка|Дополнительный ИД отслеживания для встречи, если назначение было создано непосредственно клиентом на странице планирования, а не сотрудником от имени клиента. Поддерживается только при назначении, если maxAttendeeCount — 1.|
|serviceId|Строка|ID службы [bookingService](bookingservice.md) , связанной с этим назначением.|
|serviceLocation|[location](location.md)|Расположение, в котором доставляется служба.|
|serviceName|String|Имя **bookingService, связанного** с этим назначением.<br>Это свойство является необязательным при создании новой встречи. Если не указано, оно вычисляется из службы, связанной с назначением **свойством serviceId** .|
|serviceNotes|String|Заметки [из bookingStaffMember](bookingstaffmember.md). Значение этого свойства доступно только при чтении этого **bookingAppointment** по его ID.|
|smsNotificationsEnabled|Boolean|Если `true`, указывает SMS-уведомления будут отправлены клиентам для встречи. Значение по умолчанию — `false`.|
|staffMemberIds|Коллекция объектов string|ID каждого [бронированияStaffMember](bookingstaffmember.md) , который запланирован в этом назначении.|
|startDateTime|[dateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс, в который начинается встреча.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingAppointment"
}-->

```json
{
  "customers": [
    {
      "@odata.type": "microsoft.graph.bookingCustomerInformation"
    }
  ],
  "duration": "String (timestamp)",
  "endDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "id": "String (identifier)",
  "isLocationOnline": "Boolean",
  "joinWebUrl": "String",
  "optOutOfCustomerEmail": "Boolean",
  "postBuffer": "String (timestamp)",
  "preBuffer": "String (timestamp)",
  "price": "Integer",
  "priceType": {"@odata.type": "microsoft.graph.bookingPriceType"},
  "reminders": [{"@odata.type": "microsoft.graph.bookingReminder"}],
  "selfServiceAppointmentId": "String",
  "serviceId": "String",
  "serviceLocation": {"@odata.type": "microsoft.graph.location"},
  "serviceName": "String",
  "serviceNotes": "String",
  "smsNotificationsEnabled": "Boolean",
  "staffMemberIds": ["String"],
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "maximumAttendeesCount": "Integer",
  "filledAttendeesCount": "Integer"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingAppointment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


