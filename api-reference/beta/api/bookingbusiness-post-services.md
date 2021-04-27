---
title: Создание bookingService
description: Создайте новую bookingService для указанного bookingbusiness.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 5f790cdc87cc7beedb85421cffec8dfb65aa56e3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047863"
---
# <a name="create-bookingservice"></a><span data-ttu-id="85ad8-103">Создание bookingService</span><span class="sxs-lookup"><span data-stu-id="85ad8-103">Create bookingService</span></span>

<span data-ttu-id="85ad8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85ad8-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85ad8-105">Создайте новую [bookingService](../resources/bookingservice.md) для указанного [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="85ad8-105">Create a new [bookingService](../resources/bookingservice.md) for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="85ad8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="85ad8-106">Permissions</span></span>
<span data-ttu-id="85ad8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85ad8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85ad8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85ad8-109">Permission type</span></span>      | <span data-ttu-id="85ad8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="85ad8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85ad8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85ad8-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="85ad8-112">Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="85ad8-112">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="85ad8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85ad8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85ad8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85ad8-114">Not supported.</span></span>   |
|<span data-ttu-id="85ad8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85ad8-115">Application</span></span> | <span data-ttu-id="85ad8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85ad8-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="85ad8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85ad8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/services

```
## <a name="request-headers"></a><span data-ttu-id="85ad8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85ad8-118">Request headers</span></span>
| <span data-ttu-id="85ad8-119">Имя</span><span class="sxs-lookup"><span data-stu-id="85ad8-119">Name</span></span>       | <span data-ttu-id="85ad8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="85ad8-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="85ad8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85ad8-121">Authorization</span></span>  | <span data-ttu-id="85ad8-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="85ad8-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="85ad8-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="85ad8-123">Request body</span></span>
<span data-ttu-id="85ad8-124">В теле запроса указать JSON-представление [объекта bookingService.](../resources/bookingservice.md)</span><span class="sxs-lookup"><span data-stu-id="85ad8-124">In the request body, supply a JSON representation of [bookingService](../resources/bookingservice.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="85ad8-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="85ad8-125">Response</span></span>
<span data-ttu-id="85ad8-126">В случае успешной работы этот метод возвращает код отклика и `201, Created` [объект bookingService](../resources/bookingservice.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="85ad8-126">If successful, this method returns `201, Created` response code and [bookingService](../resources/bookingservice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85ad8-127">Пример</span><span class="sxs-lookup"><span data-stu-id="85ad8-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="85ad8-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="85ad8-128">Request</span></span>
<span data-ttu-id="85ad8-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85ad8-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="85ad8-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="85ad8-130">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="85ad8-131">C#</span><span class="sxs-lookup"><span data-stu-id="85ad8-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bookingservice-from-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="85ad8-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85ad8-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bookingservice-from-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="85ad8-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85ad8-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bookingservice-from-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="85ad8-134">Java</span><span class="sxs-lookup"><span data-stu-id="85ad8-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-bookingservice-from-bookingbusiness-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="85ad8-135">В теле запроса указать JSON-представление [объекта bookingService.](../resources/bookingservice.md)</span><span class="sxs-lookup"><span data-stu-id="85ad8-135">In the request body, supply a JSON representation of [bookingService](../resources/bookingservice.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="85ad8-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="85ad8-136">Response</span></span>
<span data-ttu-id="85ad8-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="85ad8-137">The following is an example of the response.</span></span> <span data-ttu-id="85ad8-138">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="85ad8-138">Note: The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create bookingService",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


