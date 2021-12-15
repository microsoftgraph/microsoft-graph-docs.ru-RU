---
title: тип ресурса bookingAppointment
description: Представляет назначение клиента для bookingService, выполняемого набором сотрудников, предоставляемым бизнесом Microsoft Bookings.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: efb4616d2ecca386bccbdf4f83cab97e9417fda1
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2021
ms.locfileid: "61524590"
---
# <a name="bookingappointment-resource-type"></a>тип ресурса bookingAppointment

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Представляет встречу клиента для [bookingService,](bookingservice.md)выполняемую набором сотрудников, предоставляемым бизнесом Microsoft Bookings.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список встреч](../api/bookingbusiness-list-appointments.md) |  [коллекция bookingAppointment](bookingappointment.md) | Получите список объектов **bookingAppointment** в указанном [bookingbusiness.](../resources/bookingbusiness.md) |
|[Создание bookingAppointment](../api/bookingbusiness-post-appointments.md) |  [bookingAppointment](bookingappointment.md) | Создайте новое **bookingAppointment** для указанного [bookingbusiness.](../resources/bookingbusiness.md) |
|[Получить bookingAppointment](../api/bookingappointment-get.md) | [bookingAppointment](bookingappointment.md) |Ознакомьтесь с свойствами и отношениями **объекта bookingAppointment.**|
|[Обновление](../api/bookingappointment-update.md) | [bookingAppointment](bookingappointment.md)    |Обновление объекта **bookingAppointment.** |
|[удаление](../api/bookingappointment-delete.md); | Нет |Удаление **объекта bookingAppointment.** |
|[Отмена](../api/bookingappointment-cancel.md)|Нет| Отмена **объекта bookingAppointment.**|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|additionalInformation|Строка|Дополнительные сведения, которые отправляются клиенту при подтверждении встречи.|
|customerEmailAddress|Строка|SMTP-адрес [bookingCustomer,](bookingcustomer.md) который бронирует встречу.|
|customerId|Строка|ID [bookingCustomer](bookingcustomer.md) для этого назначения. Если при назначении не указывается номер, создается новый объект **bookingCustomer.** После набора следует считать **customerId** неуменяемым.|
|customerLocation|[location](location.md)|Представляет сведения о расположении [для bookingCustomer,](bookingcustomer.md) который бронирует встречу.|
|имя клиента|Строка|Имя клиента.|
|customerNotes|Строка|Заметки от клиента, связанного с этим назначением. Значение можно получить только при чтении этого **bookingAppointment** по его ID. <br> Это свойство можно установить только при первоначальном создании встречи с новым клиентом. После этого значение вычисляется от клиента, представленного **customerId.**|
|customerPhone|Строка|Номер телефона клиента.|
|клиенты|[коллекция bookingCustomerInformation](../resources/bookingcustomerinformation.md)|В нем перечислены свойства клиента для встречи. Встреча будет содержать список сведений о клиентах, и каждое подразделение будет указывать свойства клиента, который является частью этого назначения. Необязательное свойство.|
|customerTimeZone|Строка|Часовой пояс клиента. Список возможных значений см. в [списке dateTimeTimeZone.](datetimetimezone.md)|
|duration|Длительность|Продолжительность встречи, обозначаемая в [формате ISO8601.](https://www.iso.org/iso-8601-date-and-time-format.html) |
|end|[dateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс, которые заканчивается встреча.|
|filledAttendeesCount|Int32|Текущее число клиентов в записи. |
|id|Строка| ID **bookingAppointment**. Только для чтения.|
|invoiceAmount|Double|Выставленная на счету сумма.|
|invoiceDate|[dateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс счета-фактуры для этого назначения.|
|invoiceId|Строка|ID счета-фактуры.|
|invoiceStatus|строка| Состояние счета. Возможные значения: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.|
|invoiceUrl|Строка|URL-адрес счета в Microsoft Bookings.|
|isLocationOnline|Boolean|True указывает, что встреча будет проходить в Интернете. Значение по умолчанию − ложь.|
|joinWebUrl|Строка|URL-адрес собрания в Интернете для встречи.|
|maximumAttendeesCount|Int32|Максимальное число клиентов, разрешенных при встрече.|
|optOutOfCustomerEmail|Boolean|True указывает, что [bookingCustomer](bookingcustomer.md) для этого назначения не желает получать подтверждение для этого назначения.|
|postBuffer|Длительность|Количество времени, необходимое для резерва после окончания встречи, для очистки в качестве примера. Значение выражается в [формате ISO8601.](https://www.iso.org/iso-8601-date-and-time-format.html) |
|preBuffer|Длительность|Количество времени, необходимое для резерва перед началом встречи, для подготовки в качестве примера. Значение выражается в [формате ISO8601.](https://www.iso.org/iso-8601-date-and-time-format.html)|
|цена|Double|Обычная цена встречи для указанного [bookingService.](bookingservice.md)|
|priceType|bookingPriceType| Параметр, который обеспечивает гибкость структуры ценообразования служб. Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`, `unknownFutureValue`.|
|напоминания|[коллекция bookingReminder](bookingreminder.md)|Коллекция напоминаний клиентов, отправленных для этого назначения. Значение этого свойства доступно только при чтении этого **bookingAppointment** по его ID.|
|selfServiceAppointmentId|Строка|Дополнительный ИД отслеживания для встречи, если назначение было создано непосредственно клиентом на странице планирования, а не сотрудником от имени клиента.|
|serviceId|Строка|ID службы [bookingService,](bookingservice.md) связанной с этим назначением.|
|serviceLocation|[location](location.md)|Расположение, в котором доставляется служба.|
|serviceName|Строка|Имя **bookingService, связанного** с этим назначением.<br>Это свойство является необязательным при создании новой встречи. Если не указано, оно вычисляется из службы, связанной с назначением **свойством serviceId.**|
|serviceNotes|Строка|Заметки [из bookingStaffMember](bookingstaffmember.md). Значение этого свойства доступно только при чтении этого **bookingAppointment** по его ID.|
|smsNotificationsEnabled|Boolean|True указывает, что sms-уведомления будут отправлены клиентам для встречи. Значение по умолчанию − ложь.|
|staffMemberIds|Коллекция строк|ID каждого [бронированияStaffMember,](bookingstaffmember.md) который запланирован в этом назначении.|
|начать|[dateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс, в который начинается встреча.|

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
  "customerEmailAddress": "String",
  "customerId": "String",
  "customerLocation": {"@odata.type": "microsoft.graph.location"},
  "customerName": "String",
  "customerNotes": "String",
  "customerPhone": "String",
  "customerTimeZone": "String",
  "customers": [
    {
      "@odata.type": "microsoft.graph.bookingCustomerInformation"
    }
  ],
  "duration": "String (timestamp)",
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "id": "String (identifier)",
  "invoiceAmount": 1024,
  "invoiceDate": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "invoiceId": "String",
  "invoiceStatus": "string",
  "invoiceUrl": "String",
  "isLocationOnline": "Boolean",
  "joinWebUrl": "String",
  "optOutOfCustomerEmail": true,
  "postBuffer": "String (timestamp)",
  "preBuffer": "String (timestamp)",
  "price": 1024,
  "priceType": {"@odata.type": "microsoft.graph.bookingPriceType"},
  "reminders": [{"@odata.type": "microsoft.graph.bookingReminder"}],
  "selfServiceAppointmentId": "String",
  "serviceId": "String",
  "serviceLocation": {"@odata.type": "microsoft.graph.location"},
  "serviceName": "String",
  "serviceNotes": "String",
  "smsNotificationsEnabled": "Boolean",
  "staffMemberIds": ["String"],
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
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


