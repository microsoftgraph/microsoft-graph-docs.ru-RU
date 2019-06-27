---
title: Список встреч
description: Получение списка объектов Букингаппоинтмент для указанного букингбусинесс.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 2f2f1b20506cfb6f01b81a1d259551135e227b88
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258179"
---
# <a name="list-appointments"></a><span data-ttu-id="788c6-103">Список встреч</span><span class="sxs-lookup"><span data-stu-id="788c6-103">List appointments</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="788c6-104">Получение списка объектов [букингаппоинтмент](../resources/bookingappointment.md) для указанного [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="788c6-104">Get a list of [bookingAppointment](../resources/bookingappointment.md) objects for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="788c6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="788c6-105">Permissions</span></span>
<span data-ttu-id="788c6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="788c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="788c6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="788c6-108">Permission type</span></span>      | <span data-ttu-id="788c6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="788c6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="788c6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="788c6-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="788c6-111">Резервирования. Read. ALL, Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="788c6-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="788c6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="788c6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="788c6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="788c6-113">Not supported.</span></span>   |
|<span data-ttu-id="788c6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="788c6-114">Application</span></span> | <span data-ttu-id="788c6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="788c6-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="788c6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="788c6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/appointments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="788c6-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="788c6-117">Optional query parameters</span></span>
<span data-ttu-id="788c6-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="788c6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="788c6-119">Чтобы получить набор встреч из зарезервированных дел в диапазоне дат, вместо `$filter`этого [получите calendarView](bookingbusiness-list-calendarview.md) для этого диапазона дат.</span><span class="sxs-lookup"><span data-stu-id="788c6-119">To get the set of appointments of a Bookings business within a date range, instead of `$filter`, [get the calendarView](bookingbusiness-list-calendarview.md) for that date range.</span></span>

## <a name="request-headers"></a><span data-ttu-id="788c6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="788c6-120">Request headers</span></span>
| <span data-ttu-id="788c6-121">Имя</span><span class="sxs-lookup"><span data-stu-id="788c6-121">Name</span></span>      |<span data-ttu-id="788c6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="788c6-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="788c6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="788c6-123">Authorization</span></span>  | <span data-ttu-id="788c6-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="788c6-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="788c6-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="788c6-125">Request body</span></span>
<span data-ttu-id="788c6-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="788c6-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="788c6-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="788c6-127">Response</span></span>
<span data-ttu-id="788c6-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [букингаппоинтмент](../resources/bookingappointment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="788c6-128">If successful, this method returns a `200 OK` response code and collection of [bookingAppointment](../resources/bookingappointment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="788c6-129">Пример</span><span class="sxs-lookup"><span data-stu-id="788c6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="788c6-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="788c6-130">Request</span></span>
<span data-ttu-id="788c6-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="788c6-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_appointments"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments
```
##### <a name="response"></a><span data-ttu-id="788c6-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="788c6-132">Response</span></span>
<span data-ttu-id="788c6-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="788c6-133">The following is an example of the response.</span></span> <span data-ttu-id="788c6-134">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="788c6-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="788c6-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="788c6-135">All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="788c6-136">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="788c6-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="788c6-137">C#</span><span class="sxs-lookup"><span data-stu-id="788c6-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_appointments-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="788c6-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="788c6-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_appointments-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="788c6-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="788c6-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_appointments-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List appointments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-list-appointments.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingbusiness-list-appointments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-list-appointments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
