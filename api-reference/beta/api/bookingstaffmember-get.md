---
title: Получение Букингстаффмембер
description: Получение свойств и связей объекта Букингстаффмембер в указанном букингбусинесс.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: f2d7a8a3a01256d2cac324cc10ab5727f140a2a5
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262491"
---
# <a name="get-bookingstaffmember"></a><span data-ttu-id="eebca-103">Получение Букингстаффмембер</span><span class="sxs-lookup"><span data-stu-id="eebca-103">Get bookingStaffMember</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eebca-104">Получение свойств и связей объекта [букингстаффмембер](../resources/bookingstaffmember.md) в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="eebca-104">Get the properties and relationships of a [bookingStaffMember](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="eebca-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eebca-105">Permissions</span></span>
<span data-ttu-id="eebca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eebca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eebca-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eebca-108">Permission type</span></span>      | <span data-ttu-id="eebca-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eebca-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eebca-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eebca-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="eebca-111">Резервирования. Read. ALL, Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="eebca-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="eebca-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eebca-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eebca-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eebca-113">Not supported.</span></span>   |
|<span data-ttu-id="eebca-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eebca-114">Application</span></span> | <span data-ttu-id="eebca-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eebca-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="eebca-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eebca-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/staffMembers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="eebca-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="eebca-117">Optional query parameters</span></span>
<span data-ttu-id="eebca-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="eebca-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eebca-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eebca-119">Request headers</span></span>
| <span data-ttu-id="eebca-120">Имя</span><span class="sxs-lookup"><span data-stu-id="eebca-120">Name</span></span>      |<span data-ttu-id="eebca-121">Описание</span><span class="sxs-lookup"><span data-stu-id="eebca-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="eebca-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eebca-122">Authorization</span></span>  | <span data-ttu-id="eebca-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="eebca-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="eebca-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eebca-124">Request body</span></span>
<span data-ttu-id="eebca-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eebca-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="eebca-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="eebca-126">Response</span></span>
<span data-ttu-id="eebca-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [букингстаффмембер](../resources/bookingstaffmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eebca-127">If successful, this method returns a `200 OK` response code and [bookingStaffMember](../resources/bookingstaffmember.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eebca-128">Пример</span><span class="sxs-lookup"><span data-stu-id="eebca-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eebca-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="eebca-129">Request</span></span>
<span data-ttu-id="eebca-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eebca-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingstaffmember"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/71d64d0e-7225-49b6-b0b1-070d476cda51
```
##### <a name="response"></a><span data-ttu-id="eebca-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="eebca-131">Response</span></span>
<span data-ttu-id="eebca-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="eebca-132">The following is an example of the response.</span></span> <span data-ttu-id="eebca-133">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="eebca-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="eebca-134">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eebca-134">All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="eebca-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="eebca-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="eebca-136">C#</span><span class="sxs-lookup"><span data-stu-id="eebca-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_bookingstaffmember-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eebca-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="eebca-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_bookingstaffmember-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="eebca-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="eebca-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_bookingstaffmember-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/bookingstaffmember-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingstaffmember-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingstaffmember-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
