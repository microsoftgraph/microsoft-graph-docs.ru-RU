---
title: Создание bookingAppointment
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 1efde8ef8678afcee97939130e23b52312b03d83
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936804"
---
# <a name="create-bookingappointment"></a><span data-ttu-id="f55e6-104">Создание bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="f55e6-104">Create bookingAppointment</span></span>

 > <span data-ttu-id="f55e6-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f55e6-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f55e6-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f55e6-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="f55e6-107">Создание нового [bookingAppointment](../resources/bookingappointment.md) для указанного [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="f55e6-107">Create a new [bookingAppointment](../resources/bookingappointment.md) for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="f55e6-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f55e6-108">Permissions</span></span>
<span data-ttu-id="f55e6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f55e6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f55e6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f55e6-111">Permission type</span></span>      | <span data-ttu-id="f55e6-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f55e6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f55e6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f55e6-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="f55e6-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="f55e6-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="f55e6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f55e6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f55e6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f55e6-116">Not supported.</span></span>   |
|<span data-ttu-id="f55e6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f55e6-117">Application</span></span> | <span data-ttu-id="f55e6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f55e6-118">Not supported.</span></span>  |  

## <a name="http-request"></a><span data-ttu-id="f55e6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f55e6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments

```
## <a name="request-headers"></a><span data-ttu-id="f55e6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f55e6-120">Request headers</span></span>
| <span data-ttu-id="f55e6-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f55e6-121">Name</span></span>       | <span data-ttu-id="f55e6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f55e6-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f55e6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f55e6-123">Authorization</span></span>  | <span data-ttu-id="f55e6-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f55e6-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="f55e6-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f55e6-125">Request body</span></span>
<span data-ttu-id="f55e6-126">В тексте запроса укажите представление JSON объекта [bookingAppointment](../resources/bookingappointment.md) .</span><span class="sxs-lookup"><span data-stu-id="f55e6-126">In the request body, supply a JSON representation of [bookingAppointment](../resources/bookingappointment.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="f55e6-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="f55e6-127">Response</span></span>
<span data-ttu-id="f55e6-128">Успешно завершена, этот метод возвращает `201, Created` объект [bookingAppointment](../resources/bookingappointment.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f55e6-128">If successful, this method returns `201, Created` response code and [bookingAppointment](../resources/bookingappointment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f55e6-129">Пример</span><span class="sxs-lookup"><span data-stu-id="f55e6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f55e6-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="f55e6-130">Request</span></span>
<span data-ttu-id="f55e6-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f55e6-131">The following is an example of the request.</span></span> <span data-ttu-id="f55e6-132">В этом встречи не затрагивает резервирование конкретных сотрудников.</span><span class="sxs-lookup"><span data-stu-id="f55e6-132">This appointment does not involve booking specific staff members.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_bookingappointment_from_bookingbusiness"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingAppointment",
    "customerEmailAddress":"jordanm@contoso.com",
    "customerLocation":{
        "@odata.type":"#microsoft.graph.location",
        "address":{
            "@odata.type":"#microsoft.graph.physicalAddress",
            "city":"Buffalo",
            "countryOrRegion":"USA",
            "postalCode":"98052",
            "postOfficeBox":null,
            "state":"NY",
            "street":"123 First Avenue",
            "type@odata.type":"#microsoft.graph.physicalAddressType",
            "type":null
        },
        "coordinates":null,
        "displayName":"Customer",
        "locationEmailAddress":null,
        "locationType@odata.type":"#microsoft.graph.locationType",
        "locationType":null,
        "locationUri":null,
        "uniqueId":null,
        "uniqueIdType@odata.type":"#microsoft.graph.locationUniqueIdType",
        "uniqueIdType":null
    },
    "customerName":"Jordan Miller",
    "customerNotes":"Please be on time.",
    "customerPhone":"213-555-0199",
    "end":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-01T12:30:00.0000000+00:00",
        "timeZone":"UTC"
    },
    "invoiceAmount":10.0,
    "invoiceDate":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-01T12:30:00.0000000+00:00",
        "timeZone":"UTC"
    },
    "invoiceId":"1001",
    "invoiceStatus@odata.type":"#microsoft.graph.bookingInvoiceStatus",
    "invoiceStatus":"open",
    "invoiceUrl":"theInvoiceUrl",
    "optOutOfCustomerEmail":false,
    "postBuffer":"PT10M",
    "preBuffer":"PT5M",
    "price":10.0,
    "priceType@odata.type":"#microsoft.graph.bookingPriceType",
    "priceType":"fixedPrice",
    "reminders@odata.type":"#Collection(microsoft.graph.bookingReminder)",
    "reminders":[
        {
            "@odata.type":"#microsoft.graph.bookingReminder",
            "message":"This service is tomorrow",
            "offset":"P1D",
            "recipients@odata.type":"#microsoft.graph.bookingReminderRecipients",
            "recipients":"allAttendees"
        },
        {
            "@odata.type":"#microsoft.graph.bookingReminder",
            "message":"Please be available to enjoy your lunch service.",
            "offset":"PT1H",
            "recipients@odata.type":"#microsoft.graph.bookingReminderRecipients",
            "recipients":"customer"
        },
        {
            "@odata.type":"#microsoft.graph.bookingReminder",
            "message":"Please check traffic for next cater.",
            "offset":"PT2H",
            "recipients@odata.type":"#microsoft.graph.bookingReminderRecipients",
            "recipients":"staff"
        }
    ],
    "serviceId":"57da6774-a087-4d69-b0e6-6fb82c339976",
    "serviceLocation":{
        "@odata.type":"#microsoft.graph.location",
        "address":{
            "@odata.type":"#microsoft.graph.physicalAddress",
            "city":"Buffalo",
            "countryOrRegion":"USA",
            "postalCode":"98052",
            "postOfficeBox":null,
            "state":"NY",
            "street":"123 First Avenue",
            "type@odata.type":"#microsoft.graph.physicalAddressType",
            "type":null
        },
        "coordinates":null,
        "displayName":"Customer location",
        "locationEmailAddress":null,
        "locationType@odata.type":"#microsoft.graph.locationType",
        "locationType":null,
        "locationUri":null,
        "uniqueId":null,
        "uniqueIdType@odata.type":"#microsoft.graph.locationUniqueIdType",
        "uniqueIdType":null
    },
    "serviceName":"Catered bento",
    "serviceNotes":"Customer requires punctual service.",
    "start":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-01T12:00:00.0000000+00:00",
        "timeZone":"UTC"
    }
}
```
<span data-ttu-id="f55e6-133">В тексте запроса укажите представление JSON объекта [bookingAppointment](../resources/bookingappointment.md) .</span><span class="sxs-lookup"><span data-stu-id="f55e6-133">In the request body, supply a JSON representation of [bookingAppointment](../resources/bookingappointment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f55e6-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="f55e6-134">Response</span></span>
<span data-ttu-id="f55e6-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f55e6-135">The following is an example of the response.</span></span> <span data-ttu-id="f55e6-136">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="f55e6-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f55e6-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f55e6-137">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingAppointment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/appointments/$entity",
    "id": "AAMkADc7zF4J0AAA8v_KnAAA=",
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
        "dateTime": "2018-05-01T12:30:00.0000000Z",
        "timeZone": "UTC"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create bookingAppointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
