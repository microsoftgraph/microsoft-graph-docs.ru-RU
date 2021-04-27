---
title: Список staffMembers
description: Получите список объектов bookingStaffMember в указанном bookingbusiness.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 32fd259d2ac7be2f8fbf9f7b2eda10ff13699315
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047877"
---
# <a name="list-staffmembers"></a><span data-ttu-id="755c9-103">Список staffMembers</span><span class="sxs-lookup"><span data-stu-id="755c9-103">List staffMembers</span></span>

<span data-ttu-id="755c9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="755c9-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="755c9-105">Получите список объектов [bookingStaffMember](../resources/bookingstaffmember.md) в указанном [bookingbusiness.](../resources/bookingbusiness.md)</span><span class="sxs-lookup"><span data-stu-id="755c9-105">Get a list of [bookingStaffMember](../resources/bookingstaffmember.md) objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="755c9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="755c9-106">Permissions</span></span>
<span data-ttu-id="755c9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="755c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="755c9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="755c9-109">Permission type</span></span>      | <span data-ttu-id="755c9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="755c9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="755c9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="755c9-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="755c9-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="755c9-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="755c9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="755c9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="755c9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="755c9-114">Not supported.</span></span>   |
|<span data-ttu-id="755c9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="755c9-115">Application</span></span> | <span data-ttu-id="755c9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="755c9-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="755c9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="755c9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/staffMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="755c9-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="755c9-118">Optional query parameters</span></span>
<span data-ttu-id="755c9-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="755c9-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="755c9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="755c9-120">Request headers</span></span>
| <span data-ttu-id="755c9-121">Имя</span><span class="sxs-lookup"><span data-stu-id="755c9-121">Name</span></span>      |<span data-ttu-id="755c9-122">Описание</span><span class="sxs-lookup"><span data-stu-id="755c9-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="755c9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="755c9-123">Authorization</span></span>  | <span data-ttu-id="755c9-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="755c9-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="755c9-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="755c9-125">Request body</span></span>
<span data-ttu-id="755c9-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="755c9-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="755c9-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="755c9-127">Response</span></span>
<span data-ttu-id="755c9-128">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов bookingStaffMember](../resources/bookingstaffmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="755c9-128">If successful, this method returns a `200 OK` response code and collection of [bookingStaffMember](../resources/bookingstaffmember.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="755c9-129">Пример</span><span class="sxs-lookup"><span data-stu-id="755c9-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="755c9-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="755c9-130">Request</span></span>
<span data-ttu-id="755c9-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="755c9-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="755c9-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="755c9-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_staffmembers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffMembers
```
# <a name="c"></a>[<span data-ttu-id="755c9-133">C#</span><span class="sxs-lookup"><span data-stu-id="755c9-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-staffmembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="755c9-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="755c9-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-staffmembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="755c9-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="755c9-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-staffmembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="755c9-136">Java</span><span class="sxs-lookup"><span data-stu-id="755c9-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-staffmembers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="755c9-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="755c9-137">Response</span></span>
<span data-ttu-id="755c9-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="755c9-138">The following is an example of the response.</span></span> <span data-ttu-id="755c9-139">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="755c9-139">Note: The response object shown here might be shortened for readability.</span></span>
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
