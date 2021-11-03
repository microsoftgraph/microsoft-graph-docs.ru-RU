---
title: тип ресурса bookingAppointment
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 7ecd369607f260c8ebfd456ab7accaa0394e0af0
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696968"
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
|[Удаление](../api/bookingappointment-delete.md) | Нет |Удаление **объекта bookingAppointment.** |
|[Отмена](../api/bookingappointment-cancel.md)|Нет| Отмена **объекта bookingAppointment.**|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|customerEmailAddress|String|SMTP-адрес [bookingCustomer,](bookingcustomer.md) который бронирует встречу.|
|customerId|String|ID [bookingCustomer](bookingcustomer.md) для этого назначения. Если при назначении не указывается номер, создается новый объект **bookingCustomer.** После набора следует считать **customerId** неуменяемым.|
|customerLocation|[location](location.md)|Представляет сведения о расположении [для bookingCustomer,](bookingcustomer.md) который бронирует встречу.|
|имя клиента|String|Имя клиента.|
|customerNotes|String|Заметки от клиента, связанного с этим назначением. Значение можно получить только при чтении этого **bookingAppointment** по его ID. <br> Это свойство можно установить только при первоначальном создании встречи с новым клиентом. После этого значение вычисляется от клиента, представленного **customerId.**|
|customerPhone|String|Номер телефона клиента.|
|customerTimeZone|String|Часовой пояс клиента. Список возможных значений см. в [списке dateTimeTimeZone.](datetimetimezone.md)|
|duration|Длительность|Продолжительность встречи, обозначаемая в [формате ISO8601.](https://www.iso.org/iso-8601-date-and-time-format.html) |
|end|[dateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс, которые заканчивается встреча.|
|id|String| ID **bookingAppointment**. Только для чтения.|
|invoiceAmount|Double|Выставленная на счету сумма.|
|invoiceDate|[dateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс счета-фактуры для этого назначения.|
|invoiceId|String|ID счета-фактуры.|
|invoiceStatus|string| Состояние счета. Возможные значения: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.|
|invoiceUrl|String|URL-адрес счета в Microsoft Bookings.|
|isLocationOnline|Логический|True указывает, что встреча будет проходить в Интернете. Значение по умолчанию − ложь.|
|joinWebUrl|String|URL-адрес собрания в Интернете для встречи.|
|optOutOfCustomerEmail|Логический|True указывает, что [bookingCustomer](bookingcustomer.md) для этого назначения не желает получать подтверждение для этого назначения.|
|postBuffer|Длительность|Количество времени, необходимое для резерва после окончания встречи, для очистки в качестве примера. Значение выражается в [формате ISO8601.](https://www.iso.org/iso-8601-date-and-time-format.html) |
|preBuffer|Длительность|Количество времени, необходимое для резерва перед началом встречи, для подготовки в качестве примера. Значение выражается в [формате ISO8601.](https://www.iso.org/iso-8601-date-and-time-format.html)|
|цена|Double|Обычная цена встречи для указанного [bookingService.](bookingservice.md)|
|priceType|string| Параметр, который обеспечивает гибкость структуры ценообразования служб. Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.|
|напоминания|[коллекция bookingReminder](bookingreminder.md)|Коллекция напоминаний клиентов, отправленных для этого назначения. Значение этого свойства доступно только при чтении этого **bookingAppointment** по его ID.|
|selfServiceAppointmentId|String|Дополнительный ИД отслеживания для встречи, если назначение было создано непосредственно клиентом на странице планирования, а не сотрудником от имени клиента.|
|serviceId|Строка|ID службы [bookingService,](bookingservice.md) связанной с этим назначением.|
|serviceLocation|[location](location.md)|Расположение, в котором доставляется служба.|
|serviceName|String|Имя **bookingService, связанного** с этим назначением.<br>Это свойство является необязательным при создании новой встречи. Если не указано, оно вычисляется из службы, связанной с назначением **свойством serviceId.**|
|serviceNotes|String|Заметки [из bookingStaffMember](bookingstaffmember.md). Значение этого свойства доступно только при чтении этого **bookingAppointment** по его ID.|
|smsNotificationsEnabled|Логический|True указывает, что sms-уведомления будут отправлены клиентам для встречи. Значение по умолчанию − ложь.|
|staffMemberIds|Коллекция строк|ID каждого [бронированияStaffMember,](bookingstaffmember.md) который запланирован в этом назначении.|
|начать|[dateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс, в который начинается встреча.|

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
  "customerTimeZone": "String",
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
  "priceType": "string",
  "reminders": [{"@odata.type": "microsoft.graph.bookingReminder"}],
  "selfServiceAppointmentId": "String",
  "serviceId": "String",
  "serviceLocation": {"@odata.type": "microsoft.graph.location"},
  "serviceName": "String",
  "serviceNotes": "String",
  "smsNotificationsEnabled": "Boolean",
  "staffMemberIds": ["String"],
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
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


