---
title: Создание Букингстаффмембер
description: Создайте новый сотрудник в заданном букингбусинесс.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 3c4336635303874268cfda64217b5648a561f9ea
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439170"
---
# <a name="create-bookingstaffmember"></a><span data-ttu-id="db6bd-103">Создание Букингстаффмембер</span><span class="sxs-lookup"><span data-stu-id="db6bd-103">Create bookingStaffMember</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db6bd-104">Создайте новый [сотрудник](../resources/bookingstaffmember.md) в заданном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="db6bd-104">Create a new [staff member](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="db6bd-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db6bd-105">Permissions</span></span>
<span data-ttu-id="db6bd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db6bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db6bd-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db6bd-108">Permission type</span></span>      | <span data-ttu-id="db6bd-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db6bd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db6bd-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db6bd-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="db6bd-111">Резервирования. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="db6bd-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="db6bd-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db6bd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db6bd-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db6bd-113">Not supported.</span></span>   |
|<span data-ttu-id="db6bd-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db6bd-114">Application</span></span> | <span data-ttu-id="db6bd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db6bd-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="db6bd-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db6bd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/staffMembers

```
## <a name="request-headers"></a><span data-ttu-id="db6bd-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db6bd-117">Request headers</span></span>
| <span data-ttu-id="db6bd-118">Имя</span><span class="sxs-lookup"><span data-stu-id="db6bd-118">Name</span></span>       | <span data-ttu-id="db6bd-119">Описание</span><span class="sxs-lookup"><span data-stu-id="db6bd-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="db6bd-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="db6bd-120">Authorization</span></span>  | <span data-ttu-id="db6bd-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="db6bd-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="db6bd-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db6bd-122">Request body</span></span>
<span data-ttu-id="db6bd-123">В тексте запроса добавьте представление объекта [букингстаффмембер](../resources/bookingstaffmember.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db6bd-123">In the request body, supply a JSON representation of [bookingStaffMember](../resources/bookingstaffmember.md) object.</span></span> <span data-ttu-id="db6bd-124">Необходимо включить следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="db6bd-124">You must include the following properties:</span></span>

- <span data-ttu-id="db6bd-125">**displayName**</span><span class="sxs-lookup"><span data-stu-id="db6bd-125">**displayName**</span></span>
- <span data-ttu-id="db6bd-126">**emailAddress**</span><span class="sxs-lookup"><span data-stu-id="db6bd-126">**emailAddress**</span></span>
- <span data-ttu-id="db6bd-127">**ролей**</span><span class="sxs-lookup"><span data-stu-id="db6bd-127">**role**</span></span>


## <a name="response"></a><span data-ttu-id="db6bd-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="db6bd-128">Response</span></span>
<span data-ttu-id="db6bd-129">В случае успешного выполнения этот метод `201, Created` возвращает код отклика и объект [букингстаффмембер](../resources/bookingstaffmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="db6bd-129">If successful, this method returns `201, Created` response code and [bookingStaffMember](../resources/bookingstaffmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db6bd-130">Пример</span><span class="sxs-lookup"><span data-stu-id="db6bd-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db6bd-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="db6bd-131">Request</span></span>
<span data-ttu-id="db6bd-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db6bd-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="db6bd-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="db6bd-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_bookingstaffmember_from_bookingbusiness"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/staffMembers
Content-type: application/json
Content-length: 309

{
    "@odata.type":"#microsoft.graph.bookingStaffMember",
    "colorIndex":1,
    "displayName":"Dana Swope",
    "emailAddress":"danas@contoso.com",
    "role@odata.type":"#microsoft.graph.bookingStaffRole",
    "role":"externalGuest",
    "useBusinessHours":true,
    "workingHours@odata.type":"#Collection(microsoft.graph.bookingWorkHours)",
    "workingHours":[
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"monday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"tuesday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"wednesday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"thursday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"friday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        }
    ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="db6bd-134">C#</span><span class="sxs-lookup"><span data-stu-id="db6bd-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bookingstaffmember-from-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="db6bd-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="db6bd-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bookingstaffmember-from-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="db6bd-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="db6bd-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bookingstaffmember-from-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="db6bd-137">В тексте запроса добавьте представление объекта [букингстаффмембер](../resources/bookingstaffmember.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db6bd-137">In the request body, supply a JSON representation of [bookingStaffMember](../resources/bookingstaffmember.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="db6bd-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="db6bd-138">Response</span></span>
<span data-ttu-id="db6bd-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="db6bd-139">The following is an example of the response.</span></span> <span data-ttu-id="db6bd-140">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="db6bd-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="db6bd-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="db6bd-141">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingStaffMember"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/staffMembers/$entity",
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
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create bookingStaffMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
