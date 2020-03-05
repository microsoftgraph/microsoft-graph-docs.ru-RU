---
title: Создание Букингстаффмембер
description: Создайте новый сотрудник в заданном букингбусинесс.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: fc38c6bac1a775d2d3848cb6bf2938a0ac1c08c7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441160"
---
# <a name="create-bookingstaffmember"></a><span data-ttu-id="6a64f-103">Создание Букингстаффмембер</span><span class="sxs-lookup"><span data-stu-id="6a64f-103">Create bookingStaffMember</span></span>

<span data-ttu-id="6a64f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6a64f-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a64f-105">Создайте новый [сотрудник](../resources/bookingstaffmember.md) в заданном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="6a64f-105">Create a new [staff member](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="6a64f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6a64f-106">Permissions</span></span>
<span data-ttu-id="6a64f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a64f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a64f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6a64f-109">Permission type</span></span>      | <span data-ttu-id="6a64f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6a64f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a64f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6a64f-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="6a64f-112">Резервирования. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="6a64f-112">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="6a64f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6a64f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a64f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a64f-114">Not supported.</span></span>   |
|<span data-ttu-id="6a64f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6a64f-115">Application</span></span> | <span data-ttu-id="6a64f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a64f-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="6a64f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6a64f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/staffMembers

```
## <a name="request-headers"></a><span data-ttu-id="6a64f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6a64f-118">Request headers</span></span>
| <span data-ttu-id="6a64f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6a64f-119">Name</span></span>       | <span data-ttu-id="6a64f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6a64f-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6a64f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6a64f-121">Authorization</span></span>  | <span data-ttu-id="6a64f-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="6a64f-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a64f-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6a64f-123">Request body</span></span>
<span data-ttu-id="6a64f-124">В тексте запроса добавьте представление объекта [букингстаффмембер](../resources/bookingstaffmember.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a64f-124">In the request body, supply a JSON representation of [bookingStaffMember](../resources/bookingstaffmember.md) object.</span></span> <span data-ttu-id="6a64f-125">Необходимо включить следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="6a64f-125">You must include the following properties:</span></span>

- <span data-ttu-id="6a64f-126">**displayName**</span><span class="sxs-lookup"><span data-stu-id="6a64f-126">**displayName**</span></span>
- <span data-ttu-id="6a64f-127">**emailAddress**</span><span class="sxs-lookup"><span data-stu-id="6a64f-127">**emailAddress**</span></span>
- <span data-ttu-id="6a64f-128">**ролей**</span><span class="sxs-lookup"><span data-stu-id="6a64f-128">**role**</span></span>


## <a name="response"></a><span data-ttu-id="6a64f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a64f-129">Response</span></span>
<span data-ttu-id="6a64f-130">В случае успешного выполнения этот метод `201, Created` возвращает код отклика и объект [букингстаффмембер](../resources/bookingstaffmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6a64f-130">If successful, this method returns `201, Created` response code and [bookingStaffMember](../resources/bookingstaffmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a64f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6a64f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6a64f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a64f-132">Request</span></span>
<span data-ttu-id="6a64f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6a64f-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6a64f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a64f-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6a64f-135">C#</span><span class="sxs-lookup"><span data-stu-id="6a64f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bookingstaffmember-from-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6a64f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a64f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bookingstaffmember-from-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6a64f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6a64f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bookingstaffmember-from-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="6a64f-138">В тексте запроса добавьте представление объекта [букингстаффмембер](../resources/bookingstaffmember.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a64f-138">In the request body, supply a JSON representation of [bookingStaffMember](../resources/bookingstaffmember.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="6a64f-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a64f-139">Response</span></span>
<span data-ttu-id="6a64f-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6a64f-140">The following is an example of the response.</span></span> <span data-ttu-id="6a64f-141">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="6a64f-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6a64f-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6a64f-142">All of the properties will be returned from an actual call.</span></span>
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
