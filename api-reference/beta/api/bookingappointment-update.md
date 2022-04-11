---
title: Обновление bookingAppointment
description: Обновите свойства объекта bookingAppointment в указанном bookingBusiness.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: fcbbb774d3981a1174493e2305c78e2042988985
ms.sourcegitcommit: 19558bd9de9b717e7a36bfce1d6d84d0132e2697
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2022
ms.locfileid: "64755553"
---
# <a name="update-bookingappointment"></a>Обновление bookingAppointment

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновите свойства объекта [bookingAppointment](../resources/bookingappointment.md) в указанном [bookingBusiness](../resources/bookingbusiness.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированное (рабочая или учебная учетная запись) |  BookingsAppointment.ReadWrite.All, Bookings. ReadWrite.All, Bookings. Manage.All   |
|Делегированное (личная учетная запись Майкрософт) | Не поддерживается.   |
|Application | BookingsAppointment.ReadWrite.All, Bookings. Read.All  |

> [!NOTE]
> При создании пользовательского приложения с использованием разрешений приложения необходимо выполнить проверку [бизнес-правил](/graph/bookingsbusiness-business-rules).

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/appointments/{id}
```

## <a name="optional-request-headers"></a>Необязательные заголовки запросов

| Имя       | Описание|
|:-----------|:-----------|
| Авторизация  | Носитель {code}. Обязательно.|

## <a name="request-body"></a>Текст запроса

[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|customerEmailAddress|String|SMTP-адрес [bookingCustomer](../resources/bookingcustomer.md) , который резервировать встречу.|
|customerId|String|Идентификатор объекта [bookingCustomer](../resources/bookingcustomer.md) для этой встречи. Если при создании встречи не указан идентификатор, создается новый объект **bookingCustomer** . После установки идентификатор **клиента** следует считать неизменяемым.|
|customerLocation|[location](../resources/location.md)|Представляет сведения о расположении [для bookingCustomer](../resources/bookingcustomer.md) , который резервирует встречу.|
|customerName|String|Имя клиента.|
|customerNotes|String|Заметки от клиента, связанного с этой встречей. Значение можно получить только при чтении **этого объекта bookingAppointment** по его идентификатору. <br> Это свойство можно задать только при первоначальном создании встречи с новым клиентом. По истечении этого момента значение вычисляется из клиента, представленного **идентификатором клиента**.|
|customerPhone|String|Номер телефона клиента.|
|Клиентов|[Коллекция bookingCustomerInformation](../resources/bookingcustomerinformation.md)|В нем перечислены свойства клиента для встречи. Встреча будет содержать список сведений о клиенте, и каждое подразделение будет указывать свойства клиента, который является частью этой встречи. Необязательное свойство.|
|customerTimeZone|String|Часовой пояс клиента. Список возможных значений см. в [разделе dateTimeTimeZone](../resources/datetimetimezone.md).|
|duration|Длительность|Длина встречи, помеченная в [формате ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|end|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата, время и часовой пояс, на которых заканчивается встреча.|
|invoiceAmount|Двойное с плавающей точкой|Сумма, выставленная в счете.|
|invoiceDate|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата, время и часовой пояс счета для этой встречи.|
|invoiceId|String|Идентификатор счета.|
|invoiceStatus|string| Состояние счета. Возможные значения: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.|
|invoiceUrl|String|URL-адрес счета в Microsoft Bookings.|
|filledAttendeesCount|Int32|Текущее число клиентов во встрече. Обязательный.|
|isLocationOnline|Boolean|Значение true указывает, что встреча будет храниться в сети. Значение по умолчанию − ложь.|
|maximumAttendeesCount|Int32|Максимальное число клиентов, разрешенных во время встречи. Обязательный. |
|optOutOfCustomerEmail|Boolean|Значение true указывает, [что bookingCustomer](../resources/bookingcustomer.md) для этой встречи не хочет получать подтверждение для этой встречи.|
|postBuffer|Длительность|Например, время резервирования после окончания встречи для очистки. Значение выражается в [формате ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|preBuffer|Длительность|Количество времени, зарезервируемого до начала встречи, для подготовки, в качестве примера. Значение выражается в [формате ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|Цена|Двойное с плавающей точкой|Обычная цена встречи для указанной [службы bookingService](../resources/bookingservice.md).|
|priceType|bookingPriceType| Параметр, предоставляющий гибкость для структуры ценообразования служб. Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`, `unknownFutureValue`.|
|Напоминания|[Коллекция bookingReminder](../resources/bookingreminder.md)|Коллекция напоминаний клиентов, отправленных для этой встречи. Значение этого свойства доступно только при чтении **этого объекта bookingAppointment** по его идентификатору.|
|selfServiceAppointmentId|String|Дополнительный идентификатор отслеживания встречи, если встреча была создана непосредственно клиентом на странице планирования, а не сотрудником от имени клиента.|
|serviceId|Строка|Идентификатор службы [bookingService](../resources/bookingservice.md) , связанной с этой встречей.|
|serviceLocation|[location](../resources/location.md)|Расположение, куда доставляется служба.|
|serviceName|String|Имя службы **bookingService,** связанной с этой встречей.<br>Это свойство является необязательным при создании новой встречи. Если значение не указано, оно вычисляется из службы, связанной с встречей, с помощью **свойства serviceId** .|
|serviceNotes|String|Заметки из [bookingStaffMember](../resources/bookingstaffmember.md). Значение этого свойства доступно только при чтении **этого объекта bookingAppointment** по его идентификатору.|
|smsNotificationsEnabled|Логическое|Значение true указывает, что для встречи клиентам будут отправляться SMS-уведомления. Значение по умолчанию − ложь.|
|staffMemberIds|Коллекция String|Идентификатор каждого объекта [bookingStaffMember](../resources/bookingstaffmember.md) , который запланирован на эту встречу.|
|начать|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата, время и часовой пояс, с которых начинается встреча.|

> [!NOTE]
> Если максимальное число клиентов (**maximumAttedeesCount**), разрешенное в службе, больше 1:[](../resources/bookingservice.md)
> - Убедитесь, что клиенты существуют в календаре резервирования. Если это не так, создайте его с помощью [операции Create bookingCustomer](bookingbusiness-post-customers.md) .
> - Передайте действительные идентификаторы клиентов при создании или обновлении встречи. Если недопустимый идентификатор клиента, он не будет включен в объект встречи.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. Он не возвращает ничего в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

В следующем примере дата обслуживания изменяется на день и обновляется дата счета.

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "update_bookingappointment"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/appointments/AAMkADKnAAA=
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingappointment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingappointment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingappointment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-bookingappointment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-bookingappointment-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-bookingappointment-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Отклик
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


