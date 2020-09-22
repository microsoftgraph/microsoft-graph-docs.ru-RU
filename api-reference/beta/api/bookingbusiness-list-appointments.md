---
title: Список встреч
description: Получение списка объектов Букингаппоинтмент для указанного букингбусинесс.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 7de7f328d59ba20de77ec75cf5c6f16a0da2bc9e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988081"
---
# <a name="list-appointments"></a><span data-ttu-id="23079-103">Список встреч</span><span class="sxs-lookup"><span data-stu-id="23079-103">List appointments</span></span>

<span data-ttu-id="23079-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23079-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23079-105">Получение списка объектов [букингаппоинтмент](../resources/bookingappointment.md) для указанного [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="23079-105">Get a list of [bookingAppointment](../resources/bookingappointment.md) objects for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="23079-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23079-106">Permissions</span></span>
<span data-ttu-id="23079-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23079-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23079-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23079-109">Permission type</span></span>      | <span data-ttu-id="23079-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23079-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23079-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23079-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="23079-112">Резервирования. Read. ALL, Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="23079-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="23079-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23079-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23079-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23079-114">Not supported.</span></span>   |
|<span data-ttu-id="23079-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23079-115">Application</span></span> | <span data-ttu-id="23079-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23079-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="23079-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23079-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/appointments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="23079-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="23079-118">Optional query parameters</span></span>
<span data-ttu-id="23079-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="23079-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="23079-120">Чтобы получить набор встреч из зарезервированных дел в диапазоне дат, вместо этого `$filter` [получите calendarView](bookingbusiness-list-calendarview.md) для этого диапазона дат.</span><span class="sxs-lookup"><span data-stu-id="23079-120">To get the set of appointments of a Bookings business within a date range, instead of `$filter`, [get the calendarView](bookingbusiness-list-calendarview.md) for that date range.</span></span>

## <a name="request-headers"></a><span data-ttu-id="23079-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23079-121">Request headers</span></span>
| <span data-ttu-id="23079-122">Имя</span><span class="sxs-lookup"><span data-stu-id="23079-122">Name</span></span>      |<span data-ttu-id="23079-123">Описание</span><span class="sxs-lookup"><span data-stu-id="23079-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="23079-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23079-124">Authorization</span></span>  | <span data-ttu-id="23079-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="23079-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="23079-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="23079-126">Request body</span></span>
<span data-ttu-id="23079-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="23079-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="23079-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="23079-128">Response</span></span>
<span data-ttu-id="23079-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [букингаппоинтмент](../resources/bookingappointment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="23079-129">If successful, this method returns a `200 OK` response code and collection of [bookingAppointment](../resources/bookingappointment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="23079-130">Пример</span><span class="sxs-lookup"><span data-stu-id="23079-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="23079-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="23079-131">Request</span></span>
<span data-ttu-id="23079-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23079-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="23079-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="23079-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_appointments"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments
```
# <a name="c"></a>[<span data-ttu-id="23079-134">C#</span><span class="sxs-lookup"><span data-stu-id="23079-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-appointments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23079-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23079-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-appointments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23079-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23079-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-appointments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="23079-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="23079-137">Response</span></span>
<span data-ttu-id="23079-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23079-138">The following is an example of the response.</span></span> <span data-ttu-id="23079-139">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="23079-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="23079-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23079-140">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List appointments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


