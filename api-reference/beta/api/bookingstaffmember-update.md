---
title: Обновление bookingstaffmember
description: Обновление свойств bookingStaffMember в указанном bookingbusiness.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 608580a16d796a4ee1b296c0a19caea110326cff
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514560"
---
# <a name="update-bookingstaffmember"></a><span data-ttu-id="3829a-103">Обновление bookingstaffmember</span><span class="sxs-lookup"><span data-stu-id="3829a-103">Update bookingstaffmember</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3829a-104">Обновление свойств [bookingStaffMember](../resources/bookingstaffmember.md) в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="3829a-104">Update the properties of a [bookingStaffMember](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="3829a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3829a-105">Permissions</span></span>
<span data-ttu-id="3829a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3829a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3829a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3829a-108">Permission type</span></span>      | <span data-ttu-id="3829a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3829a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3829a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3829a-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="3829a-111">Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="3829a-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="3829a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3829a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3829a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3829a-113">Not supported.</span></span>   |
|<span data-ttu-id="3829a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3829a-114">Application</span></span> | <span data-ttu-id="3829a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3829a-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="3829a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3829a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/staffMembers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="3829a-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3829a-117">Optional request headers</span></span>
| <span data-ttu-id="3829a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="3829a-118">Name</span></span>       | <span data-ttu-id="3829a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="3829a-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3829a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3829a-120">Authorization</span></span>  | <span data-ttu-id="3829a-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3829a-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="3829a-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3829a-122">Request body</span></span>
<span data-ttu-id="3829a-p102">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="3829a-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3829a-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="3829a-126">Property</span></span>     | <span data-ttu-id="3829a-127">Тип</span><span class="sxs-lookup"><span data-stu-id="3829a-127">Type</span></span>   |<span data-ttu-id="3829a-128">Описание</span><span class="sxs-lookup"><span data-stu-id="3829a-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3829a-129">availabilityIsAffectedByPersonalCalendar</span><span class="sxs-lookup"><span data-stu-id="3829a-129">availabilityIsAffectedByPersonalCalendar</span></span>|<span data-ttu-id="3829a-130">Логическое</span><span class="sxs-lookup"><span data-stu-id="3829a-130">Boolean</span></span>|<span data-ttu-id="3829a-131">Значение true означает, что если сотрудник является пользователь Office 365, API резервирования применяет сотрудник личного календаря в Office 365, а также свойство **workingHours** для определения доступности.</span><span class="sxs-lookup"><span data-stu-id="3829a-131">True means that if the staff member is an Office 365 user, the Bookings API uses the staff member's personal calendar in Office 365 as well as the **workingHours** property to determine availability.</span></span> |
|<span data-ttu-id="3829a-132">ColorIndex</span><span class="sxs-lookup"><span data-stu-id="3829a-132">colorIndex</span></span>|<span data-ttu-id="3829a-133">Int32</span><span class="sxs-lookup"><span data-stu-id="3829a-133">Int32</span></span>|<span data-ttu-id="3829a-134">Определяет цвет сотрудника.</span><span class="sxs-lookup"><span data-stu-id="3829a-134">Identifies a color to represent the staff member.</span></span> <span data-ttu-id="3829a-135">Цвет соответствует цветовой палитры на странице **сведений о персонала** в приложении резервирования.</span><span class="sxs-lookup"><span data-stu-id="3829a-135">The color corresponds to the color palette in the **Staff details** page in the Bookings app.</span></span>|
|<span data-ttu-id="3829a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3829a-136">displayName</span></span>|<span data-ttu-id="3829a-137">Строка</span><span class="sxs-lookup"><span data-stu-id="3829a-137">String</span></span>|<span data-ttu-id="3829a-138">Имя сотрудника, как оно отображается для клиентов.</span><span class="sxs-lookup"><span data-stu-id="3829a-138">The name of the staff member, as displayed to customers.</span></span>|
|<span data-ttu-id="3829a-139">emailAddress</span><span class="sxs-lookup"><span data-stu-id="3829a-139">emailAddress</span></span>|<span data-ttu-id="3829a-140">String</span><span class="sxs-lookup"><span data-stu-id="3829a-140">String</span></span>|<span data-ttu-id="3829a-141">Адрес электронной почты сотрудника.</span><span class="sxs-lookup"><span data-stu-id="3829a-141">The email address of the staff member.</span></span> <span data-ttu-id="3829a-142">Это может быть в одном клиентов Office 365 как предприятию или в домене различных электронной почты.</span><span class="sxs-lookup"><span data-stu-id="3829a-142">This can be in the same Office 365 tenant as the business, or in a different email domain.</span></span> <span data-ttu-id="3829a-143">Этот адрес электронной почты используется, если свойство **sendConfirmationsToOwner** имеет значение true в политике планирования бизнеса.</span><span class="sxs-lookup"><span data-stu-id="3829a-143">This email address is used if the **sendConfirmationsToOwner** property is set to true in the scheduling policy of the business.</span></span>|
|<span data-ttu-id="3829a-144">role</span><span class="sxs-lookup"><span data-stu-id="3829a-144">role</span></span>|<span data-ttu-id="3829a-145">string</span><span class="sxs-lookup"><span data-stu-id="3829a-145">string</span></span>| <span data-ttu-id="3829a-146">Роль сотрудника в организации.</span><span class="sxs-lookup"><span data-stu-id="3829a-146">The role of the staff member in the business.</span></span> <span data-ttu-id="3829a-147">Возможные значения: `guest`, `administrator`, `viewer`, `externalGuest`.</span><span class="sxs-lookup"><span data-stu-id="3829a-147">Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.</span></span>|
|<span data-ttu-id="3829a-148">useBusinessHours</span><span class="sxs-lookup"><span data-stu-id="3829a-148">useBusinessHours</span></span>|<span data-ttu-id="3829a-149">Логическое</span><span class="sxs-lookup"><span data-stu-id="3829a-149">Boolean</span></span>|<span data-ttu-id="3829a-150">Значение true означает, что сотрудник доступность определяется свойством **businessHours** бизнеса.</span><span class="sxs-lookup"><span data-stu-id="3829a-150">True means the staff member's availability is determined by the **businessHours** property of the business.</span></span> <span data-ttu-id="3829a-151">False означает, что доступность определяется значение свойства **workingHouse** сотрудника.</span><span class="sxs-lookup"><span data-stu-id="3829a-151">False means the availability is determined by the staff member's **workingHouse** property setting.</span></span>|
|<span data-ttu-id="3829a-152">workingHours</span><span class="sxs-lookup"><span data-stu-id="3829a-152">workingHours</span></span>|<span data-ttu-id="3829a-153">[bookingWorkHours](../resources/bookingworkhours.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="3829a-153">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="3829a-154">Диапазон часов каждый день недели, по которым сотрудник доступна для резервирования.</span><span class="sxs-lookup"><span data-stu-id="3829a-154">The range of hours each day of the week that the staff member is available for booking.</span></span>|

## <a name="response"></a><span data-ttu-id="3829a-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="3829a-155">Response</span></span>
<span data-ttu-id="3829a-p107">При успешном выполнении этот метод возвращает код отклика `204 No content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3829a-p107">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3829a-158">Пример</span><span class="sxs-lookup"><span data-stu-id="3829a-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3829a-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="3829a-159">Request</span></span>
<span data-ttu-id="3829a-160">В следующем примере изменяется сотрудник расписание, чтобы иметь по понедельникам.</span><span class="sxs-lookup"><span data-stu-id="3829a-160">The following example changes the staff member's schedule to have Mondays off.</span></span>
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
##### <a name="response"></a><span data-ttu-id="3829a-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="3829a-161">Response</span></span>
<span data-ttu-id="3829a-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3829a-162">The following is an example of the response.</span></span>
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
    "Error: /api-reference/beta/api/bookingstaffmember-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
