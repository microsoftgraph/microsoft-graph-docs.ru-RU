---
title: Получение Букингаппоинтмент
description: Получение свойств и связей объекта Букингаппоинтмент в указанном букингбусинесс.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 10b9fc68d179328592b1dfdbb58a93cab55f336c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988123"
---
# <a name="get-bookingappointment"></a><span data-ttu-id="5e059-103">Получение Букингаппоинтмент</span><span class="sxs-lookup"><span data-stu-id="5e059-103">Get bookingAppointment</span></span>

<span data-ttu-id="5e059-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e059-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e059-105">Получение свойств и связей объекта [букингаппоинтмент](../resources/bookingappointment.md) в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="5e059-105">Get the properties and relationships of a [bookingAppointment](../resources/bookingappointment.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="5e059-106">Свойства **Start** и **End** всегда возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="5e059-106">The **start** and **end** properties are always returned in UTC.</span></span>
## <a name="permissions"></a><span data-ttu-id="5e059-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5e059-107">Permissions</span></span>
<span data-ttu-id="5e059-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e059-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e059-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e059-110">Permission type</span></span>      | <span data-ttu-id="5e059-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e059-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e059-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e059-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="5e059-113">Резервирования. Read. ALL, Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="5e059-113">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="5e059-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e059-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e059-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e059-115">Not supported.</span></span>   |
|<span data-ttu-id="5e059-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5e059-116">Application</span></span> | <span data-ttu-id="5e059-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e059-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="5e059-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e059-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/appointments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5e059-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5e059-119">Optional query parameters</span></span>
<span data-ttu-id="5e059-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5e059-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5e059-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5e059-121">Request headers</span></span>
| <span data-ttu-id="5e059-122">Имя</span><span class="sxs-lookup"><span data-stu-id="5e059-122">Name</span></span>      |<span data-ttu-id="5e059-123">Описание</span><span class="sxs-lookup"><span data-stu-id="5e059-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5e059-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5e059-124">Authorization</span></span>  | <span data-ttu-id="5e059-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="5e059-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e059-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5e059-126">Request body</span></span>
<span data-ttu-id="5e059-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5e059-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5e059-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e059-128">Response</span></span>
<span data-ttu-id="5e059-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [букингаппоинтмент](../resources/bookingappointment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5e059-129">If successful, this method returns a `200 OK` response code and [bookingAppointment](../resources/bookingappointment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5e059-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5e059-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5e059-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e059-131">Request</span></span>
<span data-ttu-id="5e059-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e059-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5e059-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5e059-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingappointment"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKnAAA=
```
# <a name="c"></a>[<span data-ttu-id="5e059-134">C#</span><span class="sxs-lookup"><span data-stu-id="5e059-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingappointment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5e059-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e059-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingappointment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5e059-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5e059-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingappointment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5e059-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e059-137">Response</span></span>
<span data-ttu-id="5e059-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5e059-138">The following is an example of the response.</span></span> <span data-ttu-id="5e059-139">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="5e059-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5e059-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5e059-140">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get bookingAppointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


