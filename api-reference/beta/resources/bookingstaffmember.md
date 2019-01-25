---
title: Тип ресурса bookingStaffMember
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 72130f46dc67d4491f9855706528ee5894b8352f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520279"
---
# <a name="bookingstaffmember-resource-type"></a><span data-ttu-id="b1341-104">Тип ресурса bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="b1341-104">bookingStaffMember resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="b1341-105">Представляет сотрудник, который предоставляет службы в [bookingBusiness](bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="b1341-105">Represents a staff member who provides services in a [bookingBusiness](bookingbusiness.md).</span></span>

<span data-ttu-id="b1341-106">Сотрудники могут быть частью клиента Office 355 которых настроен business резервирования, или они могут использовать службы электронной почты от других поставщиков электронной почты.</span><span class="sxs-lookup"><span data-stu-id="b1341-106">Staff members can be part of the Office 355 tenant where the booking business is configured, or they can use email services from other email providers.</span></span>

<span data-ttu-id="b1341-107">Когда резервирования встреч, API резервирования рассматривает следующие параметры для определения доступности сотрудника:</span><span class="sxs-lookup"><span data-stu-id="b1341-107">When booking appointments, the Bookings API considers the following settings to determine a staff member's availability:</span></span> 

1. <span data-ttu-id="b1341-108">По умолчанию режим работы бизнеса (свойство **businessHours** сущности [bookingBusiness](bookingbusiness.md) ) представляет общей доступности сотрудника.</span><span class="sxs-lookup"><span data-stu-id="b1341-108">By default, the hours of operation of the business (the **businessHours** property of the [bookingBusiness](bookingbusiness.md) entity) represents the general availability of the staff member.</span></span>
2. <span data-ttu-id="b1341-109">Если **useBusinessHours** имеет значение false, сотрудник определенных рабочих часов (свойство**workingHours** сущности **bookingStaffmember** ) представляет общей доступности этого элемента.</span><span class="sxs-lookup"><span data-stu-id="b1341-109">If **useBusinessHours** is false, then the staff member's specific work hours (**workingHours** property of the **bookingStaffmember** entity) represents that member's general availability.</span></span>
3. <span data-ttu-id="b1341-110">При **availabilityIsAffectedByPersonalCalendar** имеет значение true, затем API резервирования будет сначала откроете сотрудник общедоступной часов (в соответствии с #1 или #2) и убедитесь доступности часам в личный член персонала календарь перед внесением резервирования.</span><span class="sxs-lookup"><span data-stu-id="b1341-110">If **availabilityIsAffectedByPersonalCalendar** is true, then the Bookings API would first look at the staff member's generally available hours (as determined by either #1 or #2), and verify availability during those hours in the staff member's personal calendar, before making a booking.</span></span>

## <a name="methods"></a><span data-ttu-id="b1341-111">Методы</span><span class="sxs-lookup"><span data-stu-id="b1341-111">Methods</span></span>

| <span data-ttu-id="b1341-112">Метод</span><span class="sxs-lookup"><span data-stu-id="b1341-112">Method</span></span>           | <span data-ttu-id="b1341-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b1341-113">Return Type</span></span>    |<span data-ttu-id="b1341-114">Описание</span><span class="sxs-lookup"><span data-stu-id="b1341-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b1341-115">Список сотрудников</span><span class="sxs-lookup"><span data-stu-id="b1341-115">List staff members</span></span>](../api/bookingbusiness-list-staffmembers.md) | <span data-ttu-id="b1341-116">[bookingStaffMember](bookingstaffmember.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="b1341-116">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="b1341-117">Получите список объектов **bookingStaffMember** в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="b1341-117">Get a list of **bookingStaffMember** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="b1341-118">Создание bookingStaff</span><span class="sxs-lookup"><span data-stu-id="b1341-118">Create bookingStaff</span></span>](../api/bookingbusiness-post-staffmembers.md) | <span data-ttu-id="b1341-119">[bookingStaffMember](bookingstaffmember.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="b1341-119">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="b1341-120">Создание нового **bookingStaffMember** в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="b1341-120">Create a new **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="b1341-121">Получение bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="b1341-121">Get bookingStaffMember</span></span>](../api/bookingstaffmember-get.md) | [<span data-ttu-id="b1341-122">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="b1341-122">bookingStaffMember</span></span>](bookingstaffmember.md) |<span data-ttu-id="b1341-123">Получите свойства и связи **bookingStaffMember** в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="b1341-123">Get the properties and relationships of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="b1341-124">Update</span><span class="sxs-lookup"><span data-stu-id="b1341-124">Update</span></span>](../api/bookingstaffmember-update.md) | [<span data-ttu-id="b1341-125">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="b1341-125">bookingStaffMember</span></span>](bookingstaffmember.md)    |<span data-ttu-id="b1341-126">Обновление свойств **bookingStaffMember** в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="b1341-126">Update the properties of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="b1341-127">Delete</span><span class="sxs-lookup"><span data-stu-id="b1341-127">Delete</span></span>](../api/bookingstaffmember-delete.md) | <span data-ttu-id="b1341-128">Нет</span><span class="sxs-lookup"><span data-stu-id="b1341-128">None</span></span> |<span data-ttu-id="b1341-129">Удалите сотрудник в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="b1341-129">Delete a staff member in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="b1341-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="b1341-130">Properties</span></span>
| <span data-ttu-id="b1341-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1341-131">Property</span></span>     | <span data-ttu-id="b1341-132">Тип</span><span class="sxs-lookup"><span data-stu-id="b1341-132">Type</span></span>   |<span data-ttu-id="b1341-133">Описание</span><span class="sxs-lookup"><span data-stu-id="b1341-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1341-134">availabilityIsAffectedByPersonalCalendar</span><span class="sxs-lookup"><span data-stu-id="b1341-134">availabilityIsAffectedByPersonalCalendar</span></span>|<span data-ttu-id="b1341-135">Логическое</span><span class="sxs-lookup"><span data-stu-id="b1341-135">Boolean</span></span>|<span data-ttu-id="b1341-136">Значение true означает, что если сотрудник является пользователь Office 365, API резервирования будет проверки доступности сотрудника на свой личный календарь в Office 365 перед внесением резервирования.</span><span class="sxs-lookup"><span data-stu-id="b1341-136">True means that if the staff member is an Office 365 user, the Bookings API would verify the staff member's availability in their personal calendar in Office 365, before making a booking.</span></span> |
|<span data-ttu-id="b1341-137">ColorIndex</span><span class="sxs-lookup"><span data-stu-id="b1341-137">colorIndex</span></span>|<span data-ttu-id="b1341-138">Int32</span><span class="sxs-lookup"><span data-stu-id="b1341-138">Int32</span></span>|<span data-ttu-id="b1341-139">Определяет цвет сотрудника.</span><span class="sxs-lookup"><span data-stu-id="b1341-139">Identifies a color to represent the staff member.</span></span> <span data-ttu-id="b1341-140">Цвет соответствует цветовой палитры на странице **сведений о персонала** в приложении резервирования.</span><span class="sxs-lookup"><span data-stu-id="b1341-140">The color corresponds to the color palette in the **Staff details** page in the Bookings app.</span></span>|
|<span data-ttu-id="b1341-141">displayName</span><span class="sxs-lookup"><span data-stu-id="b1341-141">displayName</span></span>|<span data-ttu-id="b1341-142">String</span><span class="sxs-lookup"><span data-stu-id="b1341-142">String</span></span>|<span data-ttu-id="b1341-143">Имя сотрудника, как оно отображается для клиентов.</span><span class="sxs-lookup"><span data-stu-id="b1341-143">The name of the staff member, as displayed to customers.</span></span> <span data-ttu-id="b1341-144">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1341-144">Required.</span></span>|
|<span data-ttu-id="b1341-145">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b1341-145">emailAddress</span></span>|<span data-ttu-id="b1341-146">String</span><span class="sxs-lookup"><span data-stu-id="b1341-146">String</span></span>|<span data-ttu-id="b1341-147">Адрес электронной почты сотрудника.</span><span class="sxs-lookup"><span data-stu-id="b1341-147">The email address of the staff member.</span></span> <span data-ttu-id="b1341-148">Это может быть в одном клиентов Office 365 как предприятию или в домене различных электронной почты.</span><span class="sxs-lookup"><span data-stu-id="b1341-148">This can be in the same Office 365 tenant as the business, or in a different email domain.</span></span> <span data-ttu-id="b1341-149">Можно использовать этот адрес электронной почты, если свойство **sendConfirmationsToOwner** имеет значение true в политике планирования бизнеса.</span><span class="sxs-lookup"><span data-stu-id="b1341-149">This email address can be used if the **sendConfirmationsToOwner** property is set to true in the scheduling policy of the business.</span></span> <span data-ttu-id="b1341-150">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1341-150">Required.</span></span>|
|<span data-ttu-id="b1341-151">id</span><span class="sxs-lookup"><span data-stu-id="b1341-151">id</span></span>|<span data-ttu-id="b1341-152">Строка</span><span class="sxs-lookup"><span data-stu-id="b1341-152">String</span></span>| <span data-ttu-id="b1341-153">Идентификатор сотрудника в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="b1341-153">The ID of the staff member, in a GUID format.</span></span> <span data-ttu-id="b1341-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b1341-154">Read-only.</span></span>|
|<span data-ttu-id="b1341-155">role</span><span class="sxs-lookup"><span data-stu-id="b1341-155">role</span></span>|<span data-ttu-id="b1341-156">string</span><span class="sxs-lookup"><span data-stu-id="b1341-156">string</span></span>| <span data-ttu-id="b1341-157">Роль сотрудника в организации.</span><span class="sxs-lookup"><span data-stu-id="b1341-157">The role of the staff member in the business.</span></span> <span data-ttu-id="b1341-158">Возможные значения: `guest`, `administrator`, `viewer`, `externalGuest`.</span><span class="sxs-lookup"><span data-stu-id="b1341-158">Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.</span></span> <span data-ttu-id="b1341-159">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1341-159">Required.</span></span>|
|<span data-ttu-id="b1341-160">useBusinessHours</span><span class="sxs-lookup"><span data-stu-id="b1341-160">useBusinessHours</span></span>|<span data-ttu-id="b1341-161">Логическое</span><span class="sxs-lookup"><span data-stu-id="b1341-161">Boolean</span></span>|<span data-ttu-id="b1341-162">Имеет значение true означает, что сотрудник доступность — как указанных в свойстве **businessHours** бизнеса.</span><span class="sxs-lookup"><span data-stu-id="b1341-162">True means the staff member's availability is as specified in the **businessHours** property of the business.</span></span> <span data-ttu-id="b1341-163">False означает, что доступность определяется значение свойства **workingHours** сотрудника.</span><span class="sxs-lookup"><span data-stu-id="b1341-163">False means the availability is determined by the staff member's **workingHours** property setting.</span></span>|
|<span data-ttu-id="b1341-164">workingHours</span><span class="sxs-lookup"><span data-stu-id="b1341-164">workingHours</span></span>|<span data-ttu-id="b1341-165">[bookingWorkHours](bookingworkhours.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="b1341-165">[bookingWorkHours](bookingworkhours.md) collection</span></span>|<span data-ttu-id="b1341-166">Диапазон часов каждый день недели, по которым сотрудник доступна для резервирования.</span><span class="sxs-lookup"><span data-stu-id="b1341-166">The range of hours each day of the week that the staff member is available for booking.</span></span> <span data-ttu-id="b1341-167">По умолчанию они инициализируются совпадает со значением свойства **businessHours** бизнеса.</span><span class="sxs-lookup"><span data-stu-id="b1341-167">By default, they are initialized to be the same as the **businessHours** property of the business.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1341-168">Отношения</span><span class="sxs-lookup"><span data-stu-id="b1341-168">Relationships</span></span>
<span data-ttu-id="b1341-169">Нет</span><span class="sxs-lookup"><span data-stu-id="b1341-169">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b1341-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b1341-170">JSON representation</span></span>

<span data-ttu-id="b1341-171">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b1341-171">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingStaffMember"
}-->

```json
{
  "availabilityIsAffectedByPersonalCalendar": true,
  "colorIndex": 1024,
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)",
  "role": "string",
  "useBusinessHours": true,
  "workingHours": [{"@odata.type": "microsoft.graph.bookingWorkHours"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingStaffMember resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingstaffmember.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
