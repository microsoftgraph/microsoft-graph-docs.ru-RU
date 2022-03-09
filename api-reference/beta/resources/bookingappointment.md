---
title: тип ресурса bookingAppointment
description: Представляет назначение клиента для bookingService, выполняемого набором сотрудников, предоставляемым бизнесом Microsoft Bookings.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: ac5c39da4a9f6ad0ffc352007f10bc4d2dd68eff
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63367722"
---
# <a name="bookingappointment-resource-type"></a>тип ресурса bookingAppointment

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Представляет назначение клиента для [bookingService](bookingservice.md), выполняемого набором сотрудников, предоставляемым бизнесом Microsoft Bookings.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список встреч](../api/bookingbusiness-list-appointments.md) |  [коллекция bookingAppointment](bookingappointment.md) | Получите список объектов **bookingAppointment** в указанном [bookingbusiness](../resources/bookingbusiness.md). |
|[Создание bookingAppointment](../api/bookingbusiness-post-appointments.md) |  [bookingAppointment](bookingappointment.md) | Создание нового **bookingAppointment** для указанного [bookingbusiness](../resources/bookingbusiness.md). |
|[Получить bookingAppointment](../api/bookingappointment-get.md) | [bookingAppointment](bookingappointment.md) |Ознакомьтесь с свойствами и отношениями **объекта bookingAppointment** .|
|[Обновление](../api/bookingappointment-update.md) | [bookingAppointment](bookingappointment.md)    |Обновление объекта **bookingAppointment** . |
|[удаление](../api/bookingappointment-delete.md); | Нет |Удаление **объекта bookingAppointment** . |
|[Отмена](../api/bookingappointment-cancel.md)|Нет| Отмена **объекта bookingAppointment** .|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|additionalInformation|Строка|Дополнительные сведения, которые отправляются клиенту при подтверждении встречи.|
|customerEmailAddress|Строка|SMTP-адрес [bookingCustomer](bookingcustomer.md) , который бронирует встречу.|
|customerId|String|ID [bookingCustomer](bookingcustomer.md) для этого назначения. Если при назначении не указывается номер, создается новый объект **bookingCustomer** . После набора следует считать **customerId** неуменяемым.|
|customerLocation|[location](location.md)|Представляет сведения о расположении [для bookingCustomer](bookingcustomer.md) , который бронирует встречу.|
|имя клиента|String|Имя клиента.|
|customerNotes|Строка|Заметки от клиента, связанного с этим назначением. Значение можно получить только при чтении этого **bookingAppointment** по его ID. <br> Это свойство можно установить только при первоначальном создании встречи с новым клиентом. После этого значение вычисляется от клиента, представленного **customerId**.|
|customerPhone|Строка|Номер телефона клиента.|
|клиенты|[коллекция bookingCustomerInformation](../resources/bookingcustomerinformation.md)|В нем перечислены свойства клиента для встречи. Встреча будет содержать список сведений о клиентах, и каждое подразделение будет указывать свойства клиента, который является частью этого назначения. Необязательное свойство.|
|customerTimeZone|Строка|Часовой пояс клиента. Список возможных значений см. в [списке dateTimeTimeZone](datetimetimezone.md).|
|duration|Длительность|Продолжительность встречи, обозначаемая в [формате ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|end|[dateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс, которые заканчивается встреча.|
|filledAttendeesCount|Int32|Текущее число клиентов в записи. |
|id|Строка| ID **bookingAppointment**. Только для чтения.|
|invoiceAmount|Double|Выставленная на счету сумма.|
|invoiceDate|[dateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс счета-фактуры для этого назначения.|
|invoiceId|String|ID счета-фактуры.|
|invoiceStatus|Строка| Состояние счета. Возможные значения: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.|
|invoiceUrl|String|URL-адрес счета в Microsoft Bookings.|
|isLocationOnline|Boolean|True указывает, что встреча будет проходить в Интернете. Значение по умолчанию − ложь.|
|joinWebUrl|Строка|URL-адрес собрания в Интернете для встречи.|
|maximumAttendeesCount|Int32|Максимальное число клиентов, разрешенных при встрече. Если **значение maximumAttendeesCount** службы превышает 1, передай действительные удостоверения клиентов при создании или обновлении встречи. Чтобы создать клиента, используйте операцию [Create bookingCustomer](../api/bookingbusiness-post-customers.md) . |
|optOutOfCustomerEmail|Boolean|True указывает, что [bookingCustomer](bookingcustomer.md) для этого назначения не желает получать подтверждение для этого назначения.|
|postBuffer|Длительность|Количество времени, необходимое для резерва после окончания встречи, для очистки в качестве примера. Значение выражается в [формате ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|preBuffer|Длительность|Количество времени, необходимое для резерва перед началом встречи, для подготовки в качестве примера. Значение выражается в [формате ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|цена|Double|Обычная цена встречи для указанного [bookingService](bookingservice.md).|
|priceType|bookingPriceType| Параметр, который обеспечивает гибкость структуры ценообразования служб. Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`, `unknownFutureValue`.|
|напоминания|[коллекция bookingReminder](bookingreminder.md)|Коллекция напоминаний клиентов, отправленных для этого назначения. Значение этого свойства доступно только при чтении этого **bookingAppointment** по его ID.|
|selfServiceAppointmentId|String|Дополнительный ИД отслеживания для встречи, если назначение было создано непосредственно клиентом на странице планирования, а не сотрудником от имени клиента.|
|serviceId|Строка|ID службы [bookingService](bookingservice.md) , связанной с этим назначением.|
|serviceLocation|[location](location.md)|Расположение, в котором доставляется служба.|
|serviceName|Строка|Имя **bookingService, связанного** с этим назначением.<br>Это свойство является необязательным при создании новой встречи. Если не указано, оно вычисляется из службы, связанной с назначением **свойством serviceId** .|
|serviceNotes|String|Заметки [из bookingStaffMember](bookingstaffmember.md). Значение этого свойства доступно только при чтении этого **bookingAppointment** по его ID.|
|smsNotificationsEnabled|Boolean|True указывает, что sms-уведомления будут отправлены клиентам для встречи. Значение по умолчанию − ложь.|
|staffMemberIds|Коллекция String|ID каждого [бронированияStaffMember](bookingstaffmember.md) , который запланирован в этом назначении.|
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


