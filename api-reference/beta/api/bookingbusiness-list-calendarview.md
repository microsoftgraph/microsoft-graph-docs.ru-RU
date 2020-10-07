---
title: Представление календаря "Список резервирований"
description: Получение коллекции объектов Букингаппоинтмент для Букингбусинесс, которая происходит в указанном диапазоне дат.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: d786bcff72d438f64cc4d21d5e8a7449c2c03ea2
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2020
ms.locfileid: "48372307"
---
# <a name="list-bookings-calendarview"></a><span data-ttu-id="1ce8c-103">Представление календаря "Список резервирований"</span><span class="sxs-lookup"><span data-stu-id="1ce8c-103">List Bookings calendarView</span></span>

<span data-ttu-id="1ce8c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ce8c-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ce8c-105">Получение коллекции объектов [букингаппоинтмент](../resources/bookingappointment.md) для [букингбусинесс](../resources/bookingbusiness.md), которая происходит в указанном диапазоне дат.</span><span class="sxs-lookup"><span data-stu-id="1ce8c-105">Get the collection of [bookingAppointment](../resources/bookingappointment.md) objects for a [bookingBusiness](../resources/bookingbusiness.md), that occurs in the specified date range.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ce8c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1ce8c-106">Permissions</span></span>
<span data-ttu-id="1ce8c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ce8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ce8c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ce8c-109">Permission type</span></span>      | <span data-ttu-id="1ce8c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ce8c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ce8c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ce8c-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="1ce8c-112">Резервирования. Read. ALL, Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="1ce8c-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="1ce8c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ce8c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ce8c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ce8c-114">Not supported.</span></span>   |
|<span data-ttu-id="1ce8c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1ce8c-115">Application</span></span> | <span data-ttu-id="1ce8c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ce8c-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="1ce8c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ce8c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/calendarView?start={start-value}&end={end-value}
```

## <a name="query-parameters"></a><span data-ttu-id="1ce8c-118">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="1ce8c-118">Query parameters</span></span>

<span data-ttu-id="1ce8c-119">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="1ce8c-119">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="1ce8c-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="1ce8c-120">Parameter</span></span>    | <span data-ttu-id="1ce8c-121">Тип</span><span class="sxs-lookup"><span data-stu-id="1ce8c-121">Type</span></span>   |<span data-ttu-id="1ce8c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1ce8c-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ce8c-123">начать</span><span class="sxs-lookup"><span data-stu-id="1ce8c-123">start</span></span>|<span data-ttu-id="1ce8c-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ce8c-124">DateTimeOffset</span></span>|<span data-ttu-id="1ce8c-125">Дата и время начала периода времени, представленного в формате ISO 8601, в формате UTC или смещение относительно времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="1ce8c-125">The start date and time of a time range, represented in ISO 8601 format, as UTC or an offset from UTC.</span></span> <span data-ttu-id="1ce8c-126">Например, полночь UTC 1 января 2018 будет выглядеть следующим образом: ' 2018 г.-01-01T00:00:00Z ', и одно и то же время в PST-файле будет выглядеть следующим образом: ' 2017-12-31T16:00:00-08:00 '.</span><span class="sxs-lookup"><span data-stu-id="1ce8c-126">For example, midnight UTC on Jan 1, 2018 would look like this: '2018-01-01T00:00:00Z', and the same time in PST would look like this: '2017-12-31T16:00:00-08:00'.</span></span>|
|<span data-ttu-id="1ce8c-127">end</span><span class="sxs-lookup"><span data-stu-id="1ce8c-127">end</span></span>|<span data-ttu-id="1ce8c-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ce8c-128">DateTimeOffset</span></span>|<span data-ttu-id="1ce8c-129">Дата и время окончания периода времени, представленного в формате ISO 8601, в формате UTC или смещение относительно времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="1ce8c-129">The end date and time of a time range, represented in ISO 8601 format, as UTC or an offset from UTC.</span></span> <span data-ttu-id="1ce8c-130">Например, 3am UTC на 1 января 2018, будет выглядеть следующим образом: ' 2018 г.-01-01T03:00:00Z ', и одно и то же время в PST-файле будет выглядеть следующим образом: ' 2017-12-31T19:00:00-08:00 '.</span><span class="sxs-lookup"><span data-stu-id="1ce8c-130">For example, 3am UTC on Jan 1, 2018 would look like this: '2018-01-01T03:00:00Z', and the same time in PST would look like this: '2017-12-31T19:00:00-08:00'.</span></span>|

<span data-ttu-id="1ce8c-131">Значения `start` и `end` интерпретируются с использованием смещения часового пояса, указанного в соответствующих значениях, и не влияют на значение заголовка, если оно `Prefer: outlook.timezone` присутствует.</span><span class="sxs-lookup"><span data-stu-id="1ce8c-131">The values of `start` and `end` are interpreted using the timezone offset specified in their corresponding values and are not impacted by the value of the `Prefer: outlook.timezone` header if present.</span></span>

<span data-ttu-id="1ce8c-132">Этот метод также поддерживает некоторые [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="1ce8c-132">This method also supports some of the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1ce8c-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1ce8c-133">Request headers</span></span>
| <span data-ttu-id="1ce8c-134">Имя</span><span class="sxs-lookup"><span data-stu-id="1ce8c-134">Name</span></span>       | <span data-ttu-id="1ce8c-135">Описание</span><span class="sxs-lookup"><span data-stu-id="1ce8c-135">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1ce8c-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1ce8c-136">Authorization</span></span>  | <span data-ttu-id="1ce8c-137">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="1ce8c-137">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ce8c-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1ce8c-138">Request body</span></span>
<span data-ttu-id="1ce8c-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1ce8c-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ce8c-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ce8c-140">Response</span></span>
<span data-ttu-id="1ce8c-141">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и объект коллекции [букингаппоинтмент](../resources/bookingappointment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1ce8c-141">If successful, this method returns `200, OK` response code and [bookingAppointment](../resources/bookingappointment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ce8c-142">Пример</span><span class="sxs-lookup"><span data-stu-id="1ce8c-142">Example</span></span>
<span data-ttu-id="1ce8c-143">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="1ce8c-143">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1ce8c-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ce8c-144">Request</span></span>
<span data-ttu-id="1ce8c-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1ce8c-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1ce8c-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ce8c-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_getcalendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/calendarView?start=2018-04-30T00:00:00Z&end=2018-05-10T00:00:00Z
```
# <a name="c"></a>[<span data-ttu-id="1ce8c-147">C#</span><span class="sxs-lookup"><span data-stu-id="1ce8c-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingbusiness-getcalendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1ce8c-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1ce8c-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingbusiness-getcalendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1ce8c-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1ce8c-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingbusiness-getcalendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1ce8c-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ce8c-150">Response</span></span>
<span data-ttu-id="1ce8c-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1ce8c-151">The following is an example of the response.</span></span> <span data-ttu-id="1ce8c-152">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="1ce8c-152">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1ce8c-153">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1ce8c-153">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingAppointment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/calendarView",
    "value": [
        {
            "id": "AAMkADKpAAA=",
            "selfServiceAppointmentId": "00000000-0000-0000-0000-000000000000",
            "customerId": "80b5ddda-1e3b-4c9d-abe2-d606cc075e2e",
            "customerName": "Adele Vance",
            "customerEmailAddress": "adelev@proseware.com",
            "customerPhone": "213-555-0156",
            "customerNotes": null,
            "serviceId": "57da6774-a087-4d69-b0e6-6fb82c339976",
            "serviceName": "Catered bento",
            "duration": "PT30M",
            "preBuffer": "PT5M",
            "postBuffer": "PT10M",
            "priceType": "fixedPrice",
            "price": 10,
            "serviceNotes": null,
            "optOutOfCustomerEmail": false,
            "staffMemberIds": [],
            "invoiceAmount": 10,
            "invoiceId": "1003",
            "invoiceStatus": "open",
            "invoiceUrl": "theInvoiceUrl",
            "customerLocation": {
                "displayName": "Customer",
                "locationEmailAddress": null,
                "locationUri": "",
                "locationType": null,
                "uniqueId": null,
                "uniqueIdType": null,
                "address": {
                    "type": "home",
                    "postOfficeBox": "",
                    "street": "",
                    "city": "",
                    "state": "",
                    "countryOrRegion": "",
                    "postalCode": ""
                },
                "coordinates": {
                    "altitude": null,
                    "latitude": null,
                    "longitude": null,
                    "accuracy": null,
                    "altitudeAccuracy": null
                }
            },
            "start": {
                "dateTime": "2018-05-05T12:00:00.0000000Z",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2018-05-05T12:30:00.0000000Z",
                "timeZone": "UTC"
            },
            "serviceLocation": {
                "displayName": "Customer location (876 Tenth Avenue, Buffalo, NY 98052, USA)",
                "locationEmailAddress": null,
                "locationUri": "",
                "locationType": null,
                "uniqueId": null,
                "uniqueIdType": null,
                "address": {
                    "type": "home",
                    "postOfficeBox": "",
                    "street": "",
                    "city": "",
                    "state": "",
                    "countryOrRegion": "",
                    "postalCode": ""
                },
                "coordinates": {
                    "altitude": null,
                    "latitude": null,
                    "longitude": null,
                    "accuracy": null,
                    "altitudeAccuracy": null
                }
            },
            "reminders": [],
            "invoiceDate": {
                "dateTime": "2018-05-05T12:30:00.0000000Z",
                "timeZone": "UTC"
            }
        },
        {
            "id": "AAMkADKnAAA=",
            "selfServiceAppointmentId": "00000000-0000-0000-0000-000000000000",
            "customerId": "7ed53fa5-9ef2-4f2f-975b-27447440bc09",
            "customerName": "Jordan Miller",
            "customerEmailAddress": "jordanm@contoso.com",
            "customerPhone": "213-555-0199",
            "customerNotes": null,
            "serviceId": "57da6774-a087-4d69-b0e6-6fb82c339976",
            "serviceName": "Catered bento",
            "duration": "PT30M",
            "preBuffer": "PT5M",
            "postBuffer": "PT10M",
            "priceType": "fixedPrice",
            "price": 10,
            "serviceNotes": null,
            "optOutOfCustomerEmail": false,
            "staffMemberIds": [],
            "invoiceAmount": 10,
            "invoiceId": "1001",
            "invoiceStatus": "open",
            "invoiceUrl": "theInvoiceUrl",
            "customerLocation": {
                "displayName": "Customer",
                "locationEmailAddress": null,
                "locationUri": "",
                "locationType": null,
                "uniqueId": null,
                "uniqueIdType": null,
                "address": {
                    "type": "home",
                    "postOfficeBox": "",
                    "street": "",
                    "city": "",
                    "state": "",
                    "countryOrRegion": "",
                    "postalCode": ""
                },
                "coordinates": {
                    "altitude": null,
                    "latitude": null,
                    "longitude": null,
                    "accuracy": null,
                    "altitudeAccuracy": null
                }
            },
            "start": {
                "dateTime": "2018-05-06T12:00:00.0000000Z",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2018-05-06T12:30:00.0000000Z",
                "timeZone": "UTC"
            },
            "serviceLocation": {
                "displayName": "Customer location (123 First Avenue, Buffalo, NY 98052, USA)",
                "locationEmailAddress": null,
                "locationUri": "",
                "locationType": null,
                "uniqueId": null,
                "uniqueIdType": null,
                "address": {
                    "type": "home",
                    "postOfficeBox": "",
                    "street": "",
                    "city": "",
                    "state": "",
                    "countryOrRegion": "",
                    "postalCode": ""
                },
                "coordinates": {
                    "altitude": null,
                    "latitude": null,
                    "longitude": null,
                    "accuracy": null,
                    "altitudeAccuracy": null
                }
            },
            "reminders": [],
            "invoiceDate": {
                "dateTime": "2018-05-06T12:30:00.0000000Z",
                "timeZone": "UTC"
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingBusiness: getCalendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
