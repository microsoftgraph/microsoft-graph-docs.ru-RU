---
title: Получение bookingService
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: 25ced555f4962ef073f6f01c4eed4767ad1c9e01
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075759"
---
# <a name="get-bookingservice"></a><span data-ttu-id="da100-104">Получение bookingService</span><span class="sxs-lookup"><span data-stu-id="da100-104">Get bookingService</span></span>

 > <span data-ttu-id="da100-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="da100-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da100-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da100-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="da100-107">Получите свойства и связи объекта [bookingService](../resources/bookingservice.md) в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="da100-107">Get the properties and relationships of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="da100-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="da100-108">Permissions</span></span>
<span data-ttu-id="da100-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da100-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da100-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da100-111">Permission type</span></span>      | <span data-ttu-id="da100-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="da100-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da100-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da100-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="da100-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="da100-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="da100-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da100-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da100-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da100-116">Not supported.</span></span>   |
|<span data-ttu-id="da100-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da100-117">Application</span></span> | <span data-ttu-id="da100-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da100-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="da100-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da100-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="da100-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="da100-120">Optional query parameters</span></span>
<span data-ttu-id="da100-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="da100-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="da100-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da100-122">Request headers</span></span>
| <span data-ttu-id="da100-123">Имя</span><span class="sxs-lookup"><span data-stu-id="da100-123">Name</span></span>      |<span data-ttu-id="da100-124">Описание</span><span class="sxs-lookup"><span data-stu-id="da100-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="da100-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="da100-125">Authorization</span></span>  | <span data-ttu-id="da100-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="da100-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="da100-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="da100-127">Request body</span></span>
<span data-ttu-id="da100-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="da100-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="da100-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="da100-129">Response</span></span>
<span data-ttu-id="da100-130">Успешно завершена, этот метод возвращает `200 OK` объект [bookingService](../resources/bookingservice.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="da100-130">If successful, this method returns a `200 OK` response code and [bookingService](../resources/bookingservice.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="da100-131">Пример</span><span class="sxs-lookup"><span data-stu-id="da100-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da100-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="da100-132">Request</span></span>
<span data-ttu-id="da100-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da100-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingservice"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
```
##### <a name="response"></a><span data-ttu-id="da100-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="da100-134">Response</span></span>
<span data-ttu-id="da100-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="da100-135">The following is an example of the response.</span></span> <span data-ttu-id="da100-136">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="da100-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="da100-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="da100-137">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get bookingService",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->