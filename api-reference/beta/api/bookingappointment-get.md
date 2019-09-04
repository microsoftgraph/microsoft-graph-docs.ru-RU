---
title: Получение Букингаппоинтмент
description: Получение свойств и связей объекта Букингаппоинтмент в указанном букингбусинесс.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: d8b9734249f7b728cc0a9b5582a730fff1539b9d
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718928"
---
# <a name="get-bookingappointment"></a><span data-ttu-id="16d66-103">Получение Букингаппоинтмент</span><span class="sxs-lookup"><span data-stu-id="16d66-103">Get bookingAppointment</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16d66-104">Получение свойств и связей объекта [букингаппоинтмент](../resources/bookingappointment.md) в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="16d66-104">Get the properties and relationships of a [bookingAppointment](../resources/bookingappointment.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="16d66-105">Свойства **Start** и **End** всегда возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="16d66-105">The **start** and **end** properties are always returned in UTC.</span></span>
## <a name="permissions"></a><span data-ttu-id="16d66-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16d66-106">Permissions</span></span>
<span data-ttu-id="16d66-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16d66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16d66-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16d66-109">Permission type</span></span>      | <span data-ttu-id="16d66-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16d66-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16d66-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16d66-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="16d66-112">Резервирования. Read. ALL, Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="16d66-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="16d66-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16d66-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16d66-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16d66-114">Not supported.</span></span>   |
|<span data-ttu-id="16d66-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16d66-115">Application</span></span> | <span data-ttu-id="16d66-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16d66-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="16d66-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16d66-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/appointments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="16d66-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="16d66-118">Optional query parameters</span></span>
<span data-ttu-id="16d66-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="16d66-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="16d66-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16d66-120">Request headers</span></span>
| <span data-ttu-id="16d66-121">Имя</span><span class="sxs-lookup"><span data-stu-id="16d66-121">Name</span></span>      |<span data-ttu-id="16d66-122">Описание</span><span class="sxs-lookup"><span data-stu-id="16d66-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="16d66-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="16d66-123">Authorization</span></span>  | <span data-ttu-id="16d66-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="16d66-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="16d66-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16d66-125">Request body</span></span>
<span data-ttu-id="16d66-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="16d66-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="16d66-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="16d66-127">Response</span></span>
<span data-ttu-id="16d66-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [букингаппоинтмент](../resources/bookingappointment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="16d66-128">If successful, this method returns a `200 OK` response code and [bookingAppointment](../resources/bookingappointment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="16d66-129">Пример</span><span class="sxs-lookup"><span data-stu-id="16d66-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="16d66-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="16d66-130">Request</span></span>
<span data-ttu-id="16d66-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16d66-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="16d66-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="16d66-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingappointment"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKnAAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="16d66-133">C#</span><span class="sxs-lookup"><span data-stu-id="16d66-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingappointment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="16d66-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16d66-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingappointment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="16d66-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="16d66-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingappointment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="16d66-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="16d66-136">Response</span></span>
<span data-ttu-id="16d66-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="16d66-137">The following is an example of the response.</span></span> <span data-ttu-id="16d66-138">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="16d66-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="16d66-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16d66-139">All of the properties will be returned from an actual call.</span></span>
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
