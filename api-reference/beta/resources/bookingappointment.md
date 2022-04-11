---
title: Тип ресурса bookingAppointment
description: Представляет встречу клиента для bookingService, выполняемую набором сотрудников, предоставляемых Microsoft Bookings компании.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: c3fb44ea22819728d5d048dd0c41daed4e20cef3
ms.sourcegitcommit: 19558bd9de9b717e7a36bfce1d6d84d0132e2697
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2022
ms.locfileid: "64755700"
---
# <a name="bookingappointment-resource-type"></a>Тип ресурса bookingAppointment

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Представляет встречу клиента для [bookingService](bookingservice.md), выполняемую набором сотрудников, предоставляемых Microsoft Bookings компании.

> [!NOTE]
> При создании пользовательского приложения с использованием разрешений приложения необходимо выполнить проверку [бизнес-правил](/graph/bookingsbusiness-business-rules).

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список встреч](../api/bookingbusiness-list-appointments.md) |  [Коллекция bookingAppointment](bookingappointment.md) | Получение списка объектов **bookingAppointment** в указанном [bookingbusiness](bookingbusiness.md). |
|[Создание bookingAppointment](../api/bookingbusiness-post-appointments.md) |  [bookingAppointment](bookingappointment.md) | Создайте **новое bookingAppointment** для указанного [bookingbusiness](bookingbusiness.md). |
|[Получение bookingAppointment](../api/bookingappointment-get.md) | [bookingAppointment](bookingappointment.md) |Чтение свойств и связей объекта **bookingAppointment** .|
|[Обновление](../api/bookingappointment-update.md) | [bookingAppointment](bookingappointment.md)    |Обновление объекта **bookingAppointment** . |
|[Удаление](../api/bookingappointment-delete.md) | Нет |Удаление объекта **bookingAppointment** . |
|[Cancel](../api/bookingappointment-cancel.md)|Нет| Отмена **объекта bookingAppointment** .|

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|additionalInformation|String|Дополнительные сведения, отправляемые клиенту при подтверждении встречи.|
|customerEmailAddress|String|SMTP-адрес [bookingCustomer](bookingcustomer.md) , который резервировать встречу.|
|customerId|String|Идентификатор объекта [bookingCustomer](bookingcustomer.md) для этой встречи. Если при создании встречи не указан идентификатор, создается новый объект **bookingCustomer** . После установки идентификатор **клиента** следует считать неизменяемым.|
|customerLocation|[location](location.md)|Представляет сведения о расположении [для bookingCustomer](bookingcustomer.md) , который резервирует встречу.|
|customerName|String|Имя клиента.|
|customerNotes|String|Заметки от клиента, связанного с этой встречей. Значение можно получить только при чтении **этого объекта bookingAppointment** по его идентификатору. <br> Это свойство можно задать только при первоначальном создании встречи с новым клиентом. По истечении этого момента значение вычисляется из клиента, представленного **идентификатором клиента**.|
|customerPhone|String|Номер телефона клиента.|
|Клиентов|[Коллекция bookingCustomerInformation](bookingcustomerinformation.md)|В нем перечислены свойства клиента для встречи. Встреча будет содержать список сведений о клиенте, и каждое подразделение будет указывать свойства клиента, который является частью этой встречи. Необязательное свойство.|
|customerTimeZone|String|Часовой пояс клиента. Список возможных значений см. в [разделе dateTimeTimeZone](datetimetimezone.md).|
|duration|Длительность|Длина встречи, помеченная в [формате ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|end|[dateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс, на которых заканчивается встреча.|
|filledAttendeesCount|Int32|Текущее число клиентов во встрече. |
|id|String| Идентификатор объекта **bookingAppointment**. Только для чтения.|
|invoiceAmount|Двойное с плавающей точкой|Сумма, выставленная в счете.|
|invoiceDate|[dateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс счета для этой встречи.|
|invoiceId|String|Идентификатор счета.|
|invoiceStatus|string| Состояние счета. Возможные значения: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.|
|invoiceUrl|String|URL-адрес счета в Microsoft Bookings.|
|isLocationOnline|Логическое|Значение true указывает, что встреча будет храниться в сети. Значение по умолчанию − ложь.|
|joinWebUrl|String|URL-адрес собрания по сети для встречи.|
|maximumAttendeesCount|Int32|Максимальное число клиентов, разрешенных во время встречи. Если **значение maximumAttendeesCount** службы больше 1, передайте допустимые идентификаторы клиентов при создании или обновлении встречи. Чтобы создать клиента, используйте операцию [Create bookingCustomer](../api/bookingbusiness-post-customers.md) . |
|optOutOfCustomerEmail|Логическое|Значение true указывает, [что bookingCustomer](bookingcustomer.md) для этой встречи не хочет получать подтверждение для этой встречи.|
|postBuffer|Длительность|Например, время резервирования после окончания встречи для очистки. Значение выражается в [формате ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|preBuffer|Длительность|Количество времени, зарезервируемого до начала встречи, для подготовки, в качестве примера. Значение выражается в [формате ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|Цена|Двойное с плавающей точкой|Обычная цена встречи для указанной [службы bookingService](bookingservice.md).|
|priceType|bookingPriceType| Параметр, предоставляющий гибкость для структуры ценообразования служб. Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`, `unknownFutureValue`.|
|Напоминания|[Коллекция bookingReminder](bookingreminder.md)|Коллекция напоминаний клиентов, отправленных для этой встречи. Значение этого свойства доступно только при чтении **этого объекта bookingAppointment** по его идентификатору.|
|selfServiceAppointmentId|String|Дополнительный идентификатор отслеживания встречи, если встреча была создана непосредственно клиентом на странице планирования, а не сотрудником от имени клиента.|
|serviceId|Строка|Идентификатор службы [bookingService](bookingservice.md) , связанной с этой встречей.|
|serviceLocation|[location](location.md)|Расположение, куда доставляется служба.|
|serviceName|String|Имя службы **bookingService,** связанной с этой встречей.<br>Это свойство является необязательным при создании новой встречи. Если значение не указано, оно вычисляется из службы, связанной с встречей, с помощью **свойства serviceId** .|
|serviceNotes|String|Заметки из [bookingStaffMember](bookingstaffmember.md). Значение этого свойства доступно только при чтении **этого объекта bookingAppointment** по его идентификатору.|
|smsNotificationsEnabled|Boolean|Значение true указывает, что для встречи клиентам будут отправляться SMS-уведомления. Значение по умолчанию − ложь.|
|staffMemberIds|Коллекция String|Идентификатор каждого объекта [bookingStaffMember](bookingstaffmember.md) , который запланирован на эту встречу.|
|начать|[dateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс, с которых начинается встреча.|

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


