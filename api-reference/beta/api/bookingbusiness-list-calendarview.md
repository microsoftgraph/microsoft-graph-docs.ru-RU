---
title: Список резервирования представления календаря
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: 5abf88b4d0f0f5721ba3bcbf467406cfedfbe9f0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809466"
---
# <a name="list-bookings-calendarview"></a><span data-ttu-id="b90a8-104">Список резервирования представления календаря</span><span class="sxs-lookup"><span data-stu-id="b90a8-104">List Bookings calendarView</span></span>

 > <span data-ttu-id="b90a8-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b90a8-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b90a8-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b90a8-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="b90a8-107">Получите коллекцию объектов [bookingAppointment](../resources/bookingappointment.md) для [bookingBusiness](../resources/bookingbusiness.md), что происходит в за указанный диапазон дат.</span><span class="sxs-lookup"><span data-stu-id="b90a8-107">Get the collection of [bookingAppointment](../resources/bookingappointment.md) objects for a [bookingBusiness](../resources/bookingbusiness.md), that occurs in the specified date range.</span></span>

## <a name="permissions"></a><span data-ttu-id="b90a8-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b90a8-108">Permissions</span></span>
<span data-ttu-id="b90a8-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b90a8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b90a8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b90a8-111">Permission type</span></span>      | <span data-ttu-id="b90a8-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b90a8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b90a8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b90a8-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="b90a8-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="b90a8-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="b90a8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b90a8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b90a8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b90a8-116">Not supported.</span></span>   |
|<span data-ttu-id="b90a8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b90a8-117">Application</span></span> | <span data-ttu-id="b90a8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b90a8-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="b90a8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b90a8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/calendarView?start={start-value}&end={end-value}

```
## <a name="request-headers"></a><span data-ttu-id="b90a8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b90a8-120">Request headers</span></span>
| <span data-ttu-id="b90a8-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b90a8-121">Name</span></span>       | <span data-ttu-id="b90a8-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b90a8-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b90a8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b90a8-123">Authorization</span></span>  | <span data-ttu-id="b90a8-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b90a8-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b90a8-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b90a8-125">Request body</span></span>
<span data-ttu-id="b90a8-126">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="b90a8-126">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="b90a8-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="b90a8-127">Parameter</span></span>    | <span data-ttu-id="b90a8-128">Тип</span><span class="sxs-lookup"><span data-stu-id="b90a8-128">Type</span></span>   |<span data-ttu-id="b90a8-129">Описание</span><span class="sxs-lookup"><span data-stu-id="b90a8-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b90a8-130">start</span><span class="sxs-lookup"><span data-stu-id="b90a8-130">start</span></span>|<span data-ttu-id="b90a8-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b90a8-131">DateTimeOffset</span></span>|<span data-ttu-id="b90a8-132">Дата и время начала интервала, представленного в формате ISO 8601, как UTC или смещение времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="b90a8-132">The start date and time of a time range, represented in ISO 8601 format, as UTC or an offset from UTC.</span></span> <span data-ttu-id="b90a8-133">Например полночь по Гринвичу на 1 января 2018 будет выглядеть следующим образом: "2018-01-01T00:00:00Z", и то же время в PST-файлов будет выглядеть следующим образом: "2017-12-31T16:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="b90a8-133">For example, midnight UTC on Jan 1, 2018 would look like this: '2018-01-01T00:00:00Z', and the same time in PST would look like this: '2017-12-31T16:00:00-08:00'.</span></span>|
|<span data-ttu-id="b90a8-134">end</span><span class="sxs-lookup"><span data-stu-id="b90a8-134">end</span></span>|<span data-ttu-id="b90a8-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b90a8-135">DateTimeOffset</span></span>|<span data-ttu-id="b90a8-136">Дата и время окончания интервала, представленного в формате ISO 8601, как UTC или смещение времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="b90a8-136">The end date and time of a time range, represented in ISO 8601 format, as UTC or an offset from UTC.</span></span> <span data-ttu-id="b90a8-137">В примере 3 am UTC на 1 января 2018 будет выглядеть следующим образом: "2018-01-01T03:00:00Z", и то же время в PST-файлов будет выглядеть следующим образом: "2017-12-31T19:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="b90a8-137">For example, 3am UTC on Jan 1, 2018 would look like this: '2018-01-01T03:00:00Z', and the same time in PST would look like this: '2017-12-31T19:00:00-08:00'.</span></span>|

## <a name="response"></a><span data-ttu-id="b90a8-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="b90a8-138">Response</span></span>
<span data-ttu-id="b90a8-139">Успешно завершена, этот метод возвращает `200, OK` кода и [bookingAppointment](../resources/bookingappointment.md) коллекции объект ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b90a8-139">If successful, this method returns `200, OK` response code and [bookingAppointment](../resources/bookingappointment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b90a8-140">Пример</span><span class="sxs-lookup"><span data-stu-id="b90a8-140">Example</span></span>
<span data-ttu-id="b90a8-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="b90a8-141">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b90a8-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="b90a8-142">Request</span></span>
<span data-ttu-id="b90a8-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b90a8-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_getcalendarview"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/calendarView?start=2018-04-30T00:00:00Z&end=2018-05-10T00:00:00Z
```

##### <a name="response"></a><span data-ttu-id="b90a8-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="b90a8-144">Response</span></span>
<span data-ttu-id="b90a8-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b90a8-145">The following is an example of the response.</span></span> <span data-ttu-id="b90a8-146">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="b90a8-146">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b90a8-147">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b90a8-147">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "bookingBusiness: getCalendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
