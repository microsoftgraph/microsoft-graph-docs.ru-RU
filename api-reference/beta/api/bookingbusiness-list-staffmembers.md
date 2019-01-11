---
title: Список staffMembers
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: fdbf1c60731627e518bc5d13ad46abfbf6f39b69
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809564"
---
# <a name="list-staffmembers"></a><span data-ttu-id="3b4b1-104">Список staffMembers</span><span class="sxs-lookup"><span data-stu-id="3b4b1-104">List staffMembers</span></span>

 > <span data-ttu-id="3b4b1-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3b4b1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b4b1-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b4b1-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="3b4b1-107">Получите список объектов [bookingStaffMember](../resources/bookingstaffmember.md) в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="3b4b1-107">Get a list of [bookingStaffMember](../resources/bookingstaffmember.md) objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="3b4b1-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3b4b1-108">Permissions</span></span>
<span data-ttu-id="3b4b1-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b4b1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b4b1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b4b1-111">Permission type</span></span>      | <span data-ttu-id="3b4b1-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b4b1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b4b1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b4b1-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="3b4b1-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="3b4b1-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="3b4b1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b4b1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b4b1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b4b1-116">Not supported.</span></span>   |
|<span data-ttu-id="3b4b1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3b4b1-117">Application</span></span> | <span data-ttu-id="3b4b1-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b4b1-118">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="3b4b1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b4b1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/staffMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3b4b1-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3b4b1-120">Optional query parameters</span></span>
<span data-ttu-id="3b4b1-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3b4b1-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3b4b1-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3b4b1-122">Request headers</span></span>
| <span data-ttu-id="3b4b1-123">Имя</span><span class="sxs-lookup"><span data-stu-id="3b4b1-123">Name</span></span>      |<span data-ttu-id="3b4b1-124">Описание</span><span class="sxs-lookup"><span data-stu-id="3b4b1-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3b4b1-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b4b1-125">Authorization</span></span>  | <span data-ttu-id="3b4b1-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3b4b1-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b4b1-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3b4b1-127">Request body</span></span>
<span data-ttu-id="3b4b1-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3b4b1-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3b4b1-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="3b4b1-129">Response</span></span>
<span data-ttu-id="3b4b1-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [bookingStaffMember](../resources/bookingstaffmember.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3b4b1-130">If successful, this method returns a `200 OK` response code and collection of [bookingStaffMember](../resources/bookingstaffmember.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3b4b1-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3b4b1-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3b4b1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b4b1-132">Request</span></span>
<span data-ttu-id="3b4b1-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b4b1-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_staffmembers"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffMembers
```
##### <a name="response"></a><span data-ttu-id="3b4b1-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="3b4b1-134">Response</span></span>
<span data-ttu-id="3b4b1-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3b4b1-135">The following is an example of the response.</span></span> <span data-ttu-id="3b4b1-136">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="3b4b1-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3b4b1-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3b4b1-137">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingStaffMember",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/staffMembers",
    "value":[
        {
            "id":"8ee1c803-a1fa-406d-8259-7ab53233f148",
            "displayName":"Dana Swope",
            "emailAddress":"danas@contoso.com",
            "availabilityIsAffectedByPersonalCalendar":false,
            "colorIndex":1,
            "role":"externalGuest",
            "useBusinessHours":true,
            "workingHours":[
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
                }
            ]
        },
        {
            "id":"71d64d0e-7225-49b6-b0b1-070d476cda51",
            "displayName":"Samantha Booth",
            "emailAddress":"samanthab@M365B489948.OnMicrosoft.com",
            "availabilityIsAffectedByPersonalCalendar":true,
            "colorIndex":0,
            "role":"administrator",
            "useBusinessHours":true,
            "workingHours":[
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
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List staffMembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
