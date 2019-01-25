---
title: Получение bookingService
description: Получите свойства и связи объекта bookingService в указанном bookingbusiness.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: d3a552f4724bdf388152ef2d2538507f53692e10
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509492"
---
# <a name="get-bookingservice"></a><span data-ttu-id="3a62b-103">Получение bookingService</span><span class="sxs-lookup"><span data-stu-id="3a62b-103">Get bookingService</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a62b-104">Получите свойства и связи объекта [bookingService](../resources/bookingservice.md) в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="3a62b-104">Get the properties and relationships of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="3a62b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a62b-105">Permissions</span></span>
<span data-ttu-id="3a62b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a62b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a62b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a62b-108">Permission type</span></span>      | <span data-ttu-id="3a62b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a62b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a62b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a62b-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="3a62b-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="3a62b-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="3a62b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a62b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a62b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a62b-113">Not supported.</span></span>   |
|<span data-ttu-id="3a62b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a62b-114">Application</span></span> | <span data-ttu-id="3a62b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a62b-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="3a62b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a62b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3a62b-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3a62b-117">Optional query parameters</span></span>
<span data-ttu-id="3a62b-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3a62b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a62b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a62b-119">Request headers</span></span>
| <span data-ttu-id="3a62b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="3a62b-120">Name</span></span>      |<span data-ttu-id="3a62b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3a62b-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3a62b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a62b-122">Authorization</span></span>  | <span data-ttu-id="3a62b-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3a62b-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a62b-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a62b-124">Request body</span></span>
<span data-ttu-id="3a62b-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3a62b-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3a62b-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a62b-126">Response</span></span>
<span data-ttu-id="3a62b-127">Успешно завершена, этот метод возвращает `200 OK` объект [bookingService](../resources/bookingservice.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3a62b-127">If successful, this method returns a `200 OK` response code and [bookingService](../resources/bookingservice.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3a62b-128">Пример</span><span class="sxs-lookup"><span data-stu-id="3a62b-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a62b-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a62b-129">Request</span></span>
<span data-ttu-id="3a62b-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a62b-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingservice"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
```
##### <a name="response"></a><span data-ttu-id="3a62b-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a62b-131">Response</span></span>
<span data-ttu-id="3a62b-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3a62b-132">The following is an example of the response.</span></span> <span data-ttu-id="3a62b-133">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="3a62b-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3a62b-134">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3a62b-134">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingService"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/services/$entity",
    "id": "57da6774-a087-4d69-b0e6-6fb82c339976",
    "displayName": "Bento",
    "defaultDuration": "PT30M",
    "defaultPrice": 10,
    "defaultPriceType": "fixedPrice",
    "description": "Individual bento box lunch delivery",
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
    "defaultReminders": [
        {
            "offset": "P1D",
            "recipients": "allAttendees",
            "message": "Please be reminded that this service is tomorrow."
        }
    ],
    "schedulingPolicy": {
        "timeSlotInterval": "PT1H",
        "minimumLeadTime": "PT10H",
        "maximumAdvance": "P10D",
        "sendConfirmationsToOwner": true,
        "allowStaffSelection": true
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get bookingService",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingservice-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
