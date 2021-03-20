---
title: Службы списка
description: Получите список объектов bookingService в указанном bookingbusiness.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: b0d27418d73e16b11f27c253a6dfd57dcd861974
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942458"
---
# <a name="list-services"></a><span data-ttu-id="a365f-103">Службы списка</span><span class="sxs-lookup"><span data-stu-id="a365f-103">List services</span></span>

<span data-ttu-id="a365f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a365f-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a365f-105">Получите список объектов [bookingService](../resources/bookingservice.md) в указанном [bookingbusiness.](../resources/bookingbusiness.md)</span><span class="sxs-lookup"><span data-stu-id="a365f-105">Get a list of [bookingService](../resources/bookingservice.md) objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="a365f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a365f-106">Permissions</span></span>
<span data-ttu-id="a365f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a365f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a365f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a365f-109">Permission type</span></span>      | <span data-ttu-id="a365f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a365f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a365f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a365f-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="a365f-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="a365f-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="a365f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a365f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a365f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a365f-114">Not supported.</span></span>   |
|<span data-ttu-id="a365f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a365f-115">Application</span></span> | <span data-ttu-id="a365f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a365f-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="a365f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a365f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/services
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a365f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a365f-118">Optional query parameters</span></span>
<span data-ttu-id="a365f-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a365f-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a365f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a365f-120">Request headers</span></span>
| <span data-ttu-id="a365f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="a365f-121">Name</span></span>      |<span data-ttu-id="a365f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a365f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a365f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a365f-123">Authorization</span></span>  | <span data-ttu-id="a365f-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="a365f-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="a365f-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a365f-125">Request body</span></span>
<span data-ttu-id="a365f-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a365f-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a365f-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="a365f-127">Response</span></span>
<span data-ttu-id="a365f-128">В случае успешной работы этот метод возвращает код отклика и `200 OK` коллекцию объектов [bookingService](../resources/bookingservice.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a365f-128">If successful, this method returns a `200 OK` response code and collection of [bookingService](../resources/bookingservice.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a365f-129">Пример</span><span class="sxs-lookup"><span data-stu-id="a365f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a365f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a365f-130">Request</span></span>
<span data-ttu-id="a365f-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a365f-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a365f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a365f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_services_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services
```
# <a name="c"></a>[<span data-ttu-id="a365f-133">C#</span><span class="sxs-lookup"><span data-stu-id="a365f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-services-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a365f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a365f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-services-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a365f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a365f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-services-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a365f-136">Java</span><span class="sxs-lookup"><span data-stu-id="a365f-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-services-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a365f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a365f-137">Response</span></span>
<span data-ttu-id="a365f-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a365f-138">The following is an example of the response.</span></span> <span data-ttu-id="a365f-139">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="a365f-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a365f-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a365f-140">All of the properties will be returned from an actual call.</span></span>
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
