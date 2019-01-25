---
title: Получение bookingBusiness
description: Получите свойства и связи объекта bookingBusiness.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 229da03e377f1ff0add73195505c359c9fd68121
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508932"
---
# <a name="get-bookingbusiness"></a><span data-ttu-id="71488-103">Получение bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="71488-103">Get bookingBusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71488-104">Получите свойства и связи объекта [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="71488-104">Get the properties and relationships of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="71488-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71488-105">Permissions</span></span>
<span data-ttu-id="71488-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71488-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71488-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71488-108">Permission type</span></span>      | <span data-ttu-id="71488-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71488-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71488-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71488-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="71488-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="71488-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="71488-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71488-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71488-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71488-113">Not supported.</span></span>   |
|<span data-ttu-id="71488-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71488-114">Application</span></span> | <span data-ttu-id="71488-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71488-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="71488-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71488-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="71488-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="71488-117">Optional query parameters</span></span>
<span data-ttu-id="71488-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="71488-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71488-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71488-119">Request headers</span></span>
| <span data-ttu-id="71488-120">Имя</span><span class="sxs-lookup"><span data-stu-id="71488-120">Name</span></span>      |<span data-ttu-id="71488-121">Описание</span><span class="sxs-lookup"><span data-stu-id="71488-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="71488-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="71488-122">Authorization</span></span>  | <span data-ttu-id="71488-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="71488-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="71488-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71488-124">Request body</span></span>
<span data-ttu-id="71488-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="71488-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="71488-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="71488-126">Response</span></span>
<span data-ttu-id="71488-127">Успешно завершена, этот метод возвращает `200 OK` объект [bookingBusiness](../resources/bookingbusiness.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="71488-127">If successful, this method returns a `200 OK` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="71488-128">Пример</span><span class="sxs-lookup"><span data-stu-id="71488-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71488-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="71488-129">Request</span></span>
<span data-ttu-id="71488-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71488-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingbusiness"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Fabrikam@M365B489948.onmicrosoft.com
```
##### <a name="response"></a><span data-ttu-id="71488-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="71488-131">Response</span></span>
<span data-ttu-id="71488-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="71488-132">The following is an example of the response.</span></span> <span data-ttu-id="71488-133">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="71488-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="71488-134">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="71488-134">All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/bookingbusiness-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
