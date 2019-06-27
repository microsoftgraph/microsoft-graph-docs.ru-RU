---
title: Получение Букингсервице
description: Получение свойств и связей объекта Букингсервице в указанном букингбусинесс.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 9d868a383701fca5519c1c19b3dfe5ef5c2e7398
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35257920"
---
# <a name="get-bookingservice"></a><span data-ttu-id="63201-103">Получение Букингсервице</span><span class="sxs-lookup"><span data-stu-id="63201-103">Get bookingService</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63201-104">Получение свойств и связей объекта [букингсервице](../resources/bookingservice.md) в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="63201-104">Get the properties and relationships of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="63201-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="63201-105">Permissions</span></span>
<span data-ttu-id="63201-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63201-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63201-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63201-108">Permission type</span></span>      | <span data-ttu-id="63201-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="63201-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63201-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63201-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="63201-111">Резервирования. Read. ALL, Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="63201-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="63201-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63201-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63201-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63201-113">Not supported.</span></span>   |
|<span data-ttu-id="63201-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="63201-114">Application</span></span> | <span data-ttu-id="63201-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63201-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="63201-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63201-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="63201-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="63201-117">Optional query parameters</span></span>
<span data-ttu-id="63201-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="63201-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="63201-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="63201-119">Request headers</span></span>
| <span data-ttu-id="63201-120">Имя</span><span class="sxs-lookup"><span data-stu-id="63201-120">Name</span></span>      |<span data-ttu-id="63201-121">Описание</span><span class="sxs-lookup"><span data-stu-id="63201-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="63201-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="63201-122">Authorization</span></span>  | <span data-ttu-id="63201-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="63201-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="63201-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="63201-124">Request body</span></span>
<span data-ttu-id="63201-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="63201-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="63201-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="63201-126">Response</span></span>
<span data-ttu-id="63201-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [букингсервице](../resources/bookingservice.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="63201-127">If successful, this method returns a `200 OK` response code and [bookingService](../resources/bookingservice.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="63201-128">Пример</span><span class="sxs-lookup"><span data-stu-id="63201-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="63201-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="63201-129">Request</span></span>
<span data-ttu-id="63201-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63201-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingservice"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
```
##### <a name="response"></a><span data-ttu-id="63201-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="63201-131">Response</span></span>
<span data-ttu-id="63201-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="63201-132">The following is an example of the response.</span></span> <span data-ttu-id="63201-133">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="63201-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="63201-134">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="63201-134">All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="63201-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="63201-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="63201-136">C#</span><span class="sxs-lookup"><span data-stu-id="63201-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_bookingservice-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="63201-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="63201-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_bookingservice-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="63201-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="63201-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_bookingservice-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/bookingservice-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingservice-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingservice-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
