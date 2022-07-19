---
title: Тип ресурса bookingAppointment
description: Представляет встречу клиента для bookingService, выполняемую набором сотрудников, предоставляемых Microsoft Bookings компании.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 20b466b734ef0f91445e950e3bfee173758e4b0d
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856318"
---
# <a name="bookingappointment-resource-type"></a>Тип ресурса bookingAppointment

Пространство имен: microsoft.graph
 
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
|[удаление](../api/bookingappointment-delete.md); | Нет |Удаление объекта **bookingAppointment** . |
|[Отмена](../api/bookingappointment-cancel.md)|Нет| Отмена **объекта bookingAppointment** .|

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|additionalInformation|Строка|Дополнительные сведения, отправляемые клиенту при подтверждении встречи.|
|Клиентов|[Коллекция bookingCustomerInformation](bookingcustomerinformation.md)|В нем перечислены свойства клиента для встречи. Встреча будет содержать список сведений о клиенте, и каждое подразделение будет указывать свойства клиента, который является частью этой встречи. Необязательный элемент.|
|customerTimeZone|Строка|Часовой пояс клиента. Список возможных значений см. в [разделе dateTimeTimeZone](datetimetimezone.md).|
|duration|Длительность|Длина встречи, помеченная в [формате ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|endDateTime|[dateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс, на которых заканчивается встреча.|
|filledAttendeesCount|Int32|Текущее число клиентов во время встречи |
|id|String| Идентификатор объекта **bookingAppointment**. Только для чтения.|
|isLocationOnline|Логический|Если `true`указывает, что встреча будет храниться в сети. Значение по умолчанию — `false`.|
|joinWebUrl|Строка|URL-адрес собрания по сети для встречи.|
|maximumAttendeesCount|Int32|Максимальное число клиентов, разрешенных во время встречи. Если **значение maximumAttendeesCount** службы больше 1, передайте допустимые идентификаторы клиентов при создании или обновлении встречи. Чтобы создать клиента, используйте операцию [Create bookingCustomer](../api/bookingbusiness-post-customers.md) . |
|optOutOfCustomerEmail|Логический|Если `true` указано, что [bookingCustomer](bookingcustomer.md) для этой встречи не хочет получать подтверждение для этой встречи.|
|postBuffer|Длительность|Например, время резервирования после окончания встречи для очистки. Значение выражается в [формате ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|preBuffer|Длительность|Количество времени, зарезервируемого до начала встречи, для подготовки, в качестве примера. Значение выражается в [формате ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|Цена|Двойное с плавающей точкой|Обычная цена встречи для указанной [службы bookingService](bookingservice.md).|
|priceType|bookingPriceType| Параметр, предоставляющий гибкость для структуры ценообразования служб. Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`, `unknownFutureValue`.|
|Напоминания|[Коллекция bookingReminder](bookingreminder.md)|Коллекция напоминаний клиентов, отправленных для этой встречи. Значение этого свойства доступно только при чтении **этого объекта bookingAppointment** по его идентификатору.|
|selfServiceAppointmentId|String|Дополнительный идентификатор отслеживания встречи, если встреча была создана непосредственно клиентом на странице планирования, а не сотрудником от имени клиента. Поддерживается только для встречи, если maxAttendeeCount имеет значение 1.|
|serviceId|Строка|Идентификатор службы [bookingService](bookingservice.md) , связанной с этой встречей.|
|serviceLocation|[location](location.md)|Расположение, куда доставляется служба.|
|serviceName|Строка|Имя службы **bookingService,** связанной с этой встречей.<br>Это свойство является необязательным при создании новой встречи. Если значение не указано, оно вычисляется из службы, связанной с встречей, с помощью **свойства serviceId** .|
|serviceNotes|Строка|Заметки из [bookingStaffMember](bookingstaffmember.md). Значение этого свойства доступно только при чтении **этого объекта bookingAppointment** по его идентификатору.|
|smsNotificationsEnabled|Логический|Если `true`указано, что для встречи клиентам будут отправляться SMS-уведомления. Значение по умолчанию — `false`.|
|staffMemberIds|Коллекция строк|Идентификатор каждого объекта [bookingStaffMember](bookingstaffmember.md) , который запланирован на эту встречу.|
|startDateTime|[dateTimeTimeZone](datetimetimezone.md)|Дата, время и часовой пояс, с которых начинается встреча.|

## <a name="relationships"></a>Связи

Отсутствуют.

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