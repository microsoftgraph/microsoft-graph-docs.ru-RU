---
title: Тип ресурса Букингаппоинтмент
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: f08b33cd223a140373f6130f19099ce0c941d8b9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442194"
---
# <a name="bookingappointment-resource-type"></a>Тип ресурса Букингаппоинтмент

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Представляет встречу клиента для [букингсервице](bookingservice.md), выполняемой набором сотрудников, предоставляемых корпорацией Майкрософт для бизнеса.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список встреч](../api/bookingbusiness-list-appointments.md) |  Коллекция [букингаппоинтмент](bookingappointment.md) | Получение списка объектов **букингаппоинтмент** в указанном [букингбусинесс](../resources/bookingbusiness.md). |
|[Создание Букингаппоинтмент](../api/bookingbusiness-post-appointments.md) |  [bookingAppointment](bookingappointment.md) | Создание нового **букингаппоинтмент** для указанного [букингбусинесс](../resources/bookingbusiness.md). |
|[Получение Букингаппоинтмент](../api/bookingappointment-get.md) | [bookingAppointment](bookingappointment.md) |Чтение свойств и связей объекта **букингаппоинтмент** .|
|[обновление](../api/bookingappointment-update.md). | [bookingAppointment](bookingappointment.md)    |Обновление объекта **букингаппоинтмент** . |
|[удаление](../api/bookingappointment-delete.md); | Нет |Удаление объекта **букингаппоинтмент** . |
|[Отмена](../api/bookingappointment-cancel.md)|Нет| Отмена объекта **букингаппоинтмент** .|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|кустомеремаиладдресс|String|SMTP-адрес [букингкустомер](bookingcustomer.md) , который зарезервировано встречу.|
|customerId|String|Идентификатор [букингкустомер](bookingcustomer.md) для этой встречи. Если при создании встречи не указан идентификатор, создается новый объект **букингкустомер** . После установки необходимо учесть неизменность **customerId** .|
|кустомерлокатион|[location](location.md)|Представляет сведения о расположении для [букингкустомер](bookingcustomer.md) , который зарезервировано встречу.|
|customerName|String|Имя клиента.|
|кустомернотес|String|Примечания от клиента, связанного с этой встречей. Значение можно получить только при чтении этого **букингаппоинтмент** по его идентификатору. <br> Это свойство можно задать только при первоначальном создании встречи с новым клиентом. После этой точки значение вычисляется от клиента, представленного **customerId**.|
|кустомерфоне|String|Номер телефона клиента.|
|duration|Длительность|Длительность встречи, обозначенная в формате [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|end|[dateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс, в котором заканчивается встреча.|
|id|String| Идентификатор **букингаппоинтмент**. Только для чтения.|
|инвоицеамаунт|Двойное с плавающей точкой|Сумма счета в счете.|
|инвоицедате|[dateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс накладной для данной встречи.|
|инвоицеид|String|Идентификатор счета.|
|инвоицестатус|string| Статус счета. Возможные значения: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.|
|инвоицеурл|String|URL-адрес счета в книгах корпорации Майкрософт.|
|оптаутофкустомеремаил|Логическое|Значение true указывает, что [букингкустомер](bookingcustomer.md) для этой встречи не хочет получать подтверждение для этой встречи.|
|Буфер буфера|Длительность|Количество времени, которое необходимо зарезервировать после окончания встречи, для очистки в качестве примера. Значение выражается в формате [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|пребуфер|Длительность|Количество времени, которое необходимо зарезервировать до начала встречи, в качестве примера для подготовки. Значение выражается в формате [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|Цена|Двойное с плавающей точкой|Обычная цена для встречи с указанным [букингсервице](bookingservice.md).|
|прицетипе|string| Параметр, обеспечивающий гибкость для структуры ценообразования служб. Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.|
|напоминания|Коллекция [букингреминдер](bookingreminder.md)|Коллекция напоминаний о клиентах, отправленных для этой встречи. Значение этого свойства доступно только при чтении этого **букингаппоинтмент** с помощью идентификатора.|
|селфсервицеаппоинтментид|String|Дополнительный идентификатор отслеживания для встречи, если встреча создана непосредственно клиентом на странице планирования, в отличие от сотрудника от имени клиента;.|
|serviceId|String|Идентификатор [букингсервице](bookingservice.md) , связанный с этой встречей.|
|сервицелокатион|[location](location.md)|Место доставки службы.|
|Служба|String|Имя **букингсервице** , связанного с этой встречей.<br>Это свойство является необязательным при создании новой встречи. Если он не указан, то он вычисляется из службы, связанной с встречей, с помощью свойства **serviceId** .|
|сервиценотес|String|Заметки из [букингстаффмембер](bookingstaffmember.md). Значение этого свойства доступно только при чтении этого **букингаппоинтмент** с помощью идентификатора.|
|стаффмемберидс|Коллекция String|Идентификатор каждого [букингстаффмембер](bookingstaffmember.md) , запланированного в этой встрече.|
|начать|[dateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс, с которого начинается встреча.|

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
