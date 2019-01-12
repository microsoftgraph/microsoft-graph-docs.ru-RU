---
title: Тип ресурса bookingAppointment
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 0314c8a4d451625c2ee1df332c342c1871a098ad
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934095"
---
# <a name="bookingappointment-resource-type"></a>Тип ресурса bookingAppointment

 > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.
 
Представляет встречи клиента для [bookingService](bookingservice.md), выполняется с помощью набора персонала члены, предоставляемые резервирования Microsoft business.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список встреч](../api/bookingbusiness-list-appointments.md) |  [bookingAppointment](bookingappointment.md) коллекции | Получите список объектов **bookingAppointment** в указанном [bookingbusiness](../resources/bookingbusiness.md). |
|[Создание bookingAppointment](../api/bookingbusiness-post-appointments.md) |  [bookingAppointment](bookingappointment.md) | Создание нового **bookingAppointment** для указанного [bookingbusiness](../resources/bookingbusiness.md). |
|[Получение bookingAppointment](../api/bookingappointment-get.md) | [bookingAppointment](bookingappointment.md) |Чтение свойства и связи объекта **bookingAppointment** .|
|[обновление](../api/bookingappointment-update.md). | [bookingAppointment](bookingappointment.md)    |Обновление объекта **bookingAppointment** . |
|[Delete](../api/bookingappointment-delete.md) | Нет |Удалите объект **bookingAppointment** . |
|[Отмена](../api/bookingappointment-cancel.md)|Нет| Отмена **bookingAppointment** объекта.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|customerEmailAddress|Строка|SMTP-адрес [bookingCustomer](bookingcustomer.md) , кто резервирования встречи.|
|customerId|Строка|Идентификатор [bookingCustomer](bookingcustomer.md) для этой встречи. Если идентификатор не указан при создании встречи, будет создан новый объект **bookingCustomer** . После установки необходимо учитывать **customerId** неизменными.|
|customerLocation|[location](location.md)|Представляет сведения о расположении для [bookingCustomer](bookingcustomer.md) кто резервирования встречи.|
|customerName|Строка|Имя клиента.|
|customerNotes|Строка|Примечания из клиента, связанного с этой встречи. Можно получить значение только при чтении этой **bookingAppointment** по идентификатору. <br> Это свойство можно задать только в том случае, когда изначально Создание встречи с помощью нового клиента. После этого значение вычисляется от клиента, представленного **customerId**.|
|customerPhone|Строка|Номера телефона.|
|duration|Продолжительность|Длина встречи, идентификаторами в формате [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|end|[dateTimeTimeZone](datetimetimezone.md)|Даты, времени и часового пояса окончания встречи.|
|id|Строка| Идентификатор **bookingAppointment**. Только для чтения.|
|invoiceAmount|Double|Сумма по документу на счет.|
|invoiceDate|[dateTimeTimeZone](datetimetimezone.md)|Даты, времени и часового пояса для создания счетов-фактур для этой встречи.|
|invoiceId|Строка|ID счета.|
|invoiceStatus|string| Состояние создания счетов-фактур. Возможные значения: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.|
|invoiceUrl|Строка|URL-адрес создания счетов-фактур в Microsoft резервирования.|
|optOutOfCustomerEmail|Логический|Значение true означает, что [bookingCustomer](bookingcustomer.md) для этой встречи не хотите получать подтверждения для этой встречи.|
|postBuffer|Продолжительность|Период времени для резервирования после окончания встречи, очистка, в качестве примера. Значение задается в формате [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|пребуфер|Продолжительность|Период времени для резервирования до начала встречи, для подготовки, в качестве примера. Значение задается в формате [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|цены|Double|Цены для встречи для указанного [bookingService](bookingservice.md).|
|priceType|string| Параметр для обеспечения гибкости при цен структура служб. Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.|
|напоминания|[bookingReminder](bookingreminder.md) коллекции|Коллекция клиента напоминаний, отправляемых для этой встречи. Значение этого свойства доступна только при чтении этой **bookingAppointment** по идентификатору.|
|selfServiceAppointmentId|Строка|Идентификатор дополнительные отслеживания для встречи, если встречи был создан непосредственно с клиента на странице расписания, в отличие от сотрудником от имени клиента.|
|serviceId|Строка|Идентификатор [bookingService](bookingservice.md) , связанный с этой встречи.|
|serviceLocation|[location](location.md)|Расположение, где доставляется службу.|
|имя_службы|Строка|Имя **bookingService** , связанный с этой встречи.<br>Это свойство является необязательным при создании новой встречи. Если не указано, вычисляется из службы, связанной с встречи в свойстве **serviceId** .|
|serviceNotes|Строка|Примечания из [bookingStaffMember](bookingstaffmember.md). Значение этого свойства доступна только при чтении этой **bookingAppointment** по идентификатору.|
|staffMemberIds|Коллекция String|Идентификатор каждого [bookingStaffMember](bookingstaffmember.md) пользователей, которые планируется во встрече.|
|start|[dateTimeTimeZone](datetimetimezone.md)|Даты, времени и часового пояса начала встречи.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

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
  "duration": "String (timestamp)",
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "id": "String (identifier)",
  "invoiceAmount": 1024,
  "invoiceDate": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "invoiceId": "String",
  "invoiceStatus": "string",
  "invoiceUrl": "String",
  "optOutOfCustomerEmail": true,
  "postBuffer": "String (timestamp)",
  "preBuffer": "String (timestamp)",
  "price": 1024,
  "priceType": "string",
  "reminders": [{"@odata.type": "microsoft.graph.bookingReminder"}],
  "selfServiceAppointmentId": "String",
  "serviceId": "String",
  "serviceLocation": {"@odata.type": "microsoft.graph.location"},
  "serviceName": "String",
  "serviceNotes": "String",
  "staffMemberIds": ["String"],
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingAppointment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
