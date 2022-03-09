---
title: Обновление bookingAppointment
description: Обновление свойств объекта bookingAppointment в указанном bookingBusiness.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: d1b2e9863f8cc98cd2d17b9867817bb804dc3217
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63367974"
---
# <a name="update-bookingappointment"></a>Обновление bookingAppointment

Пространство имен: microsoft.graph

Обновление свойств объекта [bookingAppointment](../resources/bookingappointment.md) в указанном [bookingBusiness](../resources/bookingbusiness.md).
## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All   |
|Делегированное (личная учетная запись Майкрософт) | Не поддерживается.   |
|Для приложений | Не поддерживается.  |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /solutions/bookingBusinesses/{id}/appointments/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:-----------|:-----------|
| Авторизация  | Bearer {код}. Обязательно.|

## <a name="request-body"></a>Текст запроса

[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|клиенты|[коллекция bookingCustomerInformation](../resources/bookingcustomerinformation.md)|В нем перечислены свойства клиента для встречи. Встреча будет содержать список сведений о клиентах, и каждое подразделение будет указывать свойства клиента, который является частью этого назначения. Необязательное свойство.|
|customerTimeZone|String|Часовой пояс клиента. Список возможных значений см. в [списке dateTimeTimeZone](../resources/datetimetimezone.md).|
|duration|Длительность|Продолжительность встречи, обозначаемая в [формате ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|endDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата, время и часовой пояс, которые заканчивается встреча.|
|filledAttendeesCount|Int32|Текущее число клиентов в записи. Обязательный элемент.|
|isLocationOnline|Boolean|Если `true`, указывает, что встреча будет проходить в Интернете. Значение по умолчанию − ложь.|
|maximumAttendeesCount|Int32|Максимальное количество клиентов, разрешенных при встрече. Обязательный элемент. |
|optOutOfCustomerEmail|Boolean|Если `true`, указывает, что [bookingCustomer](../resources/bookingcustomer.md) для этого назначения не желает получать подтверждение для этого назначения.|
|postBuffer|Длительность|Количество времени, необходимое для резерва после окончания встречи, для очистки в качестве примера. Значение выражается в [формате ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|preBuffer|Длительность|Количество времени, необходимое для резерва перед началом встречи, для подготовки в качестве примера. Значение выражается в [формате ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|цена|Double|Обычная цена встречи для указанного [bookingService](../resources/bookingservice.md).|
|priceType|bookingPriceType| Параметр, который обеспечивает гибкость структуры ценообразования служб. Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`, `unknownFutureValue`.|
|напоминания|[коллекция bookingReminder](../resources/bookingreminder.md)|Коллекция напоминаний клиентов, отправленных для этого назначения. Значение этого свойства доступно только при чтении этого **bookingAppointment** по его ID.|
|selfServiceAppointmentId|Строка|Дополнительный ИД отслеживания для встречи, если назначение было создано непосредственно клиентом на странице планирования, а не сотрудником от имени клиента. Поддерживается только при назначении, если maxAttendeeCount — 1.|
|serviceId|Строка|ID службы [bookingService](../resources/bookingservice.md) , связанной с этим назначением.|
|serviceLocation|[location](../resources/location.md)|Расположение, в котором доставляется служба.|
|serviceName|Строка|Имя **bookingService, связанного** с этим назначением.<br>Это свойство является необязательным при создании новой встречи. Если не указано, оно вычисляется из службы, связанной с назначением **свойством serviceId** .|
|serviceNotes|String|Заметки [из bookingStaffMember](../resources/bookingstaffmember.md). Значение этого свойства доступно только при чтении этого **bookingAppointment** по его ID.|
|smsNotificationsEnabled|Boolean|Если `true`, указывает SMS-уведомления будут отправлены клиентам для встречи. Значение по умолчанию − ложь.|
|staffMemberIds|Коллекция String|ID каждого [бронированияStaffMember](../resources/bookingstaffmember.md) , который запланирован в этом назначении.|
|startDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата, время и часовой пояс, в который начинается встреча.|

> [!NOTE]
> Если максимальное число клиентов (**maximumAttedeesCount**), разрешенных в службе, превышает 1:[](../resources/bookingservice.md)
> - Убедитесь, что клиенты существуют в календаре бронирования. Если этого не сделать, создайте с помощью операции [Create bookingCustomer](bookingbusiness-post-customers.md) .
> - Передай действительные удостоверения клиентов при создании или обновлении встречи. Если удостоверение клиента не допустимо, этот клиент не будет включен в объект назначения.

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
В следующем примере дата службы изменяется на день.

<!-- {
  "blockType": "request"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/solutions/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/appointments/AAMkADKnAAA=
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingAppointment",
    "endDateTime":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:30:00.0000000+00:00",
        "timeZone":"UTC"
    },
    "startDateTime":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:00:00.0000000+00:00",
        "timeZone":"UTC"
    }
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingappointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


