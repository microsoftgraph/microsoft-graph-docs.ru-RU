---
title: Список встреч
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: 5e0846a1671a7a566e5175a331dc7c03e02af537
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076346"
---
# <a name="list-appointments"></a><span data-ttu-id="2a554-104">Список встреч</span><span class="sxs-lookup"><span data-stu-id="2a554-104">List appointments</span></span>

 > <span data-ttu-id="2a554-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2a554-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2a554-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a554-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="2a554-107">Получите список объектов [bookingAppointment](../resources/bookingappointment.md) для указанного [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="2a554-107">Get a list of [bookingAppointment](../resources/bookingappointment.md) objects for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="2a554-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2a554-108">Permissions</span></span>
<span data-ttu-id="2a554-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a554-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a554-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a554-111">Permission type</span></span>      | <span data-ttu-id="2a554-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a554-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a554-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a554-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="2a554-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="2a554-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="2a554-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a554-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a554-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a554-116">Not supported.</span></span>   |
|<span data-ttu-id="2a554-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2a554-117">Application</span></span> | <span data-ttu-id="2a554-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a554-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="2a554-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a554-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/appointments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2a554-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2a554-120">Optional query parameters</span></span>
<span data-ttu-id="2a554-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2a554-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="2a554-122">Чтобы задать встреч business резервирования в интервал дат, а не `$filter`, [Получение представления календаря](bookingbusiness-list-calendarview.md) для этого диапазона дат.</span><span class="sxs-lookup"><span data-stu-id="2a554-122">To get the set of appointments of a Bookings business within a date range, instead of `$filter`, [get the calendarView](bookingbusiness-list-calendarview.md) for that date range.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="2a554-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2a554-123">Request headers</span></span>
| <span data-ttu-id="2a554-124">Имя</span><span class="sxs-lookup"><span data-stu-id="2a554-124">Name</span></span>      |<span data-ttu-id="2a554-125">Описание</span><span class="sxs-lookup"><span data-stu-id="2a554-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2a554-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a554-126">Authorization</span></span>  | <span data-ttu-id="2a554-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2a554-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a554-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2a554-128">Request body</span></span>
<span data-ttu-id="2a554-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2a554-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2a554-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="2a554-130">Response</span></span>
<span data-ttu-id="2a554-131">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [bookingAppointment](../resources/bookingappointment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2a554-131">If successful, this method returns a `200 OK` response code and collection of [bookingAppointment](../resources/bookingappointment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2a554-132">Пример</span><span class="sxs-lookup"><span data-stu-id="2a554-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2a554-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a554-133">Request</span></span>
<span data-ttu-id="2a554-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a554-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_appointments"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments
```
##### <a name="response"></a><span data-ttu-id="2a554-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="2a554-135">Response</span></span>
<span data-ttu-id="2a554-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2a554-136">The following is an example of the response.</span></span> <span data-ttu-id="2a554-137">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="2a554-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2a554-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2a554-138">All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/appointments",
    "value": [
        {
            "id": "AAMkADKoAAA=",
            "selfServiceAppointmentId": "00000000-0000-0000-0000-000000000000",
            "customerId": "829e3cb5-3d4d-4319-a8de-1953aedaa166",
            "customerName": "Bob Kelly",
            "customerEmailAddress": "bobk@tailspintoys.com",
            "customerPhone": "213-555-0108",
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
            "invoiceId": "1002",
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
                "dateTime": "2018-04-30T13:00:00.0000000Z",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2018-04-30T13:30:00.0000000Z",
                "timeZone": "UTC"
            },
            "serviceLocation": {
                "displayName": "Customer location (987 Third Avenue, Buffalo, NY 98052, USA)",
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
                "dateTime": "2018-04-30T13:30:00.0000000Z",
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
                "dateTime": "2018-05-01T12:00:00.0000000Z",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2018-05-01T12:30:00.0000000Z",
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
                "dateTime": "2018-05-01T12:30:00.0000000Z",
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
  "description": "List appointments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->