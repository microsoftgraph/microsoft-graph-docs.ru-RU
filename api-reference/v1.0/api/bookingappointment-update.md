---
title: Обновление bookingAppointment
description: Обновите свойства объекта bookingAppointment в указанном bookingBusiness.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 429d6331bdff07c7e3c8010b6801725c42f8efc4
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856073"
---
# <a name="update-bookingappointment"></a>Обновление bookingAppointment

Пространство имен: microsoft.graph

Обновите свойства объекта [bookingAppointment](../resources/bookingappointment.md) в указанном [bookingBusiness](../resources/bookingbusiness.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All   |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.   |
|Приложение | BookingsAppointment.ReadWrite.All, Bookings.Read.All  |

> [!NOTE]
> При создании пользовательского приложения с использованием разрешений приложения необходимо выполнить проверку [бизнес-правил](/graph/bookingsbusiness-business-rules).

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /solutions/bookingBusinesses/{id}/appointments/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:-----------|:-----------|
| Авторизация  | Носитель {code}. Обязательно.|

## <a name="request-body"></a>Текст запроса

[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Клиентов|[Коллекция bookingCustomerInformation](../resources/bookingcustomerinformation.md)|В нем перечислены свойства клиента для встречи. Встреча будет содержать список сведений о клиенте, и каждое подразделение будет указывать свойства клиента, который является частью этой встречи. Необязательный элемент.|
|customerTimeZone|Строка|Часовой пояс клиента. Список возможных значений см. в [разделе dateTimeTimeZone](../resources/datetimetimezone.md).|
|duration|Длительность|Длина встречи, помеченная в [формате ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|endDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата, время и часовой пояс, на которых заканчивается встреча.|
|filledAttendeesCount|Int32|Текущее число клиентов во встрече. Обязательный.|
|isLocationOnline|Логический|Если `true`указывает, что встреча будет храниться в сети. Значение по умолчанию − ложь.|
|maximumAttendeesCount|Int32|Максимальное число клиентов, разрешенных во время встречи. Обязательный. |
|optOutOfCustomerEmail|Логический|Если `true`указывает, что [bookingCustomer](../resources/bookingcustomer.md) для этой встречи не хочет получать подтверждение для этой встречи.|
|postBuffer|Длительность|Например, время резервирования после окончания встречи для очистки. Значение выражается в [формате ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|preBuffer|Длительность|Количество времени, зарезервируемого до начала встречи, для подготовки, в качестве примера. Значение выражается в [формате ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|Цена|Двойное с плавающей точкой|Обычная цена встречи для указанной [службы bookingService](../resources/bookingservice.md).|
|priceType|bookingPriceType| Параметр, предоставляющий гибкость для структуры ценообразования служб. Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`, `unknownFutureValue`.|
|Напоминания|[Коллекция bookingReminder](../resources/bookingreminder.md)|Коллекция напоминаний клиентов, отправленных для этой встречи. Значение этого свойства доступно только при чтении **этого объекта bookingAppointment** по его идентификатору.|
|selfServiceAppointmentId|Строка|Дополнительный идентификатор отслеживания для встречи, если встреча была создана непосредственно клиентом на странице планирования, а не сотрудником от имени клиента. Поддерживается только для встречи, если maxAttendeeCount имеет значение 1.|
|serviceId|Строка|Идентификатор службы [bookingService](../resources/bookingservice.md) , связанной с этой встречей.|
|serviceLocation|[location](../resources/location.md)|Расположение, куда доставляется служба.|
|serviceName|Строка|Имя службы **bookingService,** связанной с этой встречей.<br>Это свойство является необязательным при создании новой встречи. Если значение не указано, оно вычисляется из службы, связанной с встречей, с помощью **свойства serviceId** .|
|serviceNotes|Строка|Заметки из [bookingStaffMember](../resources/bookingstaffmember.md). Значение этого свойства доступно только при чтении **этого объекта bookingAppointment** по его идентификатору.|
|smsNotificationsEnabled|Логический|Если `true`указано, что для встречи клиентам будут отправляться SMS-уведомления. Значение по умолчанию − ложь.|
|staffMemberIds|Коллекция строк|Идентификатор каждого объекта [bookingStaffMember](../resources/bookingstaffmember.md) , который запланирован на эту встречу.|
|startDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата, время и часовой пояс, с которых начинается встреча.|

> [!NOTE]
> Если максимальное число клиентов (**maximumAttedeesCount**), разрешенное в службе, больше 1:[](../resources/bookingservice.md)
> - Убедитесь, что клиенты существуют в календаре резервирования. Если это не так, создайте его с помощью [операции Create bookingCustomer](bookingbusiness-post-customers.md) .
> - Передайте действительные идентификаторы клиентов при создании или обновлении встречи. Если недопустимый идентификатор клиента, он не будет включен в объект встречи.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. Он не возвращает ничего в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

В следующем примере дата обслуживания изменяется на день.

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