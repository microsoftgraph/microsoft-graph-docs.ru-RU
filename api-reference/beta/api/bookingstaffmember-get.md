---
title: Получение Букингстаффмембер
description: Получение свойств и связей объекта Букингстаффмембер в указанном букингбусинесс.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 3258189da65ee53df9a9da209cfc516467ea06f1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865234"
---
# <a name="get-bookingstaffmember"></a><span data-ttu-id="37c5e-103">Получение Букингстаффмембер</span><span class="sxs-lookup"><span data-stu-id="37c5e-103">Get bookingStaffMember</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37c5e-104">Получение свойств и связей объекта [букингстаффмембер](../resources/bookingstaffmember.md) в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="37c5e-104">Get the properties and relationships of a [bookingStaffMember](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="37c5e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="37c5e-105">Permissions</span></span>
<span data-ttu-id="37c5e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37c5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37c5e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37c5e-108">Permission type</span></span>      | <span data-ttu-id="37c5e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="37c5e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37c5e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37c5e-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="37c5e-111">Резервирования. Read. ALL, Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="37c5e-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="37c5e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37c5e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37c5e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37c5e-113">Not supported.</span></span>   |
|<span data-ttu-id="37c5e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="37c5e-114">Application</span></span> | <span data-ttu-id="37c5e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37c5e-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="37c5e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37c5e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/staffMembers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="37c5e-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="37c5e-117">Optional query parameters</span></span>
<span data-ttu-id="37c5e-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="37c5e-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="37c5e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="37c5e-119">Request headers</span></span>
| <span data-ttu-id="37c5e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="37c5e-120">Name</span></span>      |<span data-ttu-id="37c5e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="37c5e-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="37c5e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="37c5e-122">Authorization</span></span>  | <span data-ttu-id="37c5e-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="37c5e-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="37c5e-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="37c5e-124">Request body</span></span>
<span data-ttu-id="37c5e-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="37c5e-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="37c5e-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="37c5e-126">Response</span></span>
<span data-ttu-id="37c5e-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [букингстаффмембер](../resources/bookingstaffmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="37c5e-127">If successful, this method returns a `200 OK` response code and [bookingStaffMember](../resources/bookingstaffmember.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="37c5e-128">Пример</span><span class="sxs-lookup"><span data-stu-id="37c5e-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="37c5e-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="37c5e-129">Request</span></span>
<span data-ttu-id="37c5e-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37c5e-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="37c5e-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="37c5e-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingstaffmember"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/71d64d0e-7225-49b6-b0b1-070d476cda51
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="37c5e-132">C#</span><span class="sxs-lookup"><span data-stu-id="37c5e-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingstaffmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="37c5e-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="37c5e-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingstaffmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="37c5e-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="37c5e-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingstaffmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="37c5e-135">Java</span><span class="sxs-lookup"><span data-stu-id="37c5e-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bookingstaffmember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="37c5e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="37c5e-136">Response</span></span>
<span data-ttu-id="37c5e-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="37c5e-137">The following is an example of the response.</span></span> <span data-ttu-id="37c5e-138">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="37c5e-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="37c5e-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="37c5e-139">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingStaffMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/staffMembers/$entity",
    "id": "71d64d0e-7225-49b6-b0b1-070d476cda51",
    "displayName": "Samantha Booth",
    "emailAddress": "samanthab@M365B489948.OnMicrosoft.com",
    "availabilityIsAffectedByPersonalCalendar": true,
    "colorIndex": 0,
    "role": "administrator",
    "useBusinessHours": true,
    "workingHours": [
        {
            "day": "monday",
            "timeSlots": [
                {
                    "start": "08:00:00.0000000",
                    "end": "17:00:00.0000000"
                }
            ]
        },
        {
            "day": "tuesday",
            "timeSlots": [
                {
                    "start": "08:00:00.0000000",
                    "end": "17:00:00.0000000"
                }
            ]
        },
        {
            "day": "wednesday",
            "timeSlots": [
                {
                    "start": "08:00:00.0000000",
                    "end": "17:00:00.0000000"
                }
            ]
        },
        {
            "day": "thursday",
            "timeSlots": [
                {
                    "start": "08:00:00.0000000",
                    "end": "17:00:00.0000000"
                }
            ]
        },
        {
            "day": "friday",
            "timeSlots": [
                {
                    "start": "08:00:00.0000000",
                    "end": "17:00:00.0000000"
                }
            ]
        },
        {
            "day": "saturday",
            "timeSlots": []
        },
        {
            "day": "sunday",
            "timeSlots": []
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get bookingStaffMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
