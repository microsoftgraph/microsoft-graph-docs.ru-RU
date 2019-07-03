---
title: Список служб
description: Получение списка объектов Букингсервице в указанном букингбусинесс.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 1dcc364348794b39996fdafdc2c7120096a92e18
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439261"
---
# <a name="list-services"></a><span data-ttu-id="4e68b-103">Список служб</span><span class="sxs-lookup"><span data-stu-id="4e68b-103">List services</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e68b-104">Получение списка объектов [букингсервице](../resources/bookingservice.md) в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="4e68b-104">Get a list of [bookingService](../resources/bookingservice.md) objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="4e68b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4e68b-105">Permissions</span></span>
<span data-ttu-id="4e68b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e68b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e68b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e68b-108">Permission type</span></span>      | <span data-ttu-id="4e68b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e68b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e68b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e68b-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="4e68b-111">Резервирования. Read. ALL, Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="4e68b-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="4e68b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e68b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e68b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e68b-113">Not supported.</span></span>   |
|<span data-ttu-id="4e68b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e68b-114">Application</span></span> | <span data-ttu-id="4e68b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e68b-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="4e68b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e68b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/services
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4e68b-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4e68b-117">Optional query parameters</span></span>
<span data-ttu-id="4e68b-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4e68b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4e68b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e68b-119">Request headers</span></span>
| <span data-ttu-id="4e68b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4e68b-120">Name</span></span>      |<span data-ttu-id="4e68b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4e68b-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4e68b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4e68b-122">Authorization</span></span>  | <span data-ttu-id="4e68b-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="4e68b-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e68b-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4e68b-124">Request body</span></span>
<span data-ttu-id="4e68b-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4e68b-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4e68b-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e68b-126">Response</span></span>
<span data-ttu-id="4e68b-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [букингсервице](../resources/bookingservice.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4e68b-127">If successful, this method returns a `200 OK` response code and collection of [bookingService](../resources/bookingservice.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4e68b-128">Пример</span><span class="sxs-lookup"><span data-stu-id="4e68b-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4e68b-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e68b-129">Request</span></span>
<span data-ttu-id="4e68b-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e68b-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4e68b-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e68b-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_services"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4e68b-132">C#</span><span class="sxs-lookup"><span data-stu-id="4e68b-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-services-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4e68b-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="4e68b-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-services-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4e68b-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4e68b-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-services-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4e68b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e68b-135">Response</span></span>
<span data-ttu-id="4e68b-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4e68b-136">The following is an example of the response.</span></span> <span data-ttu-id="4e68b-137">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="4e68b-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4e68b-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4e68b-138">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List services",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
