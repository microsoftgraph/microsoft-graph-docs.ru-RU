---
title: Список staffMembers
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: a2b04aba32d3bbc51dc380f51b54a2700114fd20
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076698"
---
# <a name="list-staffmembers"></a><span data-ttu-id="56c16-104">Список staffMembers</span><span class="sxs-lookup"><span data-stu-id="56c16-104">List staffMembers</span></span>

 > <span data-ttu-id="56c16-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="56c16-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56c16-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56c16-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="56c16-107">Получите список объектов [bookingStaffMember](../resources/bookingstaffmember.md) в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="56c16-107">Get a list of [bookingStaffMember](../resources/bookingstaffmember.md) objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="56c16-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="56c16-108">Permissions</span></span>
<span data-ttu-id="56c16-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56c16-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56c16-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56c16-111">Permission type</span></span>      | <span data-ttu-id="56c16-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="56c16-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56c16-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56c16-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="56c16-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="56c16-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="56c16-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56c16-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56c16-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56c16-116">Not supported.</span></span>   |
|<span data-ttu-id="56c16-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="56c16-117">Application</span></span> | <span data-ttu-id="56c16-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56c16-118">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="56c16-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56c16-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/staffMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="56c16-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="56c16-120">Optional query parameters</span></span>
<span data-ttu-id="56c16-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="56c16-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="56c16-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="56c16-122">Request headers</span></span>
| <span data-ttu-id="56c16-123">Имя</span><span class="sxs-lookup"><span data-stu-id="56c16-123">Name</span></span>      |<span data-ttu-id="56c16-124">Описание</span><span class="sxs-lookup"><span data-stu-id="56c16-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="56c16-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="56c16-125">Authorization</span></span>  | <span data-ttu-id="56c16-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="56c16-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="56c16-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="56c16-127">Request body</span></span>
<span data-ttu-id="56c16-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="56c16-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="56c16-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="56c16-129">Response</span></span>
<span data-ttu-id="56c16-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [bookingStaffMember](../resources/bookingstaffmember.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="56c16-130">If successful, this method returns a `200 OK` response code and collection of [bookingStaffMember](../resources/bookingstaffmember.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="56c16-131">Пример</span><span class="sxs-lookup"><span data-stu-id="56c16-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="56c16-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="56c16-132">Request</span></span>
<span data-ttu-id="56c16-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56c16-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_staffmembers"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffMembers
```
##### <a name="response"></a><span data-ttu-id="56c16-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="56c16-134">Response</span></span>
<span data-ttu-id="56c16-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="56c16-135">The following is an example of the response.</span></span> <span data-ttu-id="56c16-136">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="56c16-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="56c16-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="56c16-137">All of the properties will be returned from an actual call.</span></span>
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