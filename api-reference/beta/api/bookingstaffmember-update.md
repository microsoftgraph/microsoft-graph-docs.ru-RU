---
title: Обновление bookingstaffmember
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: 4ba2ea126f916b6bd91b83bdd81e24d30fae8ac4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824985"
---
# <a name="update-bookingstaffmember"></a><span data-ttu-id="14e82-104">Обновление bookingstaffmember</span><span class="sxs-lookup"><span data-stu-id="14e82-104">Update bookingstaffmember</span></span>

 > <span data-ttu-id="14e82-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="14e82-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="14e82-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14e82-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="14e82-107">Обновление свойств [bookingStaffMember](../resources/bookingstaffmember.md) в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="14e82-107">Update the properties of a [bookingStaffMember](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="14e82-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="14e82-108">Permissions</span></span>
<span data-ttu-id="14e82-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14e82-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14e82-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14e82-111">Permission type</span></span>      | <span data-ttu-id="14e82-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="14e82-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14e82-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14e82-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="14e82-114">Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="14e82-114">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="14e82-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14e82-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14e82-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14e82-116">Not supported.</span></span>   |
|<span data-ttu-id="14e82-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14e82-117">Application</span></span> | <span data-ttu-id="14e82-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14e82-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="14e82-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14e82-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/staffMembers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="14e82-120">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14e82-120">Optional request headers</span></span>
| <span data-ttu-id="14e82-121">Имя</span><span class="sxs-lookup"><span data-stu-id="14e82-121">Name</span></span>       | <span data-ttu-id="14e82-122">Описание</span><span class="sxs-lookup"><span data-stu-id="14e82-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="14e82-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="14e82-123">Authorization</span></span>  | <span data-ttu-id="14e82-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="14e82-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="14e82-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="14e82-125">Request body</span></span>
<span data-ttu-id="14e82-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="14e82-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="14e82-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="14e82-129">Property</span></span>     | <span data-ttu-id="14e82-130">Тип</span><span class="sxs-lookup"><span data-stu-id="14e82-130">Type</span></span>   |<span data-ttu-id="14e82-131">Описание</span><span class="sxs-lookup"><span data-stu-id="14e82-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="14e82-132">availabilityIsAffectedByPersonalCalendar</span><span class="sxs-lookup"><span data-stu-id="14e82-132">availabilityIsAffectedByPersonalCalendar</span></span>|<span data-ttu-id="14e82-133">Логический</span><span class="sxs-lookup"><span data-stu-id="14e82-133">Boolean</span></span>|<span data-ttu-id="14e82-134">Значение true означает, что если сотрудник является пользователь Office 365, API резервирования применяет сотрудник личного календаря в Office 365, а также свойство **workingHours** для определения доступности.</span><span class="sxs-lookup"><span data-stu-id="14e82-134">True means that if the staff member is an Office 365 user, the Bookings API uses the staff member's personal calendar in Office 365 as well as the **workingHours** property to determine availability.</span></span> |
|<span data-ttu-id="14e82-135">ColorIndex (en)</span><span class="sxs-lookup"><span data-stu-id="14e82-135">colorIndex</span></span>|<span data-ttu-id="14e82-136">Int32</span><span class="sxs-lookup"><span data-stu-id="14e82-136">Int32</span></span>|<span data-ttu-id="14e82-137">Определяет цвет сотрудника.</span><span class="sxs-lookup"><span data-stu-id="14e82-137">Identifies a color to represent the staff member.</span></span> <span data-ttu-id="14e82-138">Цвет соответствует цветовой палитры на странице **сведений о персонала** в приложении резервирования.</span><span class="sxs-lookup"><span data-stu-id="14e82-138">The color corresponds to the color palette in the **Staff details** page in the Bookings app.</span></span>|
|<span data-ttu-id="14e82-139">displayName</span><span class="sxs-lookup"><span data-stu-id="14e82-139">displayName</span></span>|<span data-ttu-id="14e82-140">Строка</span><span class="sxs-lookup"><span data-stu-id="14e82-140">String</span></span>|<span data-ttu-id="14e82-141">Имя сотрудника, как оно отображается для клиентов.</span><span class="sxs-lookup"><span data-stu-id="14e82-141">The name of the staff member, as displayed to customers.</span></span>|
|<span data-ttu-id="14e82-142">emailAddress</span><span class="sxs-lookup"><span data-stu-id="14e82-142">emailAddress</span></span>|<span data-ttu-id="14e82-143">String</span><span class="sxs-lookup"><span data-stu-id="14e82-143">String</span></span>|<span data-ttu-id="14e82-144">Адрес электронной почты сотрудника.</span><span class="sxs-lookup"><span data-stu-id="14e82-144">The email address of the staff member.</span></span> <span data-ttu-id="14e82-145">Это может быть в одном клиентов Office 365 как предприятию или в домене различных электронной почты.</span><span class="sxs-lookup"><span data-stu-id="14e82-145">This can be in the same Office 365 tenant as the business, or in a different email domain.</span></span> <span data-ttu-id="14e82-146">Этот адрес электронной почты используется, если свойство **sendConfirmationsToOwner** имеет значение true в политике планирования бизнеса.</span><span class="sxs-lookup"><span data-stu-id="14e82-146">This email address is used if the **sendConfirmationsToOwner** property is set to true in the scheduling policy of the business.</span></span>|
|<span data-ttu-id="14e82-147">role</span><span class="sxs-lookup"><span data-stu-id="14e82-147">role</span></span>|<span data-ttu-id="14e82-148">string</span><span class="sxs-lookup"><span data-stu-id="14e82-148">string</span></span>| <span data-ttu-id="14e82-149">Роль сотрудника в организации.</span><span class="sxs-lookup"><span data-stu-id="14e82-149">The role of the staff member in the business.</span></span> <span data-ttu-id="14e82-150">Возможные значения: `guest`, `administrator`, `viewer`, `externalGuest`.</span><span class="sxs-lookup"><span data-stu-id="14e82-150">Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.</span></span>|
|<span data-ttu-id="14e82-151">useBusinessHours</span><span class="sxs-lookup"><span data-stu-id="14e82-151">useBusinessHours</span></span>|<span data-ttu-id="14e82-152">Логический</span><span class="sxs-lookup"><span data-stu-id="14e82-152">Boolean</span></span>|<span data-ttu-id="14e82-153">Значение true означает, что сотрудник доступность определяется свойством **businessHours** бизнеса.</span><span class="sxs-lookup"><span data-stu-id="14e82-153">True means the staff member's availability is determined by the **businessHours** property of the business.</span></span> <span data-ttu-id="14e82-154">False означает, что доступность определяется значение свойства **workingHouse** сотрудника.</span><span class="sxs-lookup"><span data-stu-id="14e82-154">False means the availability is determined by the staff member's **workingHouse** property setting.</span></span>|
|<span data-ttu-id="14e82-155">workingHours</span><span class="sxs-lookup"><span data-stu-id="14e82-155">workingHours</span></span>|<span data-ttu-id="14e82-156">[bookingWorkHours](../resources/bookingworkhours.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="14e82-156">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="14e82-157">Диапазон часов каждый день недели, по которым сотрудник доступна для резервирования.</span><span class="sxs-lookup"><span data-stu-id="14e82-157">The range of hours each day of the week that the staff member is available for booking.</span></span>|

## <a name="response"></a><span data-ttu-id="14e82-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="14e82-158">Response</span></span>
<span data-ttu-id="14e82-p109">При успешном выполнении этот метод возвращает код отклика `204 No content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="14e82-p109">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="14e82-161">Пример</span><span class="sxs-lookup"><span data-stu-id="14e82-161">Example</span></span>
##### <a name="request"></a><span data-ttu-id="14e82-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="14e82-162">Request</span></span>
<span data-ttu-id="14e82-163">В следующем примере изменяется сотрудник расписание, чтобы иметь по понедельникам.</span><span class="sxs-lookup"><span data-stu-id="14e82-163">The following example changes the staff member's schedule to have Mondays off.</span></span>
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
##### <a name="response"></a><span data-ttu-id="14e82-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="14e82-164">Response</span></span>
<span data-ttu-id="14e82-165">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="14e82-165">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update bookingstaffmember",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
