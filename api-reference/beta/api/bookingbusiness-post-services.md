---
title: Создание bookingService
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: 73e38c0abfeacb43d3ac7f4e28345ac56becb667
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814296"
---
# <a name="create-bookingservice"></a><span data-ttu-id="11acf-104">Создание bookingService</span><span class="sxs-lookup"><span data-stu-id="11acf-104">Create bookingService</span></span>

 > <span data-ttu-id="11acf-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="11acf-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="11acf-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11acf-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="11acf-107">Создание нового [bookingService](../resources/bookingservice.md) для указанного [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="11acf-107">Create a new [bookingService](../resources/bookingservice.md) for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="11acf-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="11acf-108">Permissions</span></span>
<span data-ttu-id="11acf-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11acf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11acf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11acf-111">Permission type</span></span>      | <span data-ttu-id="11acf-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="11acf-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11acf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11acf-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="11acf-114">Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="11acf-114">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="11acf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11acf-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11acf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11acf-116">Not supported.</span></span>   |
|<span data-ttu-id="11acf-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="11acf-117">Application</span></span> | <span data-ttu-id="11acf-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11acf-118">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="11acf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11acf-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/services

```
## <a name="request-headers"></a><span data-ttu-id="11acf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="11acf-120">Request headers</span></span>
| <span data-ttu-id="11acf-121">Имя</span><span class="sxs-lookup"><span data-stu-id="11acf-121">Name</span></span>       | <span data-ttu-id="11acf-122">Описание</span><span class="sxs-lookup"><span data-stu-id="11acf-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="11acf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="11acf-123">Authorization</span></span>  | <span data-ttu-id="11acf-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="11acf-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="11acf-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="11acf-125">Request body</span></span>
<span data-ttu-id="11acf-126">В тексте запроса укажите представление JSON объекта [bookingService](../resources/bookingservice.md) .</span><span class="sxs-lookup"><span data-stu-id="11acf-126">In the request body, supply a JSON representation of [bookingService](../resources/bookingservice.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="11acf-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="11acf-127">Response</span></span>
<span data-ttu-id="11acf-128">Успешно завершена, этот метод возвращает `201, Created` объект [bookingService](../resources/bookingservice.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="11acf-128">If successful, this method returns `201, Created` response code and [bookingService](../resources/bookingservice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11acf-129">Пример</span><span class="sxs-lookup"><span data-stu-id="11acf-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="11acf-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="11acf-130">Request</span></span>
<span data-ttu-id="11acf-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="11acf-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_bookingservice_from_bookingbusiness"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingService",
    "defaultDuration":"PT1H30M",
    "defaultLocation":{
        "@odata.type":"#microsoft.graph.location",
        "address":{
            "@odata.type":"#microsoft.graph.physicalAddress",
            "city":"Buffalo",
            "countryOrRegion":"USA",
            "postalCode":"98052",
            "postOfficeBox":null,
            "state":"NY",
            "street":"4567 First Street",
            "type@odata.type":"#microsoft.graph.physicalAddressType",
            "type":null
        },
        "coordinates":null,
        "displayName":"Contoso Lunch Delivery",
        "locationEmailAddress":null,
        "locationType@odata.type":"#microsoft.graph.locationType",
        "locationType":null,
        "locationUri":null,
        "uniqueId":null,
        "uniqueIdType@odata.type":"#microsoft.graph.locationUniqueIdType",
        "uniqueIdType":null
    },
    "defaultPrice":10.0,
    "defaultPriceType@odata.type":"#microsoft.graph.bookingPriceType",
    "defaultPriceType":"fixedPrice",
    "defaultReminders@odata.type":"#Collection(microsoft.graph.bookingReminder)",
    "defaultReminders":[
        {
            "@odata.type":"#microsoft.graph.bookingReminder",
            "message":"Please be reminded that this service is tomorrow.",
            "offset":"P1D",
            "recipients@odata.type":"#microsoft.graph.bookingReminderRecipients",
            "recipients":"allAttendees"
        }
    ],
    "description":"Individual bento box lunch delivery",
    "displayName":"Bento",
    "isHiddenFromCustomers":false,
    "notes":"Home-cooked special",
    "postBuffer":"PT10M",
    "preBuffer":"PT5M",
    "schedulingPolicy":{
        "@odata.type":"#microsoft.graph.bookingSchedulingPolicy",
        "allowStaffSelection":true,
        "maximumAdvance":"P10D",
        "minimumLeadTime":"PT10H",
        "sendConfirmationsToOwner":true,
        "timeSlotInterval":"PT1H"
    },
    "staffMemberIds@odata.type":"#Collection(String)",
    "staffMemberIds":[
        "d90d1e8c-5cfe-48cf-a2d5-966267375b6a",
        "2f5f8794-0b29-45b5-b56a-2eb5ff7aa880"
    ]
}
```
<span data-ttu-id="11acf-132">В тексте запроса укажите представление JSON объекта [bookingService](../resources/bookingservice.md) .</span><span class="sxs-lookup"><span data-stu-id="11acf-132">In the request body, supply a JSON representation of [bookingService](../resources/bookingservice.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="11acf-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="11acf-133">Response</span></span>
<span data-ttu-id="11acf-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="11acf-134">The following is an example of the response.</span></span> <span data-ttu-id="11acf-135">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="11acf-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="11acf-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="11acf-136">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingService"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/services/$entity",
    "id": "57da6774-a087-4d69-b0e6-6fb82c339976",
    "displayName": "Bento",
    "defaultDuration": "PT1H30M",
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
  "description": "Create bookingService",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
