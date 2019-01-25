---
title: Список резервирования представления календаря
description: Получите коллекцию объектов bookingAppointment для bookingBusiness, что происходит в за указанный диапазон дат.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 39b96e089d035ffd21155064252e36fd07a0a6c5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526076"
---
# <a name="list-bookings-calendarview"></a><span data-ttu-id="ebc08-103">Список резервирования представления календаря</span><span class="sxs-lookup"><span data-stu-id="ebc08-103">List Bookings calendarView</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebc08-104">Получите коллекцию объектов [bookingAppointment](../resources/bookingappointment.md) для [bookingBusiness](../resources/bookingbusiness.md), что происходит в за указанный диапазон дат.</span><span class="sxs-lookup"><span data-stu-id="ebc08-104">Get the collection of [bookingAppointment](../resources/bookingappointment.md) objects for a [bookingBusiness](../resources/bookingbusiness.md), that occurs in the specified date range.</span></span>

## <a name="permissions"></a><span data-ttu-id="ebc08-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ebc08-105">Permissions</span></span>
<span data-ttu-id="ebc08-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebc08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebc08-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ebc08-108">Permission type</span></span>      | <span data-ttu-id="ebc08-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ebc08-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebc08-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ebc08-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="ebc08-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="ebc08-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="ebc08-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ebc08-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebc08-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebc08-113">Not supported.</span></span>   |
|<span data-ttu-id="ebc08-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ebc08-114">Application</span></span> | <span data-ttu-id="ebc08-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebc08-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="ebc08-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ebc08-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/calendarView?start={start-value}&end={end-value}

```
## <a name="request-headers"></a><span data-ttu-id="ebc08-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ebc08-117">Request headers</span></span>
| <span data-ttu-id="ebc08-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ebc08-118">Name</span></span>       | <span data-ttu-id="ebc08-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ebc08-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ebc08-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebc08-120">Authorization</span></span>  | <span data-ttu-id="ebc08-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ebc08-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebc08-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ebc08-122">Request body</span></span>
<span data-ttu-id="ebc08-123">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="ebc08-123">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="ebc08-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="ebc08-124">Parameter</span></span>    | <span data-ttu-id="ebc08-125">Тип</span><span class="sxs-lookup"><span data-stu-id="ebc08-125">Type</span></span>   |<span data-ttu-id="ebc08-126">Описание</span><span class="sxs-lookup"><span data-stu-id="ebc08-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ebc08-127">start</span><span class="sxs-lookup"><span data-stu-id="ebc08-127">start</span></span>|<span data-ttu-id="ebc08-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebc08-128">DateTimeOffset</span></span>|<span data-ttu-id="ebc08-129">Дата и время начала интервала, представленного в формате ISO 8601, как UTC или смещение времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="ebc08-129">The start date and time of a time range, represented in ISO 8601 format, as UTC or an offset from UTC.</span></span> <span data-ttu-id="ebc08-130">Например полночь по Гринвичу на 1 января 2018 будет выглядеть следующим образом: "2018-01-01T00:00:00Z", и то же время в PST-файлов будет выглядеть следующим образом: "2017-12-31T16:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="ebc08-130">For example, midnight UTC on Jan 1, 2018 would look like this: '2018-01-01T00:00:00Z', and the same time in PST would look like this: '2017-12-31T16:00:00-08:00'.</span></span>|
|<span data-ttu-id="ebc08-131">end</span><span class="sxs-lookup"><span data-stu-id="ebc08-131">end</span></span>|<span data-ttu-id="ebc08-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebc08-132">DateTimeOffset</span></span>|<span data-ttu-id="ebc08-133">Дата и время окончания интервала, представленного в формате ISO 8601, как UTC или смещение времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="ebc08-133">The end date and time of a time range, represented in ISO 8601 format, as UTC or an offset from UTC.</span></span> <span data-ttu-id="ebc08-134">В примере 3 am UTC на 1 января 2018 будет выглядеть следующим образом: "2018-01-01T03:00:00Z", и то же время в PST-файлов будет выглядеть следующим образом: "2017-12-31T19:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="ebc08-134">For example, 3am UTC on Jan 1, 2018 would look like this: '2018-01-01T03:00:00Z', and the same time in PST would look like this: '2017-12-31T19:00:00-08:00'.</span></span>|

## <a name="response"></a><span data-ttu-id="ebc08-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="ebc08-135">Response</span></span>
<span data-ttu-id="ebc08-136">Успешно завершена, этот метод возвращает `200, OK` кода и [bookingAppointment](../resources/bookingappointment.md) коллекции объект ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ebc08-136">If successful, this method returns `200, OK` response code and [bookingAppointment](../resources/bookingappointment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebc08-137">Пример</span><span class="sxs-lookup"><span data-stu-id="ebc08-137">Example</span></span>
<span data-ttu-id="ebc08-138">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ebc08-138">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ebc08-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="ebc08-139">Request</span></span>
<span data-ttu-id="ebc08-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ebc08-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_getcalendarview"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/calendarView?start=2018-04-30T00:00:00Z&end=2018-05-10T00:00:00Z
```

##### <a name="response"></a><span data-ttu-id="ebc08-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="ebc08-141">Response</span></span>
<span data-ttu-id="ebc08-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ebc08-142">The following is an example of the response.</span></span> <span data-ttu-id="ebc08-143">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="ebc08-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ebc08-144">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ebc08-144">All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/bookingbusiness-list-calendarview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
