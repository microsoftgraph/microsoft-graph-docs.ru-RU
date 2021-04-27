---
title: Представление календаря "Список резервирований"
description: Получите коллекцию объектов bookingAppointment для bookingBusiness, которая происходит в указанном диапазоне дат.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: d96e5b2f2c7f435a0ea8dcd39a4b58ae7657c222
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047912"
---
# <a name="list-bookings-calendarview"></a><span data-ttu-id="437ec-103">Представление календаря "Список резервирований"</span><span class="sxs-lookup"><span data-stu-id="437ec-103">List Bookings calendarView</span></span>

<span data-ttu-id="437ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="437ec-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="437ec-105">Получите коллекцию [объектов bookingAppointment](../resources/bookingappointment.md) для [bookingBusiness,](../resources/bookingbusiness.md)которая происходит в указанном диапазоне дат.</span><span class="sxs-lookup"><span data-stu-id="437ec-105">Get the collection of [bookingAppointment](../resources/bookingappointment.md) objects for a [bookingBusiness](../resources/bookingbusiness.md), that occurs in the specified date range.</span></span>

## <a name="permissions"></a><span data-ttu-id="437ec-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="437ec-106">Permissions</span></span>
<span data-ttu-id="437ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="437ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="437ec-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="437ec-109">Permission type</span></span>      | <span data-ttu-id="437ec-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="437ec-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="437ec-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="437ec-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="437ec-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="437ec-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="437ec-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="437ec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="437ec-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="437ec-114">Not supported.</span></span>   |
|<span data-ttu-id="437ec-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="437ec-115">Application</span></span> | <span data-ttu-id="437ec-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="437ec-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="437ec-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="437ec-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/calendarView?start={start-value}&end={end-value}
```

## <a name="query-parameters"></a><span data-ttu-id="437ec-118">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="437ec-118">Query parameters</span></span>

<span data-ttu-id="437ec-119">В URL-адресе запроса укажите перечисленные ниже обязательные параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="437ec-119">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="437ec-120">Параметр</span><span class="sxs-lookup"><span data-stu-id="437ec-120">Parameter</span></span>    | <span data-ttu-id="437ec-121">Тип</span><span class="sxs-lookup"><span data-stu-id="437ec-121">Type</span></span>   |<span data-ttu-id="437ec-122">Описание</span><span class="sxs-lookup"><span data-stu-id="437ec-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="437ec-123">начать</span><span class="sxs-lookup"><span data-stu-id="437ec-123">start</span></span>|<span data-ttu-id="437ec-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="437ec-124">DateTimeOffset</span></span>|<span data-ttu-id="437ec-125">Дата начала и время диапазона времени, представленного в формате ISO 8601, как UTC или смещение от UTC.</span><span class="sxs-lookup"><span data-stu-id="437ec-125">The start date and time of a time range, represented in ISO 8601 format, as UTC or an offset from UTC.</span></span> <span data-ttu-id="437ec-126">Например, полночь UTC 1 января 2018 г. будет выглядеть так: '2018-01-01T00:00:00Z', и то же время в PST будет выглядеть так: '2017-12-31T16:00:00-08:00'.</span><span class="sxs-lookup"><span data-stu-id="437ec-126">For example, midnight UTC on Jan 1, 2018 would look like this: '2018-01-01T00:00:00Z', and the same time in PST would look like this: '2017-12-31T16:00:00-08:00'.</span></span>|
|<span data-ttu-id="437ec-127">end</span><span class="sxs-lookup"><span data-stu-id="437ec-127">end</span></span>|<span data-ttu-id="437ec-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="437ec-128">DateTimeOffset</span></span>|<span data-ttu-id="437ec-129">Дата окончания и время диапазона времени, представленного в формате ISO 8601, как UTC или смещение от UTC.</span><span class="sxs-lookup"><span data-stu-id="437ec-129">The end date and time of a time range, represented in ISO 8601 format, as UTC or an offset from UTC.</span></span> <span data-ttu-id="437ec-130">Например, 1 января 2018 г. UTC в 3:00 будет выглядеть так: '2018-01-01T03:00:00Z', а в PST будет выглядеть так: '2017-12-31T19:00:00-08:00'.</span><span class="sxs-lookup"><span data-stu-id="437ec-130">For example, 3am UTC on Jan 1, 2018 would look like this: '2018-01-01T03:00:00Z', and the same time in PST would look like this: '2017-12-31T19:00:00-08:00'.</span></span>|

<span data-ttu-id="437ec-131">Значения и интерпретируются с помощью смещения часового пояса, указанного в соответствующих значениях, и не влияют на значение заглавного заглавного `start` `end` `Prefer: outlook.timezone` загона, если он присутствует.</span><span class="sxs-lookup"><span data-stu-id="437ec-131">The values of `start` and `end` are interpreted using the timezone offset specified in their corresponding values and are not impacted by the value of the `Prefer: outlook.timezone` header if present.</span></span>

<span data-ttu-id="437ec-132">Этот метод также поддерживает некоторые [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="437ec-132">This method also supports some of the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="437ec-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="437ec-133">Request headers</span></span>
| <span data-ttu-id="437ec-134">Имя</span><span class="sxs-lookup"><span data-stu-id="437ec-134">Name</span></span>       | <span data-ttu-id="437ec-135">Описание</span><span class="sxs-lookup"><span data-stu-id="437ec-135">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="437ec-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="437ec-136">Authorization</span></span>  | <span data-ttu-id="437ec-137">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="437ec-137">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="437ec-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="437ec-138">Request body</span></span>
<span data-ttu-id="437ec-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="437ec-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="437ec-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="437ec-140">Response</span></span>
<span data-ttu-id="437ec-141">В случае успешного выполнения этот метод возвращает код ответа и `200, OK` [объект коллекции bookingAppointment](../resources/bookingappointment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="437ec-141">If successful, this method returns `200, OK` response code and [bookingAppointment](../resources/bookingappointment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="437ec-142">Пример</span><span class="sxs-lookup"><span data-stu-id="437ec-142">Example</span></span>
<span data-ttu-id="437ec-143">Ниже приводится пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="437ec-143">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="437ec-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="437ec-144">Request</span></span>
<span data-ttu-id="437ec-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="437ec-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="437ec-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="437ec-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_getcalendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/calendarView?start=2018-04-30T00:00:00Z&end=2018-05-10T00:00:00Z
```
# <a name="c"></a>[<span data-ttu-id="437ec-147">C#</span><span class="sxs-lookup"><span data-stu-id="437ec-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingbusiness-getcalendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="437ec-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="437ec-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingbusiness-getcalendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="437ec-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="437ec-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingbusiness-getcalendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="437ec-150">Java</span><span class="sxs-lookup"><span data-stu-id="437ec-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/bookingbusiness-getcalendarview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="437ec-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="437ec-151">Response</span></span>
<span data-ttu-id="437ec-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="437ec-152">The following is an example of the response.</span></span> <span data-ttu-id="437ec-153">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="437ec-153">Note: The response object shown here might be shortened for readability.</span></span>
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
