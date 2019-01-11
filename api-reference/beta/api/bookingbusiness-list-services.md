---
title: Список служб
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: ceb26fe3e628db30860620871d495e98e80b711d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829654"
---
# <a name="list-services"></a><span data-ttu-id="619f9-104">Список служб</span><span class="sxs-lookup"><span data-stu-id="619f9-104">List services</span></span>

 > <span data-ttu-id="619f9-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="619f9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="619f9-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="619f9-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="619f9-107">Получите список объектов [bookingService](../resources/bookingservice.md) в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="619f9-107">Get a list of [bookingService](../resources/bookingservice.md) objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="619f9-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="619f9-108">Permissions</span></span>
<span data-ttu-id="619f9-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="619f9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="619f9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="619f9-111">Permission type</span></span>      | <span data-ttu-id="619f9-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="619f9-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="619f9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="619f9-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="619f9-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="619f9-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="619f9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="619f9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="619f9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="619f9-116">Not supported.</span></span>   |
|<span data-ttu-id="619f9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="619f9-117">Application</span></span> | <span data-ttu-id="619f9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="619f9-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="619f9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="619f9-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/services
```
## <a name="optional-query-parameters"></a><span data-ttu-id="619f9-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="619f9-120">Optional query parameters</span></span>
<span data-ttu-id="619f9-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="619f9-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="619f9-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="619f9-122">Request headers</span></span>
| <span data-ttu-id="619f9-123">Имя</span><span class="sxs-lookup"><span data-stu-id="619f9-123">Name</span></span>      |<span data-ttu-id="619f9-124">Описание</span><span class="sxs-lookup"><span data-stu-id="619f9-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="619f9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="619f9-125">Authorization</span></span>  | <span data-ttu-id="619f9-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="619f9-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="619f9-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="619f9-127">Request body</span></span>
<span data-ttu-id="619f9-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="619f9-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="619f9-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="619f9-129">Response</span></span>
<span data-ttu-id="619f9-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [bookingService](../resources/bookingservice.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="619f9-130">If successful, this method returns a `200 OK` response code and collection of [bookingService](../resources/bookingservice.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="619f9-131">Пример</span><span class="sxs-lookup"><span data-stu-id="619f9-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="619f9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="619f9-132">Request</span></span>
<span data-ttu-id="619f9-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="619f9-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_services"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services
```
##### <a name="response"></a><span data-ttu-id="619f9-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="619f9-134">Response</span></span>
<span data-ttu-id="619f9-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="619f9-135">The following is an example of the response.</span></span> <span data-ttu-id="619f9-136">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="619f9-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="619f9-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="619f9-137">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingService",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/services",
    "value": [
        {
            "id": "f9b9121f-aed7-4c8c-bb3a-a1796a0b0b2d",
            "displayName": "Initial service",
            "defaultDuration": "PT10M",
            "defaultPrice": 0,
            "defaultPriceType": "notSet",
            "description": "Not sure how to choose? Let us introduce you to our traditional family recipes.",
            "isHiddenFromCustomers": false,
            "notes": "This is where you can add notes about this service that only you and your staff see.",
            "preBuffer": "PT0S",
            "postBuffer": "PT0S",
            "staffMemberIds": [],
            "schedulingPolicy": null,
            "defaultLocation": {
                "displayName": "Contoso Lunch Delivery",
                "locationEmailAddress": null,
                "locationUri": "",
                "locationType": null,
                "uniqueId": null,
                "uniqueIdType": null,
                "address": {
                    "type": "home",
                    "postOfficeBox": "",
                    "street": "4567 First Street",
                    "city": "Buffalo",
                    "state": "NY",
                    "countryOrRegion": "USA",
                    "postalCode": "98052"
                },
                "coordinates": {
                    "altitude": null,
                    "latitude": null,
                    "longitude": null,
                    "accuracy": null,
                    "altitudeAccuracy": null
                }
            },
            "defaultReminders": []
        },
        {
            "id": "57da6774-a087-4d69-b0e6-6fb82c339976",
            "displayName": "Catered bento",
            "defaultDuration": "PT30M",
            "defaultPrice": 10,
            "defaultPriceType": "fixedPrice",
            "description": "Catered individual bento box lunch",
            "isHiddenFromCustomers": false,
            "notes": "Home-cooked special",
            "preBuffer": "PT5M",
            "postBuffer": "PT10M",
            "staffMemberIds": [],
            "defaultLocation": {
                "displayName": "Contoso Lunch Delivery",
                "locationEmailAddress": null,
                "locationUri": "",
                "locationType": null,
                "uniqueId": null,
                "uniqueIdType": null,
                "address": {
                    "type": "home",
                    "postOfficeBox": "",
                    "street": "4567 First Street",
                    "city": "Buffalo",
                    "state": "NY",
                    "countryOrRegion": "USA",
                    "postalCode": "98052"
                },
                "coordinates": {
                    "altitude": null,
                    "latitude": null,
                    "longitude": null,
                    "accuracy": null,
                    "altitudeAccuracy": null
                }
            },
            "defaultReminders": [],
            "schedulingPolicy": {
                "timeSlotInterval": "PT1H",
                "minimumLeadTime": "PT10H",
                "maximumAdvance": "P10D",
                "sendConfirmationsToOwner": true,
                "allowStaffSelection": true
            }
        },
        {
            "id": "635a7b7c-4230-4d3b-a42b-698e89927528",
            "displayName": "Kaiseki",
            "defaultDuration": "PT1H30M",
            "defaultPrice": 30,
            "defaultPriceType": "fixedPrice",
            "description": "Individual kaiseki lunch delivery",
            "isHiddenFromCustomers": false,
            "notes": "Home-cooked special",
            "preBuffer": "PT5M",
            "postBuffer": "PT10M",
            "staffMemberIds": [],
            "defaultLocation": {
                "displayName": "Contoso Lunch Delivery",
                "locationEmailAddress": null,
                "locationUri": "",
                "locationType": null,
                "uniqueId": null,
                "uniqueIdType": null,
                "address": {
                    "type": "home",
                    "postOfficeBox": "",
                    "street": "4567 First Street",
                    "city": "Buffalo",
                    "state": "NY",
                    "countryOrRegion": "USA",
                    "postalCode": "98052"
                },
                "coordinates": {
                    "altitude": null,
                    "latitude": null,
                    "longitude": null,
                    "accuracy": null,
                    "altitudeAccuracy": null
                }
            },
            "defaultReminders": [],
            "schedulingPolicy": {
                "timeSlotInterval": "PT1H",
                "minimumLeadTime": "PT10H",
                "maximumAdvance": "P10D",
                "sendConfirmationsToOwner": true,
                "allowStaffSelection": true
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List services",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
