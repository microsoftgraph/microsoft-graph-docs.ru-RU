---
title: Обновление bookingappointment
description: Обновление свойств объекта bookingAppointment в указанном bookingbusiness.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 82f58ccde66790c09aad80e84ef2aa2bc1b7addb
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094863"
---
# <a name="update-bookingappointment"></a>Обновление bookingappointment

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [bookingAppointment](../resources/bookingappointment.md) в указанном [bookingBusiness](../resources/bookingbusiness.md).
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
| Авторизация  | Bearer {код}. Обязательно.|

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|customerEmailAddress|Строка|SMTP-адрес [bookingCustomer,](../resources/bookingcustomer.md) который бронирует встречу.|
|customerId|String|ID [bookingCustomer](../resources/bookingcustomer.md) для этого назначения. Если при назначении не указывается номер, создается новый объект **bookingCustomer.** После набора следует считать **customerId** неуменяемым.|
|customerLocation|[location](../resources/location.md)|Представляет сведения о расположении [для bookingCustomer,](../resources/bookingcustomer.md) который бронирует встречу.|
|имя клиента|String|Имя клиента.|
|customerNotes|Строка|Заметки от клиента, связанного с этим назначением. Значение можно получить только при чтении этого **bookingAppointment** по его ID. <br> Это свойство можно установить только при первоначальном создании встречи с новым клиентом. После этого значение вычисляется от клиента, представленного **customerId.**|
|customerPhone|String|Номер телефона клиента.|
|клиенты|[коллекция bookingCustomerInformation](../resources/bookingcustomerinformation.md)|В нем перечислены свойства клиента для встречи. Встреча будет содержать список сведений о клиентах, и каждое подразделение будет указывать свойства клиента, который является частью этого назначения. Необязательное свойство.|
|customerTimeZone|Строка|Часовой пояс клиента. Список возможных значений см. в [списке dateTimeTimeZone.](../resources/datetimetimezone.md)|
|duration|Длительность|Продолжительность встречи, обозначаемая в [формате ISO8601.](https://www.iso.org/iso-8601-date-and-time-format.html) |
|end|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата, время и часовой пояс, которые заканчивается встреча.|
|invoiceAmount|Double|Выставленная на счету сумма.|
|invoiceDate|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата, время и часовой пояс счета-фактуры для этого назначения.|
|invoiceId|String|ID счета-фактуры.|
|invoiceStatus|string| Состояние счета. Возможные значения: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.|
|invoiceUrl|String|URL-адрес счета в Microsoft Bookings.|
|filledAttendeesCount|Int32|Текущее число клиентов в записи. Обязательный.|
|isLocationOnline|Логический|True указывает, что встреча будет проходить в Интернете. Значение по умолчанию − ложь.|
|maximumAttendeesCount|Int32|Максимальное количество клиентов, разрешенных при встрече. Обязательное.|
|optOutOfCustomerEmail|Логическое|True указывает, что [bookingCustomer](../resources/bookingcustomer.md) для этого назначения не желает получать подтверждение для этого назначения.|
|postBuffer|Длительность|Количество времени, необходимое для резерва после окончания встречи, для очистки в качестве примера. Значение выражается в [формате ISO8601.](https://www.iso.org/iso-8601-date-and-time-format.html) |
|preBuffer|Длительность|Количество времени, необходимое для резерва перед началом встречи, для подготовки в качестве примера. Значение выражается в [формате ISO8601.](https://www.iso.org/iso-8601-date-and-time-format.html)|
|цена|Double|Обычная цена встречи для указанного [bookingService.](../resources/bookingservice.md)|
|priceType|bookingPriceType| Параметр, который обеспечивает гибкость структуры ценообразования служб. Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`, `unknownFutureValue`.|
|напоминания|[коллекция bookingReminder](../resources/bookingreminder.md)|Коллекция напоминаний клиентов, отправленных для этого назначения. Значение этого свойства доступно только при чтении этого **bookingAppointment** по его ID.|
|selfServiceAppointmentId|String|Дополнительный ИД отслеживания для встречи, если назначение было создано непосредственно клиентом на странице планирования, а не сотрудником от имени клиента.|
|serviceId|Строка|ID службы [bookingService,](../resources/bookingservice.md) связанной с этим назначением.|
|serviceLocation|[location](../resources/location.md)|Расположение, в котором доставляется служба.|
|serviceName|Строка|Имя **bookingService, связанного** с этим назначением.<br>Это свойство является необязательным при создании новой встречи. Если не указано, оно вычисляется из службы, связанной с назначением **свойством serviceId.**|
|serviceNotes|Строка|Заметки [из bookingStaffMember](../resources/bookingstaffmember.md). Значение этого свойства доступно только при чтении этого **bookingAppointment** по его ID.|
|smsNotificationsEnabled|Логический|True указывает, что sms-уведомления будут отправлены клиентам для встречи. Значение по умолчанию − ложь.|
|staffMemberIds|Коллекция строк|ID каждого [бронированияStaffMember,](../resources/bookingstaffmember.md) который запланирован в этом назначении.|
|начать|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата, время и часовой пояс, в который начинается встреча.|


## <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.
## <a name="example"></a>Пример
### <a name="request"></a>Запрос
В следующем примере дата службы изменяется на день и обновляется.

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


