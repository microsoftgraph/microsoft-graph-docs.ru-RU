---
title: Получение bookingAppointment
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: 7b9b04a8104bfe6f4569a31d0e88616af4e97fdc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850801"
---
# <a name="get-bookingappointment"></a><span data-ttu-id="789f5-104">Получение bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="789f5-104">Get bookingAppointment</span></span>

 > <span data-ttu-id="789f5-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="789f5-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="789f5-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="789f5-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="789f5-107">Получите свойства и связи объекта [bookingAppointment](../resources/bookingappointment.md) в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="789f5-107">Get the properties and relationships of a [bookingAppointment](../resources/bookingappointment.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="789f5-108">Свойства **start** и **end** всегда возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="789f5-108">The **start** and **end** properties are always returned in UTC.</span></span>
## <a name="permissions"></a><span data-ttu-id="789f5-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="789f5-109">Permissions</span></span>
<span data-ttu-id="789f5-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="789f5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="789f5-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="789f5-112">Permission type</span></span>      | <span data-ttu-id="789f5-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="789f5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="789f5-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="789f5-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="789f5-115">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="789f5-115">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="789f5-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="789f5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="789f5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="789f5-117">Not supported.</span></span>   |
|<span data-ttu-id="789f5-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="789f5-118">Application</span></span> | <span data-ttu-id="789f5-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="789f5-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="789f5-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="789f5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/appointments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="789f5-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="789f5-121">Optional query parameters</span></span>
<span data-ttu-id="789f5-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="789f5-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="789f5-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="789f5-123">Request headers</span></span>
| <span data-ttu-id="789f5-124">Имя</span><span class="sxs-lookup"><span data-stu-id="789f5-124">Name</span></span>      |<span data-ttu-id="789f5-125">Описание</span><span class="sxs-lookup"><span data-stu-id="789f5-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="789f5-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="789f5-126">Authorization</span></span>  | <span data-ttu-id="789f5-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="789f5-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="789f5-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="789f5-128">Request body</span></span>
<span data-ttu-id="789f5-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="789f5-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="789f5-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="789f5-130">Response</span></span>
<span data-ttu-id="789f5-131">Успешно завершена, этот метод возвращает `200 OK` объект [bookingAppointment](../resources/bookingappointment.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="789f5-131">If successful, this method returns a `200 OK` response code and [bookingAppointment](../resources/bookingappointment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="789f5-132">Пример</span><span class="sxs-lookup"><span data-stu-id="789f5-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="789f5-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="789f5-133">Request</span></span>
<span data-ttu-id="789f5-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="789f5-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingappointment"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKnAAA=
```
##### <a name="response"></a><span data-ttu-id="789f5-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="789f5-135">Response</span></span>
<span data-ttu-id="789f5-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="789f5-136">The following is an example of the response.</span></span> <span data-ttu-id="789f5-137">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="789f5-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="789f5-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="789f5-138">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingAppointment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/appointments/$entity",
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
    "serviceNotes": "Customer requires punctual service.",
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
    "reminders": [
        {
            "offset": "P1D",
            "recipients": "allAttendees",
            "message": "This service is tomorrow"
        },
        {
            "offset": "PT1H",
            "recipients": "customer",
            "message": "Please be available to enjoy your lunch service."
        },
        {
            "offset": "PT2H",
            "recipients": "staff",
            "message": "Please check traffic for next cater."
        }
    ],
    "invoiceDate": {
        "dateTime": "2018-05-06T12:30:00.0000000Z",
        "timeZone": "UTC"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get bookingAppointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
