---
title: Обновление букингстаффмембер
description: Обновление свойств объекта Букингстаффмембер в указанном букингбусинесс.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 999eb8bf61b07d64046a356af510c7cb71011400
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895659"
---
# <a name="update-bookingstaffmember"></a><span data-ttu-id="2b3d7-103">Обновление букингстаффмембер</span><span class="sxs-lookup"><span data-stu-id="2b3d7-103">Update bookingstaffmember</span></span>

<span data-ttu-id="2b3d7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b3d7-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b3d7-105">Обновление свойств объекта [букингстаффмембер](../resources/bookingstaffmember.md) в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="2b3d7-105">Update the properties of a [bookingStaffMember](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="2b3d7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2b3d7-106">Permissions</span></span>
<span data-ttu-id="2b3d7-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="2b3d7-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="2b3d7-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b3d7-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b3d7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b3d7-109">Permission type</span></span>      | <span data-ttu-id="2b3d7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b3d7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b3d7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b3d7-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="2b3d7-112">Резервирования. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="2b3d7-112">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="2b3d7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b3d7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b3d7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b3d7-114">Not supported.</span></span>   |
|<span data-ttu-id="2b3d7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b3d7-115">Application</span></span> | <span data-ttu-id="2b3d7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b3d7-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="2b3d7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b3d7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/staffMembers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="2b3d7-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b3d7-118">Optional request headers</span></span>
| <span data-ttu-id="2b3d7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2b3d7-119">Name</span></span>       | <span data-ttu-id="2b3d7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2b3d7-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2b3d7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2b3d7-121">Authorization</span></span>  | <span data-ttu-id="2b3d7-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2b3d7-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b3d7-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b3d7-123">Request body</span></span>
<span data-ttu-id="2b3d7-124">In the request body, supply the values for relevant fields that should be updated.</span><span class="sxs-lookup"><span data-stu-id="2b3d7-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="2b3d7-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span><span class="sxs-lookup"><span data-stu-id="2b3d7-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="2b3d7-126">For best performance you shouldn't include existing values that haven't changed.</span><span class="sxs-lookup"><span data-stu-id="2b3d7-126">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2b3d7-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b3d7-127">Property</span></span>     | <span data-ttu-id="2b3d7-128">Тип</span><span class="sxs-lookup"><span data-stu-id="2b3d7-128">Type</span></span>   |<span data-ttu-id="2b3d7-129">Описание</span><span class="sxs-lookup"><span data-stu-id="2b3d7-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b3d7-130">аваилабилитисаффектедбиперсоналкалендар</span><span class="sxs-lookup"><span data-stu-id="2b3d7-130">availabilityIsAffectedByPersonalCalendar</span></span>|<span data-ttu-id="2b3d7-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b3d7-131">Boolean</span></span>|<span data-ttu-id="2b3d7-132">Значение true означает, что если сотрудник является пользователем Microsoft 365, то в API учета используется личный календарь сотрудника в Microsoft 365, а свойство **воркингхаурс** для определения доступности.</span><span class="sxs-lookup"><span data-stu-id="2b3d7-132">True means that if the staff member is a Microsoft 365 user, the Bookings API uses the staff member's personal calendar in Microsoft 365 as well as the **workingHours** property to determine availability.</span></span> |
|<span data-ttu-id="2b3d7-133">colorIndex</span><span class="sxs-lookup"><span data-stu-id="2b3d7-133">colorIndex</span></span>|<span data-ttu-id="2b3d7-134">Int32</span><span class="sxs-lookup"><span data-stu-id="2b3d7-134">Int32</span></span>|<span data-ttu-id="2b3d7-135">Определяет цвет для представления сотрудника.</span><span class="sxs-lookup"><span data-stu-id="2b3d7-135">Identifies a color to represent the staff member.</span></span> <span data-ttu-id="2b3d7-136">Цвет соответствует цветовой палитре на странице " **сведения о персонале** " в приложении "книги".</span><span class="sxs-lookup"><span data-stu-id="2b3d7-136">The color corresponds to the color palette in the **Staff details** page in the Bookings app.</span></span>|
|<span data-ttu-id="2b3d7-137">displayName</span><span class="sxs-lookup"><span data-stu-id="2b3d7-137">displayName</span></span>|<span data-ttu-id="2b3d7-138">String</span><span class="sxs-lookup"><span data-stu-id="2b3d7-138">String</span></span>|<span data-ttu-id="2b3d7-139">Имя сотрудника, отображаемое для клиентов.</span><span class="sxs-lookup"><span data-stu-id="2b3d7-139">The name of the staff member, as displayed to customers.</span></span>|
|<span data-ttu-id="2b3d7-140">emailAddress</span><span class="sxs-lookup"><span data-stu-id="2b3d7-140">emailAddress</span></span>|<span data-ttu-id="2b3d7-141">String</span><span class="sxs-lookup"><span data-stu-id="2b3d7-141">String</span></span>|<span data-ttu-id="2b3d7-142">Адрес электронной почты сотрудника.</span><span class="sxs-lookup"><span data-stu-id="2b3d7-142">The email address of the staff member.</span></span> <span data-ttu-id="2b3d7-143">Это может быть тот же клиент Microsoft 365, что и в Организации, или в другом домене электронной почты.</span><span class="sxs-lookup"><span data-stu-id="2b3d7-143">This can be in the same Microsoft 365 tenant as the business, or in a different email domain.</span></span> <span data-ttu-id="2b3d7-144">Этот адрес электронной почты используется, если для свойства **сендконфирматионстувнер** в политике планирования бизнеса задано значение true.</span><span class="sxs-lookup"><span data-stu-id="2b3d7-144">This email address is used if the **sendConfirmationsToOwner** property is set to true in the scheduling policy of the business.</span></span>|
|<span data-ttu-id="2b3d7-145">role</span><span class="sxs-lookup"><span data-stu-id="2b3d7-145">role</span></span>|<span data-ttu-id="2b3d7-146">string</span><span class="sxs-lookup"><span data-stu-id="2b3d7-146">string</span></span>| <span data-ttu-id="2b3d7-147">Роль сотрудника в Организации.</span><span class="sxs-lookup"><span data-stu-id="2b3d7-147">The role of the staff member in the business.</span></span> <span data-ttu-id="2b3d7-148">Возможные значения: `guest`, `administrator`, `viewer`, `externalGuest`.</span><span class="sxs-lookup"><span data-stu-id="2b3d7-148">Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.</span></span>|
|<span data-ttu-id="2b3d7-149">усебусинесшаурс</span><span class="sxs-lookup"><span data-stu-id="2b3d7-149">useBusinessHours</span></span>|<span data-ttu-id="2b3d7-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b3d7-150">Boolean</span></span>|<span data-ttu-id="2b3d7-151">Значение true означает, что доступность сотрудника определяется свойством **businessHours** предприятия.</span><span class="sxs-lookup"><span data-stu-id="2b3d7-151">True means the staff member's availability is determined by the **businessHours** property of the business.</span></span> <span data-ttu-id="2b3d7-152">Значение false означает, что доступность определяется значением свойства **воркингхаусе** сотрудника.</span><span class="sxs-lookup"><span data-stu-id="2b3d7-152">False means the availability is determined by the staff member's **workingHouse** property setting.</span></span>|
|<span data-ttu-id="2b3d7-153">workingHours</span><span class="sxs-lookup"><span data-stu-id="2b3d7-153">workingHours</span></span>|<span data-ttu-id="2b3d7-154">Коллекция [букингворкхаурс](../resources/bookingworkhours.md)</span><span class="sxs-lookup"><span data-stu-id="2b3d7-154">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="2b3d7-155">Диапазон часов на каждый день недели, когда сотрудник становится доступен для резервирования.</span><span class="sxs-lookup"><span data-stu-id="2b3d7-155">The range of hours each day of the week that the staff member is available for booking.</span></span>|

## <a name="response"></a><span data-ttu-id="2b3d7-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b3d7-156">Response</span></span>
<span data-ttu-id="2b3d7-157">If successful, this method returns a `204 No content` response code.</span><span class="sxs-lookup"><span data-stu-id="2b3d7-157">If successful, this method returns a `204 No content` response code.</span></span> <span data-ttu-id="2b3d7-158">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="2b3d7-158">It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2b3d7-159">Пример</span><span class="sxs-lookup"><span data-stu-id="2b3d7-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b3d7-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b3d7-160">Request</span></span>
<span data-ttu-id="2b3d7-161">В следующем примере для сотрудника в календарном плане изменяется понедельник.</span><span class="sxs-lookup"><span data-stu-id="2b3d7-161">The following example changes the staff member's schedule to have Mondays off.</span></span>

# <a name="http"></a>[<span data-ttu-id="2b3d7-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b3d7-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_bookingstaffmember"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/8ee1c803-a1fa-406d-8259-7ab53233f148
Content-type: application/json

{
    "workingHours":[
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"monday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[

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
# <a name="c"></a>[<span data-ttu-id="2b3d7-163">C#</span><span class="sxs-lookup"><span data-stu-id="2b3d7-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingstaffmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b3d7-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b3d7-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingstaffmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b3d7-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b3d7-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingstaffmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2b3d7-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b3d7-166">Response</span></span>
<span data-ttu-id="2b3d7-167">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2b3d7-167">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingstaffmember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
