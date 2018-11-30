---
title: Получение bookingBusiness
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: 809bfad0685f595b4b8076210c6345760b22f3bc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077009"
---
# <a name="get-bookingbusiness"></a><span data-ttu-id="c9712-104">Получение bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="c9712-104">Get bookingBusiness</span></span>

 > <span data-ttu-id="c9712-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c9712-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9712-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9712-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="c9712-107">Получите свойства и связи объекта [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="c9712-107">Get the properties and relationships of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c9712-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c9712-108">Permissions</span></span>
<span data-ttu-id="c9712-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9712-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9712-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9712-111">Permission type</span></span>      | <span data-ttu-id="c9712-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9712-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9712-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9712-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="c9712-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="c9712-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="c9712-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9712-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9712-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9712-116">Not supported.</span></span>   |
|<span data-ttu-id="c9712-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9712-117">Application</span></span> | <span data-ttu-id="c9712-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9712-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="c9712-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9712-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c9712-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c9712-120">Optional query parameters</span></span>
<span data-ttu-id="c9712-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c9712-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c9712-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9712-122">Request headers</span></span>
| <span data-ttu-id="c9712-123">Имя</span><span class="sxs-lookup"><span data-stu-id="c9712-123">Name</span></span>      |<span data-ttu-id="c9712-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c9712-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c9712-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9712-125">Authorization</span></span>  | <span data-ttu-id="c9712-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c9712-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9712-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c9712-127">Request body</span></span>
<span data-ttu-id="c9712-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c9712-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c9712-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="c9712-129">Response</span></span>
<span data-ttu-id="c9712-130">Успешно завершена, этот метод возвращает `200 OK` объект [bookingBusiness](../resources/bookingbusiness.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c9712-130">If successful, this method returns a `200 OK` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c9712-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c9712-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c9712-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9712-132">Request</span></span>
<span data-ttu-id="c9712-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9712-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingbusiness"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Fabrikam@M365B489948.onmicrosoft.com
```
##### <a name="response"></a><span data-ttu-id="c9712-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="c9712-134">Response</span></span>
<span data-ttu-id="c9712-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c9712-135">The following is an example of the response.</span></span> <span data-ttu-id="c9712-136">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="c9712-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c9712-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c9712-137">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->