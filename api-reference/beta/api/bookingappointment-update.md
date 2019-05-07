---
title: Обновление букингаппоинтмент
description: Обновление свойств объекта Букингаппоинтмент в указанном букингбусинесс.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 32596ae8528f6c73ae4b82852baaed0031db7b57
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636214"
---
# <a name="update-bookingappointment"></a>Обновление букингаппоинтмент

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [букингаппоинтмент](../resources/bookingappointment.md) в указанном [букингбусинесс](../resources/bookingbusiness.md).
## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL   |
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
| Авторизация  | Bearer {code}|

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Кустомеремаиладдресс|String|SMTP-адрес [букингкустомер](../resources/bookingcustomer.md) , который зарезервировано встречу.|
|customerId|String|Идентификатор [букингкустомер](../resources/bookingcustomer.md) для этой встречи. Если при создании встречи не указан идентификатор, создается новый объект **букингкустомер** . После установки необходимо учесть неизменность **customerId** .|
|Кустомерлокатион|[location](../resources/location.md)|Представляет сведения о расположении для [букингкустомер](../resources/bookingcustomer.md) , который зарезервировано встречу.|
|customerName|String|Имя клиента.|
|Кустомернотес|String|Примечания от клиента, связанного с этой встречей. Значение можно получить только при чтении этого **букингаппоинтмент** по его идентификатору. <br> Это свойство можно задать только при первоначальном создании встречи с новым клиентом. После этой точки значение вычисляется от клиента, представленного **customerId**.|
|Кустомерфоне|String|Номер телефона клиента.|
|duration|Duration (Длительность)|Длительность встречи, обозначенная в формате [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|end|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата, время и часовой пояс, в котором заканчивается встреча.|
|Инвоицеамаунт|Двойное|Сумма счета в счете.|
|Инвоицедате|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата, время и часовой пояс накладной для данной встречи.|
|Инвоицеид|String|Идентификатор счета.|
|Инвоицестатус|string| Статус счета. Возможные значения: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.|
|Инвоицеурл|String|URL-адрес счета в книгах корпорации Майкрософт.|
|Оптаутофкустомеремаил|Логический|Значение true указывает, что [букингкустомер](../resources/bookingcustomer.md) для этой встречи не хочет получать подтверждение для этой встречи.|
|Буфер буфера|Duration (Длительность)|Количество времени, которое необходимо зарезервировать после окончания встречи, для очистки в качестве примера. Значение выражается в формате [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) . |
|пребуфер|Duration (Длительность)|Количество времени, которое необходимо зарезервировать до начала встречи, в качестве примера для подготовки. Значение выражается в формате [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) .|
|Цена|Двойное|Обычная цена для встречи с указанным [букингсервице](../resources/bookingservice.md).|
|Прицетипе|string| Параметр, обеспечивающий гибкость для структуры ценообразования служб. Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.|
|напоминания|Коллекция [букингреминдер](../resources/bookingreminder.md)|Коллекция напоминаний о клиентах, отправленных для этой встречи. Значение этого свойства доступно только при чтении этого **букингаппоинтмент** с помощью идентификатора.|
|Селфсервицеаппоинтментид|String|Дополнительный идентификатор отслеживания для встречи, если встреча создана непосредственно клиентом на странице планирования, в отличие от сотрудника от имени клиента;.|
|serviceId|String|Идентификатор [букингсервице](../resources/bookingservice.md) , связанный с этой встречей.|
|Сервицелокатион|[location](../resources/location.md)|Место доставки службы.|
|Служба|String|Имя **букингсервице** , связанного с этой встречей.<br>Это свойство является необязательным при создании новой встречи. Если он не указан, то он вычисляется из службы, связанной с встречей, с помощью свойства **serviceId** .|
|Сервиценотес|String|Заметки из [букингстаффмембер](../resources/bookingstaffmember.md). Значение этого свойства доступно только при чтении этого **букингаппоинтмент** с помощью идентификатора.|
|Стаффмемберидс|Коллекция String|Идентификатор каждого [букингстаффмембер](../resources/bookingstaffmember.md) , запланированного в этой встрече.|
|начать|[dateTimeTimeZone](../resources/datetimetimezone.md)|Дата, время и часовой пояс, с которого начинается встреча.|


## <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
В следующем примере дата обслуживания изменяется на день, а также обновляется и Дата выставления счета.
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
##### <a name="response"></a>Отклик
Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a>Пример кода для SDK
# <a name="ctabcs"></a>[Языках](#tab/cs)
[!INCLUDE [sample-code](../includes/update_bookingappointment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Язык](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_bookingappointment-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/bookingappointment-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingappointment-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
