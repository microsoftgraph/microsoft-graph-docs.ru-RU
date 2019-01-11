---
title: Обновление bookingappointment
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: baedaf0e894dfdda96c43ff9dc0cb47ce796db9e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809683"
---
# <a name="update-bookingappointment"></a>Обновление bookingappointment

 > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.
 
Обновление свойства объекта [bookingAppointment](../resources/bookingappointment.md) в указанном [bookingbusiness](../resources/bookingbusiness.md).
## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All   |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.   |
|Для приложений | Не поддерживается.  |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/appointments/{id}
```
## <a name="optional-request-headers"></a>Необязательные заголовки запросов
| Имя       | Описание|
|:-----------|:-----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>Тело запроса
В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|customerEmailAddress|Строка|SMTP-адрес [bookingCustomer](../resources/bookingcustomer.md) , кто резервирования встречи.|
|customerId|Строка|Идентификатор [bookingCustomer](../resources/bookingcustomer.md) для этой встречи. Если идентификатор не указан при создании встречи, будет создан новый объект **bookingCustomer** . После установки необходимо учитывать **customerId** неизменными.|
|customerLocation|[location](../resources/location.md)|Представляет сведения о расположении для [bookingCustomer](../resources/bookingcustomer.md) кто резервирования встречи.|
|customerName|Строка|Имя клиента.|
|customerNotes|Строка|Примечания из клиента, связанного с этой встречи. Можно получить значение только при чтении этой **bookingAppointment** по идентификатору. <br> Это свойство можно задать только в том случае, когда изначально Создание встречи с помощью нового клиента. После этого значение вычисляется от клиента, представленного **customerId**.|
|customerPhone|Строка|Номера телефона.|
|duration|Продолжительность|Длина встречи, идентификаторами в формате [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|end|[dateTimeTimeZone](../resources/datetimetimezone.md)|Даты, времени и часового пояса окончания встречи.|
|invoiceAmount|Double|Сумма по документу на счет.|
|invoiceDate|[dateTimeTimeZone](../resources/datetimetimezone.md)|Даты, времени и часового пояса для создания счетов-фактур для этой встречи.|
|invoiceId|Строка|ID счета.|
|invoiceStatus|string| Состояние создания счетов-фактур. Возможные значения: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.|
|invoiceUrl|Строка|URL-адрес создания счетов-фактур в Microsoft резервирования.|
|optOutOfCustomerEmail|Логический|Значение true означает, что [bookingCustomer](../resources/bookingcustomer.md) для этой встречи не хотите получать подтверждения для этой встречи.|
|postBuffer|Продолжительность|Период времени для резервирования после окончания встречи, очистка, в качестве примера. Значение задается в формате [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|пребуфер|Продолжительность|Период времени для резервирования до начала встречи, для подготовки, в качестве примера. Значение задается в формате [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|цены|Double|Цены для встречи для указанного [bookingService](../resources/bookingservice.md).|
|priceType|string| Параметр для обеспечения гибкости при цен структура служб. Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.|
|напоминания|[bookingReminder](../resources/bookingreminder.md) коллекции|Коллекция клиента напоминаний, отправляемых для этой встречи. Значение этого свойства доступна только при чтении этой **bookingAppointment** по идентификатору.|
|selfServiceAppointmentId|Строка|Идентификатор дополнительные отслеживания для встречи, если встречи был создан непосредственно с клиента на странице расписания, в отличие от сотрудником от имени клиента.|
|serviceId|Строка|Идентификатор [bookingService](../resources/bookingservice.md) , связанный с этой встречи.|
|serviceLocation|[location](../resources/location.md)|Расположение, где доставляется службу.|
|имя_службы|Строка|Имя **bookingService** , связанный с этой встречи.<br>Это свойство является необязательным при создании новой встречи. Если не указано, вычисляется из службы, связанной с встречи в свойстве **serviceId** .|
|serviceNotes|Строка|Примечания из [bookingStaffMember](../resources/bookingstaffmember.md). Значение этого свойства доступна только при чтении этой **bookingAppointment** по идентификатору.|
|staffMemberIds|Коллекция String|Идентификатор каждого [bookingStaffMember](../resources/bookingstaffmember.md) пользователей, которые планируется во встрече.|
|start|[dateTimeTimeZone](../resources/datetimetimezone.md)|Даты, времени и часового пояса начала встречи.|


## <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
В следующем примере изменяется дата обслуживания на один день и обновлены дату создания счетов-фактур.
<!-- {
  "blockType": "request",
  "name": "update_bookingappointment"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKnAAA=
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingAppointment",
    "end":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:30:00.0000000+00:00",
        "timeZone":"UTC"
    },
    "invoiceDate":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:30:00.0000000+00:00",
        "timeZone":"UTC"
    },
    "start":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:00:00.0000000+00:00",
        "timeZone":"UTC"
    }
}
```
##### <a name="response"></a>Ответ
Ниже приведен пример ответа.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update bookingappointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
