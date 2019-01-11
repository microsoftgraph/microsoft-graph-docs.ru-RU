---
title: Тип ресурса bookingStaffMember
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: 382da1b0710b691a6563a40c03ed62397262911d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884457"
---
# <a name="bookingstaffmember-resource-type"></a><span data-ttu-id="48d2c-104">Тип ресурса bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="48d2c-104">bookingStaffMember resource type</span></span>

 > <span data-ttu-id="48d2c-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="48d2c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="48d2c-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48d2c-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="48d2c-107">Представляет сотрудник, который предоставляет службы в [bookingBusiness](bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="48d2c-107">Represents a staff member who provides services in a [bookingBusiness](bookingbusiness.md).</span></span>

<span data-ttu-id="48d2c-108">Сотрудники могут быть частью клиента Office 355 которых настроен business резервирования, или они могут использовать службы электронной почты от других поставщиков электронной почты.</span><span class="sxs-lookup"><span data-stu-id="48d2c-108">Staff members can be part of the Office 355 tenant where the booking business is configured, or they can use email services from other email providers.</span></span>

<span data-ttu-id="48d2c-109">Когда резервирования встреч, API резервирования рассматривает следующие параметры для определения доступности сотрудника:</span><span class="sxs-lookup"><span data-stu-id="48d2c-109">When booking appointments, the Bookings API considers the following settings to determine a staff member's availability:</span></span> 

