---
title: Получение Букингсервице
description: Получение свойств и связей объекта Букингсервице в указанном букингбусинесс.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 8218365646f7ba4d7401362bf1b5365a47218821
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313235"
---
# <a name="get-bookingservice"></a><span data-ttu-id="9f3bd-103">Получение Букингсервице</span><span class="sxs-lookup"><span data-stu-id="9f3bd-103">Get bookingService</span></span>

<span data-ttu-id="9f3bd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f3bd-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f3bd-105">Получение свойств и связей объекта [букингсервице](../resources/bookingservice.md) в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="9f3bd-105">Get the properties and relationships of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="9f3bd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f3bd-106">Permissions</span></span>
<span data-ttu-id="9f3bd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f3bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f3bd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f3bd-109">Permission type</span></span>      | <span data-ttu-id="9f3bd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f3bd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f3bd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f3bd-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="9f3bd-112">Резервирования. Read. ALL, Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="9f3bd-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="9f3bd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f3bd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f3bd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f3bd-114">Not supported.</span></span>   |
|<span data-ttu-id="9f3bd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f3bd-115">Application</span></span> | <span data-ttu-id="9f3bd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f3bd-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="9f3bd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f3bd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9f3bd-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9f3bd-118">Optional query parameters</span></span>
<span data-ttu-id="9f3bd-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9f3bd-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9f3bd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f3bd-120">Request headers</span></span>
| <span data-ttu-id="9f3bd-121">Имя</span><span class="sxs-lookup"><span data-stu-id="9f3bd-121">Name</span></span>      |<span data-ttu-id="9f3bd-122">Описание</span><span class="sxs-lookup"><span data-stu-id="9f3bd-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9f3bd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f3bd-123">Authorization</span></span>  | <span data-ttu-id="9f3bd-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9f3bd-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f3bd-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f3bd-125">Request body</span></span>
<span data-ttu-id="9f3bd-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9f3bd-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9f3bd-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f3bd-127">Response</span></span>
<span data-ttu-id="9f3bd-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [букингсервице](../resources/bookingservice.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9f3bd-128">If successful, this method returns a `200 OK` response code and [bookingService](../resources/bookingservice.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9f3bd-129">Пример</span><span class="sxs-lookup"><span data-stu-id="9f3bd-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9f3bd-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f3bd-130">Request</span></span>
<span data-ttu-id="9f3bd-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f3bd-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9f3bd-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f3bd-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingservice"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
```
# <a name="c"></a>[<span data-ttu-id="9f3bd-133">C#</span><span class="sxs-lookup"><span data-stu-id="9f3bd-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingservice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9f3bd-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f3bd-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingservice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9f3bd-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9f3bd-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingservice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9f3bd-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f3bd-136">Response</span></span>
<span data-ttu-id="9f3bd-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9f3bd-137">The following is an example of the response.</span></span> <span data-ttu-id="9f3bd-138">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="9f3bd-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9f3bd-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f3bd-139">All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->