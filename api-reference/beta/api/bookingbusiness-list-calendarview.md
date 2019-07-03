---
title: Представление календаря "Список резервирований"
description: Получение коллекции объектов Букингаппоинтмент для Букингбусинесс, которая происходит в указанном диапазоне дат.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 95a72cacef1ca2c52f0bf6c80b9428eeb99f5d19
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439289"
---
# <a name="list-bookings-calendarview"></a><span data-ttu-id="89cb5-103">Представление календаря "Список резервирований"</span><span class="sxs-lookup"><span data-stu-id="89cb5-103">List Bookings calendarView</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89cb5-104">Получение коллекции объектов [букингаппоинтмент](../resources/bookingappointment.md) для [букингбусинесс](../resources/bookingbusiness.md), которая происходит в указанном диапазоне дат.</span><span class="sxs-lookup"><span data-stu-id="89cb5-104">Get the collection of [bookingAppointment](../resources/bookingappointment.md) objects for a [bookingBusiness](../resources/bookingbusiness.md), that occurs in the specified date range.</span></span>

## <a name="permissions"></a><span data-ttu-id="89cb5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="89cb5-105">Permissions</span></span>
<span data-ttu-id="89cb5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89cb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89cb5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89cb5-108">Permission type</span></span>      | <span data-ttu-id="89cb5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="89cb5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89cb5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89cb5-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="89cb5-111">Резервирования. Read. ALL, Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="89cb5-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="89cb5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89cb5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89cb5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89cb5-113">Not supported.</span></span>   |
|<span data-ttu-id="89cb5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="89cb5-114">Application</span></span> | <span data-ttu-id="89cb5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89cb5-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="89cb5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89cb5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/calendarView?start={start-value}&end={end-value}

```
## <a name="request-headers"></a><span data-ttu-id="89cb5-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="89cb5-117">Request headers</span></span>
| <span data-ttu-id="89cb5-118">Имя</span><span class="sxs-lookup"><span data-stu-id="89cb5-118">Name</span></span>       | <span data-ttu-id="89cb5-119">Описание</span><span class="sxs-lookup"><span data-stu-id="89cb5-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="89cb5-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="89cb5-120">Authorization</span></span>  | <span data-ttu-id="89cb5-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="89cb5-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="89cb5-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="89cb5-122">Request body</span></span>
<span data-ttu-id="89cb5-123">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="89cb5-123">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="89cb5-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="89cb5-124">Parameter</span></span>    | <span data-ttu-id="89cb5-125">Тип</span><span class="sxs-lookup"><span data-stu-id="89cb5-125">Type</span></span>   |<span data-ttu-id="89cb5-126">Описание</span><span class="sxs-lookup"><span data-stu-id="89cb5-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89cb5-127">начать</span><span class="sxs-lookup"><span data-stu-id="89cb5-127">start</span></span>|<span data-ttu-id="89cb5-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89cb5-128">DateTimeOffset</span></span>|<span data-ttu-id="89cb5-129">Дата и время начала периода времени, представленного в формате ISO 8601, в формате UTC или смещение относительно времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="89cb5-129">The start date and time of a time range, represented in ISO 8601 format, as UTC or an offset from UTC.</span></span> <span data-ttu-id="89cb5-130">Например, полночь UTC 1 января 2018 будет выглядеть следующим образом: ' 2018 г.-01-01T00:00:00Z ', и одно и то же время в PST-файле будет выглядеть следующим образом: ' 2017-12-31T16:00:00-08:00 '.</span><span class="sxs-lookup"><span data-stu-id="89cb5-130">For example, midnight UTC on Jan 1, 2018 would look like this: '2018-01-01T00:00:00Z', and the same time in PST would look like this: '2017-12-31T16:00:00-08:00'.</span></span>|
|<span data-ttu-id="89cb5-131">end</span><span class="sxs-lookup"><span data-stu-id="89cb5-131">end</span></span>|<span data-ttu-id="89cb5-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89cb5-132">DateTimeOffset</span></span>|<span data-ttu-id="89cb5-133">Дата и время окончания периода времени, представленного в формате ISO 8601, в формате UTC или смещение относительно времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="89cb5-133">The end date and time of a time range, represented in ISO 8601 format, as UTC or an offset from UTC.</span></span> <span data-ttu-id="89cb5-134">Например, 3am UTC на 1 января 2018, будет выглядеть следующим образом: ' 2018 г.-01-01T03:00:00Z ', и одно и то же время в PST-файле будет выглядеть следующим образом: ' 2017-12-31T19:00:00-08:00 '.</span><span class="sxs-lookup"><span data-stu-id="89cb5-134">For example, 3am UTC on Jan 1, 2018 would look like this: '2018-01-01T03:00:00Z', and the same time in PST would look like this: '2017-12-31T19:00:00-08:00'.</span></span>|

## <a name="response"></a><span data-ttu-id="89cb5-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="89cb5-135">Response</span></span>
<span data-ttu-id="89cb5-136">В случае успешного выполнения этот метод `200, OK` возвращает код отклика и объект коллекции [букингаппоинтмент](../resources/bookingappointment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="89cb5-136">If successful, this method returns `200, OK` response code and [bookingAppointment](../resources/bookingappointment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89cb5-137">Пример</span><span class="sxs-lookup"><span data-stu-id="89cb5-137">Example</span></span>
<span data-ttu-id="89cb5-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="89cb5-138">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="89cb5-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="89cb5-139">Request</span></span>
<span data-ttu-id="89cb5-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89cb5-140">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="89cb5-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="89cb5-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_getcalendarview"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/calendarView?start=2018-04-30T00:00:00Z&end=2018-05-10T00:00:00Z
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="89cb5-142">C#</span><span class="sxs-lookup"><span data-stu-id="89cb5-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingbusiness-getcalendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="89cb5-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="89cb5-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingbusiness-getcalendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="89cb5-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="89cb5-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingbusiness-getcalendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="89cb5-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="89cb5-145">Response</span></span>
<span data-ttu-id="89cb5-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="89cb5-146">The following is an example of the response.</span></span> <span data-ttu-id="89cb5-147">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="89cb5-147">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="89cb5-148">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="89cb5-148">All of the properties will be returned from an actual call.</span></span>
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