1. <span data-ttu-id="48d2c-110">По умолчанию режим работы бизнеса (свойство **businessHours** сущности [bookingBusiness](bookingbusiness.md) ) представляет общей доступности сотрудника.</span><span class="sxs-lookup"><span data-stu-id="48d2c-110">By default, the hours of operation of the business (the **businessHours** property of the [bookingBusiness](bookingbusiness.md) entity) represents the general availability of the staff member.</span></span>
2. <span data-ttu-id="48d2c-111">Если **useBusinessHours** имеет значение false, сотрудник определенных рабочих часов (свойство**workingHours** сущности **bookingStaffmember** ) представляет общей доступности этого элемента.</span><span class="sxs-lookup"><span data-stu-id="48d2c-111">If **useBusinessHours** is false, then the staff member's specific work hours (**workingHours** property of the **bookingStaffmember** entity) represents that member's general availability.</span></span>
3. <span data-ttu-id="48d2c-112">При **availabilityIsAffectedByPersonalCalendar** имеет значение true, затем API резервирования будет сначала откроете сотрудник общедоступной часов (в соответствии с #1 или #2) и убедитесь доступности часам в личный член персонала календарь перед внесением резервирования.</span><span class="sxs-lookup"><span data-stu-id="48d2c-112">If **availabilityIsAffectedByPersonalCalendar** is true, then the Bookings API would first look at the staff member's generally available hours (as determined by either #1 or #2), and verify availability during those hours in the staff member's personal calendar, before making a booking.</span></span>

## <a name="methods"></a><span data-ttu-id="48d2c-113">Методы</span><span class="sxs-lookup"><span data-stu-id="48d2c-113">Methods</span></span>

| <span data-ttu-id="48d2c-114">Метод</span><span class="sxs-lookup"><span data-stu-id="48d2c-114">Method</span></span>           | <span data-ttu-id="48d2c-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="48d2c-115">Return Type</span></span>    |<span data-ttu-id="48d2c-116">Описание</span><span class="sxs-lookup"><span data-stu-id="48d2c-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="48d2c-117">Список сотрудников</span><span class="sxs-lookup"><span data-stu-id="48d2c-117">List staff members</span></span>](../api/bookingbusiness-list-staffmembers.md) | <span data-ttu-id="48d2c-118">[bookingStaffMember](bookingstaffmember.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="48d2c-118">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="48d2c-119">Получите список объектов **bookingStaffMember** в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="48d2c-119">Get a list of **bookingStaffMember** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="48d2c-120">Создание bookingStaff</span><span class="sxs-lookup"><span data-stu-id="48d2c-120">Create bookingStaff</span></span>](../api/bookingbusiness-post-staffmembers.md) | <span data-ttu-id="48d2c-121">[bookingStaffMember](bookingstaffmember.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="48d2c-121">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="48d2c-122">Создание нового **bookingStaffMember** в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="48d2c-122">Create a new **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="48d2c-123">Получение bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="48d2c-123">Get bookingStaffMember</span></span>](../api/bookingstaffmember-get.md) | [<span data-ttu-id="48d2c-124">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="48d2c-124">bookingStaffMember</span></span>](bookingstaffmember.md) |<span data-ttu-id="48d2c-125">Получите свойства и связи **bookingStaffMember** в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="48d2c-125">Get the properties and relationships of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|<span data-ttu-id="48d2c-126">[обновление](../api/bookingstaffmember-update.md).</span><span class="sxs-lookup"><span data-stu-id="48d2c-126">[Update](../api/bookingstaffmember-update.md)</span></span> | [<span data-ttu-id="48d2c-127">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="48d2c-127">bookingStaffMember</span></span>](bookingstaffmember.md)    |<span data-ttu-id="48d2c-128">Обновление свойств **bookingStaffMember** в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="48d2c-128">Update the properties of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="48d2c-129">Delete</span><span class="sxs-lookup"><span data-stu-id="48d2c-129">Delete</span></span>](../api/bookingstaffmember-delete.md) | <span data-ttu-id="48d2c-130">Нет</span><span class="sxs-lookup"><span data-stu-id="48d2c-130">None</span></span> |<span data-ttu-id="48d2c-131">Удалите сотрудник в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="48d2c-131">Delete a staff member in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="48d2c-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="48d2c-132">Properties</span></span>
| <span data-ttu-id="48d2c-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="48d2c-133">Property</span></span>     | <span data-ttu-id="48d2c-134">Тип</span><span class="sxs-lookup"><span data-stu-id="48d2c-134">Type</span></span>   |<span data-ttu-id="48d2c-135">Описание</span><span class="sxs-lookup"><span data-stu-id="48d2c-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48d2c-136">availabilityIsAffectedByPersonalCalendar</span><span class="sxs-lookup"><span data-stu-id="48d2c-136">availabilityIsAffectedByPersonalCalendar</span></span>|<span data-ttu-id="48d2c-137">Логический</span><span class="sxs-lookup"><span data-stu-id="48d2c-137">Boolean</span></span>|<span data-ttu-id="48d2c-138">Значение true означает, что если сотрудник является пользователь Office 365, API резервирования будет проверки доступности сотрудника на свой личный календарь в Office 365 перед внесением резервирования.</span><span class="sxs-lookup"><span data-stu-id="48d2c-138">True means that if the staff member is an Office 365 user, the Bookings API would verify the staff member's availability in their personal calendar in Office 365, before making a booking.</span></span> |
|<span data-ttu-id="48d2c-139">ColorIndex (en)</span><span class="sxs-lookup"><span data-stu-id="48d2c-139">colorIndex</span></span>|<span data-ttu-id="48d2c-140">Int32</span><span class="sxs-lookup"><span data-stu-id="48d2c-140">Int32</span></span>|<span data-ttu-id="48d2c-141">Определяет цвет сотрудника.</span><span class="sxs-lookup"><span data-stu-id="48d2c-141">Identifies a color to represent the staff member.</span></span> <span data-ttu-id="48d2c-142">Цвет соответствует цветовой палитры на странице **сведений о персонала** в приложении резервирования.</span><span class="sxs-lookup"><span data-stu-id="48d2c-142">The color corresponds to the color palette in the **Staff details** page in the Bookings app.</span></span>|
|<span data-ttu-id="48d2c-143">displayName</span><span class="sxs-lookup"><span data-stu-id="48d2c-143">displayName</span></span>|<span data-ttu-id="48d2c-144">Строка</span><span class="sxs-lookup"><span data-stu-id="48d2c-144">String</span></span>|<span data-ttu-id="48d2c-145">Имя сотрудника, как оно отображается для клиентов.</span><span class="sxs-lookup"><span data-stu-id="48d2c-145">The name of the staff member, as displayed to customers.</span></span> <span data-ttu-id="48d2c-146">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48d2c-146">Required.</span></span>|
|<span data-ttu-id="48d2c-147">emailAddress</span><span class="sxs-lookup"><span data-stu-id="48d2c-147">emailAddress</span></span>|<span data-ttu-id="48d2c-148">String</span><span class="sxs-lookup"><span data-stu-id="48d2c-148">String</span></span>|<span data-ttu-id="48d2c-149">Адрес электронной почты сотрудника.</span><span class="sxs-lookup"><span data-stu-id="48d2c-149">The email address of the staff member.</span></span> <span data-ttu-id="48d2c-150">Это может быть в одном клиентов Office 365 как предприятию или в домене различных электронной почты.</span><span class="sxs-lookup"><span data-stu-id="48d2c-150">This can be in the same Office 365 tenant as the business, or in a different email domain.</span></span> <span data-ttu-id="48d2c-151">Можно использовать этот адрес электронной почты, если свойство **sendConfirmationsToOwner** имеет значение true в политике планирования бизнеса.</span><span class="sxs-lookup"><span data-stu-id="48d2c-151">This email address can be used if the **sendConfirmationsToOwner** property is set to true in the scheduling policy of the business.</span></span> <span data-ttu-id="48d2c-152">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48d2c-152">Required.</span></span>|
|<span data-ttu-id="48d2c-153">id</span><span class="sxs-lookup"><span data-stu-id="48d2c-153">id</span></span>|<span data-ttu-id="48d2c-154">Строка</span><span class="sxs-lookup"><span data-stu-id="48d2c-154">String</span></span>| <span data-ttu-id="48d2c-155">Идентификатор сотрудника в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="48d2c-155">The ID of the staff member, in a GUID format.</span></span> <span data-ttu-id="48d2c-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="48d2c-156">Read-only.</span></span>|
|<span data-ttu-id="48d2c-157">role</span><span class="sxs-lookup"><span data-stu-id="48d2c-157">role</span></span>|<span data-ttu-id="48d2c-158">string</span><span class="sxs-lookup"><span data-stu-id="48d2c-158">string</span></span>| <span data-ttu-id="48d2c-159">Роль сотрудника в организации.</span><span class="sxs-lookup"><span data-stu-id="48d2c-159">The role of the staff member in the business.</span></span> <span data-ttu-id="48d2c-160">Возможные значения: `guest`, `administrator`, `viewer`, `externalGuest`.</span><span class="sxs-lookup"><span data-stu-id="48d2c-160">Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.</span></span> <span data-ttu-id="48d2c-161">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48d2c-161">Required.</span></span>|
|<span data-ttu-id="48d2c-162">useBusinessHours</span><span class="sxs-lookup"><span data-stu-id="48d2c-162">useBusinessHours</span></span>|<span data-ttu-id="48d2c-163">Логический</span><span class="sxs-lookup"><span data-stu-id="48d2c-163">Boolean</span></span>|<span data-ttu-id="48d2c-164">Имеет значение true означает, что сотрудник доступность — как указанных в свойстве **businessHours** бизнеса.</span><span class="sxs-lookup"><span data-stu-id="48d2c-164">True means the staff member's availability is as specified in the **businessHours** property of the business.</span></span> <span data-ttu-id="48d2c-165">False означает, что доступность определяется значение свойства **workingHours** сотрудника.</span><span class="sxs-lookup"><span data-stu-id="48d2c-165">False means the availability is determined by the staff member's **workingHours** property setting.</span></span>|
|<span data-ttu-id="48d2c-166">workingHours</span><span class="sxs-lookup"><span data-stu-id="48d2c-166">workingHours</span></span>|<span data-ttu-id="48d2c-167">[bookingWorkHours](bookingworkhours.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="48d2c-167">[bookingWorkHours](bookingworkhours.md) collection</span></span>|<span data-ttu-id="48d2c-168">Диапазон часов каждый день недели, по которым сотрудник доступна для резервирования.</span><span class="sxs-lookup"><span data-stu-id="48d2c-168">The range of hours each day of the week that the staff member is available for booking.</span></span> <span data-ttu-id="48d2c-169">По умолчанию они инициализируются совпадает со значением свойства **businessHours** бизнеса.</span><span class="sxs-lookup"><span data-stu-id="48d2c-169">By default, they are initialized to be the same as the **businessHours** property of the business.</span></span>|

## <a name="relationships"></a><span data-ttu-id="48d2c-170">Связи</span><span class="sxs-lookup"><span data-stu-id="48d2c-170">Relationships</span></span>
<span data-ttu-id="48d2c-171">Нет</span><span class="sxs-lookup"><span data-stu-id="48d2c-171">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="48d2c-172">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="48d2c-172">JSON representation</span></span>

<span data-ttu-id="48d2c-173">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48d2c-173">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "bookingStaffMember resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
