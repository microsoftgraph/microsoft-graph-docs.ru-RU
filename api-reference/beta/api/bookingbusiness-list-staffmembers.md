---
title: Список Стаффмемберс
description: Получение списка объектов Букингстаффмембер в указанном букингбусинесс.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 13ee8acefbcb7b2e405f9f45f864debb80320084
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36720223"
---
# <a name="list-staffmembers"></a><span data-ttu-id="cbf83-103">Список Стаффмемберс</span><span class="sxs-lookup"><span data-stu-id="cbf83-103">List staffMembers</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbf83-104">Получение списка объектов [букингстаффмембер](../resources/bookingstaffmember.md) в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="cbf83-104">Get a list of [bookingStaffMember](../resources/bookingstaffmember.md) objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="cbf83-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cbf83-105">Permissions</span></span>
<span data-ttu-id="cbf83-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbf83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbf83-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cbf83-108">Permission type</span></span>      | <span data-ttu-id="cbf83-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cbf83-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cbf83-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cbf83-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="cbf83-111">Резервирования. Read. ALL, Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="cbf83-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="cbf83-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cbf83-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbf83-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cbf83-113">Not supported.</span></span>   |
|<span data-ttu-id="cbf83-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cbf83-114">Application</span></span> | <span data-ttu-id="cbf83-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cbf83-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="cbf83-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cbf83-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/staffMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cbf83-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cbf83-117">Optional query parameters</span></span>
<span data-ttu-id="cbf83-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cbf83-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cbf83-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cbf83-119">Request headers</span></span>
| <span data-ttu-id="cbf83-120">Имя</span><span class="sxs-lookup"><span data-stu-id="cbf83-120">Name</span></span>      |<span data-ttu-id="cbf83-121">Описание</span><span class="sxs-lookup"><span data-stu-id="cbf83-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cbf83-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cbf83-122">Authorization</span></span>  | <span data-ttu-id="cbf83-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="cbf83-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbf83-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cbf83-124">Request body</span></span>
<span data-ttu-id="cbf83-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cbf83-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="cbf83-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbf83-126">Response</span></span>
<span data-ttu-id="cbf83-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [букингстаффмембер](../resources/bookingstaffmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cbf83-127">If successful, this method returns a `200 OK` response code and collection of [bookingStaffMember](../resources/bookingstaffmember.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cbf83-128">Пример</span><span class="sxs-lookup"><span data-stu-id="cbf83-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cbf83-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="cbf83-129">Request</span></span>
<span data-ttu-id="cbf83-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cbf83-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cbf83-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="cbf83-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_staffmembers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffMembers
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cbf83-132">C#</span><span class="sxs-lookup"><span data-stu-id="cbf83-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-staffmembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cbf83-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cbf83-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-staffmembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cbf83-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="cbf83-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-staffmembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cbf83-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbf83-135">Response</span></span>
<span data-ttu-id="cbf83-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cbf83-136">The following is an example of the response.</span></span> <span data-ttu-id="cbf83-137">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="cbf83-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="cbf83-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cbf83-138">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List staffMembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
