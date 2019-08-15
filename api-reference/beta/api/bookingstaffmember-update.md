---
title: Обновление букингстаффмембер
description: Обновление свойств объекта Букингстаффмембер в указанном букингбусинесс.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: d9a9e6d429fddfc087506a02191918571fb4c7dc
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419284"
---
# <a name="update-bookingstaffmember"></a><span data-ttu-id="63fe9-103">Обновление букингстаффмембер</span><span class="sxs-lookup"><span data-stu-id="63fe9-103">Update bookingstaffmember</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63fe9-104">Обновление свойств объекта [букингстаффмембер](../resources/bookingstaffmember.md) в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="63fe9-104">Update the properties of a [bookingStaffMember](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="63fe9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="63fe9-105">Permissions</span></span>
<span data-ttu-id="63fe9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63fe9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63fe9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63fe9-108">Permission type</span></span>      | <span data-ttu-id="63fe9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="63fe9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63fe9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63fe9-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="63fe9-111">Резервирования. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="63fe9-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="63fe9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63fe9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63fe9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63fe9-113">Not supported.</span></span>   |
|<span data-ttu-id="63fe9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="63fe9-114">Application</span></span> | <span data-ttu-id="63fe9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63fe9-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="63fe9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63fe9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/staffMembers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="63fe9-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="63fe9-117">Optional request headers</span></span>
| <span data-ttu-id="63fe9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="63fe9-118">Name</span></span>       | <span data-ttu-id="63fe9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="63fe9-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="63fe9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="63fe9-120">Authorization</span></span>  | <span data-ttu-id="63fe9-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="63fe9-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="63fe9-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="63fe9-122">Request body</span></span>
<span data-ttu-id="63fe9-p102">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="63fe9-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="63fe9-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="63fe9-126">Property</span></span>     | <span data-ttu-id="63fe9-127">Тип</span><span class="sxs-lookup"><span data-stu-id="63fe9-127">Type</span></span>   |<span data-ttu-id="63fe9-128">Описание</span><span class="sxs-lookup"><span data-stu-id="63fe9-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63fe9-129">аваилабилитисаффектедбиперсоналкалендар</span><span class="sxs-lookup"><span data-stu-id="63fe9-129">availabilityIsAffectedByPersonalCalendar</span></span>|<span data-ttu-id="63fe9-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="63fe9-130">Boolean</span></span>|<span data-ttu-id="63fe9-131">True означает, что если сотрудник является пользователем Office 365, то в API учета используется личный календарь сотрудника в Office 365, а свойство **воркингхаурс** для определения доступности.</span><span class="sxs-lookup"><span data-stu-id="63fe9-131">True means that if the staff member is an Office 365 user, the Bookings API uses the staff member's personal calendar in Office 365 as well as the **workingHours** property to determine availability.</span></span> |
|<span data-ttu-id="63fe9-132">colorIndex</span><span class="sxs-lookup"><span data-stu-id="63fe9-132">colorIndex</span></span>|<span data-ttu-id="63fe9-133">Int32</span><span class="sxs-lookup"><span data-stu-id="63fe9-133">Int32</span></span>|<span data-ttu-id="63fe9-134">Определяет цвет для представления сотрудника.</span><span class="sxs-lookup"><span data-stu-id="63fe9-134">Identifies a color to represent the staff member.</span></span> <span data-ttu-id="63fe9-135">Цвет соответствует цветовой палитре на странице " **сведения о персонале** " в приложении "книги".</span><span class="sxs-lookup"><span data-stu-id="63fe9-135">The color corresponds to the color palette in the **Staff details** page in the Bookings app.</span></span>|
|<span data-ttu-id="63fe9-136">displayName</span><span class="sxs-lookup"><span data-stu-id="63fe9-136">displayName</span></span>|<span data-ttu-id="63fe9-137">String</span><span class="sxs-lookup"><span data-stu-id="63fe9-137">String</span></span>|<span data-ttu-id="63fe9-138">Имя сотрудника, отображаемое для клиентов.</span><span class="sxs-lookup"><span data-stu-id="63fe9-138">The name of the staff member, as displayed to customers.</span></span>|
|<span data-ttu-id="63fe9-139">emailAddress</span><span class="sxs-lookup"><span data-stu-id="63fe9-139">emailAddress</span></span>|<span data-ttu-id="63fe9-140">String</span><span class="sxs-lookup"><span data-stu-id="63fe9-140">String</span></span>|<span data-ttu-id="63fe9-141">Адрес электронной почты сотрудника.</span><span class="sxs-lookup"><span data-stu-id="63fe9-141">The email address of the staff member.</span></span> <span data-ttu-id="63fe9-142">Это может быть тот же клиент Office 365, что и в Организации, или в другом домене электронной почты.</span><span class="sxs-lookup"><span data-stu-id="63fe9-142">This can be in the same Office 365 tenant as the business, or in a different email domain.</span></span> <span data-ttu-id="63fe9-143">Этот адрес электронной почты используется, если для свойства **сендконфирматионстувнер** в политике планирования бизнеса задано значение true.</span><span class="sxs-lookup"><span data-stu-id="63fe9-143">This email address is used if the **sendConfirmationsToOwner** property is set to true in the scheduling policy of the business.</span></span>|
|<span data-ttu-id="63fe9-144">role</span><span class="sxs-lookup"><span data-stu-id="63fe9-144">role</span></span>|<span data-ttu-id="63fe9-145">string</span><span class="sxs-lookup"><span data-stu-id="63fe9-145">string</span></span>| <span data-ttu-id="63fe9-146">Роль сотрудника в Организации.</span><span class="sxs-lookup"><span data-stu-id="63fe9-146">The role of the staff member in the business.</span></span> <span data-ttu-id="63fe9-147">Возможные значения: `guest`, `administrator`, `viewer`, `externalGuest`.</span><span class="sxs-lookup"><span data-stu-id="63fe9-147">Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.</span></span>|
|<span data-ttu-id="63fe9-148">усебусинесшаурс</span><span class="sxs-lookup"><span data-stu-id="63fe9-148">useBusinessHours</span></span>|<span data-ttu-id="63fe9-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="63fe9-149">Boolean</span></span>|<span data-ttu-id="63fe9-150">Значение true означает, что доступность сотрудника определяется свойством **businessHours** предприятия.</span><span class="sxs-lookup"><span data-stu-id="63fe9-150">True means the staff member's availability is determined by the **businessHours** property of the business.</span></span> <span data-ttu-id="63fe9-151">Значение false означает, что доступность определяется значением свойства **воркингхаусе** сотрудника.</span><span class="sxs-lookup"><span data-stu-id="63fe9-151">False means the availability is determined by the staff member's **workingHouse** property setting.</span></span>|
|<span data-ttu-id="63fe9-152">workingHours</span><span class="sxs-lookup"><span data-stu-id="63fe9-152">workingHours</span></span>|<span data-ttu-id="63fe9-153">Коллекция [букингворкхаурс](../resources/bookingworkhours.md)</span><span class="sxs-lookup"><span data-stu-id="63fe9-153">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="63fe9-154">Диапазон часов на каждый день недели, когда сотрудник становится доступен для резервирования.</span><span class="sxs-lookup"><span data-stu-id="63fe9-154">The range of hours each day of the week that the staff member is available for booking.</span></span>|

## <a name="response"></a><span data-ttu-id="63fe9-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="63fe9-155">Response</span></span>
<span data-ttu-id="63fe9-p107">При успешном выполнении этот метод возвращает код отклика `204 No content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="63fe9-p107">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="63fe9-158">Пример</span><span class="sxs-lookup"><span data-stu-id="63fe9-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="63fe9-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="63fe9-159">Request</span></span>
<span data-ttu-id="63fe9-160">В следующем примере для сотрудника в календарном плане изменяется понедельник.</span><span class="sxs-lookup"><span data-stu-id="63fe9-160">The following example changes the staff member's schedule to have Mondays off.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="63fe9-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="63fe9-161">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="63fe9-162">C#</span><span class="sxs-lookup"><span data-stu-id="63fe9-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingstaffmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="63fe9-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63fe9-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingstaffmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="63fe9-164">Цель — C</span><span class="sxs-lookup"><span data-stu-id="63fe9-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingstaffmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="63fe9-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="63fe9-165">Response</span></span>
<span data-ttu-id="63fe9-166">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="63fe9-166">The following is an example of the response.</span></span>
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
