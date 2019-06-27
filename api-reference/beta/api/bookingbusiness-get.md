---
title: Получение Букингбусинесс
description: Получение свойств и связей объекта Букингбусинесс.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 69dfb30f0a372eba6f3aa46ccd1c9b30fd25aff3
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258260"
---
# <a name="get-bookingbusiness"></a><span data-ttu-id="242f1-103">Получение Букингбусинесс</span><span class="sxs-lookup"><span data-stu-id="242f1-103">Get bookingBusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="242f1-104">Получение свойств и связей объекта [букингбусинесс](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="242f1-104">Get the properties and relationships of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="242f1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="242f1-105">Permissions</span></span>
<span data-ttu-id="242f1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="242f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="242f1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="242f1-108">Permission type</span></span>      | <span data-ttu-id="242f1-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="242f1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="242f1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="242f1-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="242f1-111">Резервирования. Read. ALL, Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="242f1-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="242f1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="242f1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="242f1-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="242f1-113">Not supported.</span></span>   |
|<span data-ttu-id="242f1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="242f1-114">Application</span></span> | <span data-ttu-id="242f1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="242f1-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="242f1-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="242f1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="242f1-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="242f1-117">Optional query parameters</span></span>
<span data-ttu-id="242f1-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="242f1-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="242f1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="242f1-119">Request headers</span></span>
| <span data-ttu-id="242f1-120">Имя</span><span class="sxs-lookup"><span data-stu-id="242f1-120">Name</span></span>      |<span data-ttu-id="242f1-121">Описание</span><span class="sxs-lookup"><span data-stu-id="242f1-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="242f1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="242f1-122">Authorization</span></span>  | <span data-ttu-id="242f1-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="242f1-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="242f1-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="242f1-124">Request body</span></span>
<span data-ttu-id="242f1-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="242f1-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="242f1-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="242f1-126">Response</span></span>
<span data-ttu-id="242f1-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [букингбусинесс](../resources/bookingbusiness.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="242f1-127">If successful, this method returns a `200 OK` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="242f1-128">Пример</span><span class="sxs-lookup"><span data-stu-id="242f1-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="242f1-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="242f1-129">Request</span></span>
<span data-ttu-id="242f1-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="242f1-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingbusiness"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Fabrikam@M365B489948.onmicrosoft.com
```
##### <a name="response"></a><span data-ttu-id="242f1-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="242f1-131">Response</span></span>
<span data-ttu-id="242f1-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="242f1-132">The following is an example of the response.</span></span> <span data-ttu-id="242f1-133">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="242f1-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="242f1-134">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="242f1-134">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingBusiness"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses/$entity",
    "id":"Fabrikam@M365B489948.onmicrosoft.com",
    "displayName":"Fabrikam",
    "businessType":"",
    "phone":"206-555-0100",
    "email":"manager@fabrikam.com",
    "webSiteUrl":"https://www.fabrikam.com/",
    "defaultCurrencyIso":"USD",
    "isPublished":false,
    "publicUrl":null,
    "address":{
        "type":"home",
        "postOfficeBox":"",
        "street":"4567 Main Street",
        "city":"Buffalo",
        "state":"NY",
        "countryOrRegion":"USA",
        "postalCode":"98052"
    },
    "businessHours":[
        {
            "day":"monday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"tuesday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"wednesday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"thursday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"friday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"saturday",
            "timeSlots":[

            ]
        },
        {
            "day":"sunday",
            "timeSlots":[

            ]
        }
    ],
    "schedulingPolicy":{
        "timeSlotInterval":"PT30M",
        "minimumLeadTime":"P1D",
        "maximumAdvance":"P365D",
        "sendConfirmationsToOwner":true,
        "allowStaffSelection":true
    }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="242f1-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="242f1-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="242f1-136">C#</span><span class="sxs-lookup"><span data-stu-id="242f1-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_bookingbusiness-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="242f1-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="242f1-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_bookingbusiness-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="242f1-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="242f1-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_bookingbusiness-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingbusiness-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
