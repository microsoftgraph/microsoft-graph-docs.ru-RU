---
title: Тип ресурса Букингстаффмембер
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 1de32728aff808975efd3121c9fd99fd0819b06c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013089"
---
# <a name="bookingstaffmember-resource-type"></a><span data-ttu-id="14935-104">Тип ресурса Букингстаффмембер</span><span class="sxs-lookup"><span data-stu-id="14935-104">bookingStaffMember resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="14935-105">Представляет сотрудника, который предоставляет службы в [букингбусинесс](bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="14935-105">Represents a staff member who provides services in a [bookingBusiness](bookingbusiness.md).</span></span>

<span data-ttu-id="14935-106">Сотрудники могут входить в состав клиента Office 355, на котором настроена Настройка бизнеса, или они могут использовать службы электронной почты от других поставщиков услуг электронной почты.</span><span class="sxs-lookup"><span data-stu-id="14935-106">Staff members can be part of the Office 355 tenant where the booking business is configured, or they can use email services from other email providers.</span></span>

<span data-ttu-id="14935-107">При резервировании встреч API учета рассматривает следующие параметры для определения доступности сотрудников:</span><span class="sxs-lookup"><span data-stu-id="14935-107">When booking appointments, the Bookings API considers the following settings to determine a staff member's availability:</span></span> 

1. <span data-ttu-id="14935-108">По умолчанию часы работы бизнеса (свойство **businessHours** объекта [букингбусинесс](bookingbusiness.md) ) представляют общую доступность сотрудника.</span><span class="sxs-lookup"><span data-stu-id="14935-108">By default, the hours of operation of the business (the **businessHours** property of the [bookingBusiness](bookingbusiness.md) entity) represents the general availability of the staff member.</span></span>
2. <span data-ttu-id="14935-109">Если **усебусинесшаурс** имеет значение false, то характер рабочего времени сотрудника (свойства**воркингхаурс** объекта **букингстаффмембер** ) представляет общую доступность этого члена.</span><span class="sxs-lookup"><span data-stu-id="14935-109">If **useBusinessHours** is false, then the staff member's specific work hours (**workingHours** property of the **bookingStaffmember** entity) represents that member's general availability.</span></span>
3. <span data-ttu-id="14935-110">Если **аваилабилитисаффектедбиперсоналкалендар** имеет значение true, то API для работы с книгами сначала рассмотрю общедоступные часы сотрудника (как определено в #1 или #2), а также проверяйте доступность в течение этих часов в личном элементе сотрудника. Календарь, перед выполнением резервирования.</span><span class="sxs-lookup"><span data-stu-id="14935-110">If **availabilityIsAffectedByPersonalCalendar** is true, then the Bookings API would first look at the staff member's generally available hours (as determined by either #1 or #2), and verify availability during those hours in the staff member's personal calendar, before making a booking.</span></span>

## <a name="methods"></a><span data-ttu-id="14935-111">Методы</span><span class="sxs-lookup"><span data-stu-id="14935-111">Methods</span></span>

| <span data-ttu-id="14935-112">Метод</span><span class="sxs-lookup"><span data-stu-id="14935-112">Method</span></span>           | <span data-ttu-id="14935-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="14935-113">Return Type</span></span>    |<span data-ttu-id="14935-114">Описание</span><span class="sxs-lookup"><span data-stu-id="14935-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="14935-115">Список сотрудников</span><span class="sxs-lookup"><span data-stu-id="14935-115">List staff members</span></span>](../api/bookingbusiness-list-staffmembers.md) | <span data-ttu-id="14935-116">Коллекция [букингстаффмембер](bookingstaffmember.md)</span><span class="sxs-lookup"><span data-stu-id="14935-116">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="14935-117">Получение списка объектов **букингстаффмембер** в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="14935-117">Get a list of **bookingStaffMember** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="14935-118">Создание Букингстафф</span><span class="sxs-lookup"><span data-stu-id="14935-118">Create bookingStaff</span></span>](../api/bookingbusiness-post-staffmembers.md) | <span data-ttu-id="14935-119">Коллекция [букингстаффмембер](bookingstaffmember.md)</span><span class="sxs-lookup"><span data-stu-id="14935-119">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="14935-120">Создание нового **букингстаффмембер** в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="14935-120">Create a new **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="14935-121">Получение Букингстаффмембер</span><span class="sxs-lookup"><span data-stu-id="14935-121">Get bookingStaffMember</span></span>](../api/bookingstaffmember-get.md) | [<span data-ttu-id="14935-122">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="14935-122">bookingStaffMember</span></span>](bookingstaffmember.md) |<span data-ttu-id="14935-123">Получение свойств и связей объекта **букингстаффмембер** в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="14935-123">Get the properties and relationships of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|<span data-ttu-id="14935-124">[обновление](../api/bookingstaffmember-update.md);</span><span class="sxs-lookup"><span data-stu-id="14935-124">[Update](../api/bookingstaffmember-update.md)</span></span> | [<span data-ttu-id="14935-125">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="14935-125">bookingStaffMember</span></span>](bookingstaffmember.md)    |<span data-ttu-id="14935-126">Обновление свойств объекта **букингстаффмембер** в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="14935-126">Update the properties of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="14935-127">Удаление</span><span class="sxs-lookup"><span data-stu-id="14935-127">Delete</span></span>](../api/bookingstaffmember-delete.md) | <span data-ttu-id="14935-128">Нет</span><span class="sxs-lookup"><span data-stu-id="14935-128">None</span></span> |<span data-ttu-id="14935-129">Удаление сотрудника в заданном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="14935-129">Delete a staff member in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="14935-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="14935-130">Properties</span></span>
| <span data-ttu-id="14935-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="14935-131">Property</span></span>     | <span data-ttu-id="14935-132">Тип</span><span class="sxs-lookup"><span data-stu-id="14935-132">Type</span></span>   |<span data-ttu-id="14935-133">Описание</span><span class="sxs-lookup"><span data-stu-id="14935-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="14935-134">Аваилабилитисаффектедбиперсоналкалендар</span><span class="sxs-lookup"><span data-stu-id="14935-134">availabilityIsAffectedByPersonalCalendar</span></span>|<span data-ttu-id="14935-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="14935-135">Boolean</span></span>|<span data-ttu-id="14935-136">True означает, что если сотрудник является пользователем Office 365, то API для резервирования будет проверять доступность сотрудников в личном календаре в Office 365 перед выполнением резервирования.</span><span class="sxs-lookup"><span data-stu-id="14935-136">True means that if the staff member is an Office 365 user, the Bookings API would verify the staff member's availability in their personal calendar in Office 365, before making a booking.</span></span> |
|<span data-ttu-id="14935-137">colorIndex</span><span class="sxs-lookup"><span data-stu-id="14935-137">colorIndex</span></span>|<span data-ttu-id="14935-138">Int32</span><span class="sxs-lookup"><span data-stu-id="14935-138">Int32</span></span>|<span data-ttu-id="14935-139">Определяет цвет для представления сотрудника.</span><span class="sxs-lookup"><span data-stu-id="14935-139">Identifies a color to represent the staff member.</span></span> <span data-ttu-id="14935-140">Цвет соответствует цветовой палитре на странице " **сведения о персонале** " в приложении "книги".</span><span class="sxs-lookup"><span data-stu-id="14935-140">The color corresponds to the color palette in the **Staff details** page in the Bookings app.</span></span>|
|<span data-ttu-id="14935-141">displayName</span><span class="sxs-lookup"><span data-stu-id="14935-141">displayName</span></span>|<span data-ttu-id="14935-142">Строка</span><span class="sxs-lookup"><span data-stu-id="14935-142">String</span></span>|<span data-ttu-id="14935-143">Имя сотрудника, отображаемое для клиентов.</span><span class="sxs-lookup"><span data-stu-id="14935-143">The name of the staff member, as displayed to customers.</span></span> <span data-ttu-id="14935-144">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="14935-144">Required.</span></span>|
|<span data-ttu-id="14935-145">emailAddress</span><span class="sxs-lookup"><span data-stu-id="14935-145">emailAddress</span></span>|<span data-ttu-id="14935-146">String</span><span class="sxs-lookup"><span data-stu-id="14935-146">String</span></span>|<span data-ttu-id="14935-147">Адрес электронной почты сотрудника.</span><span class="sxs-lookup"><span data-stu-id="14935-147">The email address of the staff member.</span></span> <span data-ttu-id="14935-148">Это может быть тот же клиент Office 365, что и в Организации, или в другом домене электронной почты.</span><span class="sxs-lookup"><span data-stu-id="14935-148">This can be in the same Office 365 tenant as the business, or in a different email domain.</span></span> <span data-ttu-id="14935-149">Этот адрес электронной почты можно использовать, если для свойства **сендконфирматионстувнер** в политике планирования бизнеса задано значение true.</span><span class="sxs-lookup"><span data-stu-id="14935-149">This email address can be used if the **sendConfirmationsToOwner** property is set to true in the scheduling policy of the business.</span></span> <span data-ttu-id="14935-150">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14935-150">Required.</span></span>|
|<span data-ttu-id="14935-151">id</span><span class="sxs-lookup"><span data-stu-id="14935-151">id</span></span>|<span data-ttu-id="14935-152">String</span><span class="sxs-lookup"><span data-stu-id="14935-152">String</span></span>| <span data-ttu-id="14935-153">Идентификатор сотрудника в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="14935-153">The ID of the staff member, in a GUID format.</span></span> <span data-ttu-id="14935-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="14935-154">Read-only.</span></span>|
|<span data-ttu-id="14935-155">role</span><span class="sxs-lookup"><span data-stu-id="14935-155">role</span></span>|<span data-ttu-id="14935-156">string</span><span class="sxs-lookup"><span data-stu-id="14935-156">string</span></span>| <span data-ttu-id="14935-157">Роль сотрудника в Организации.</span><span class="sxs-lookup"><span data-stu-id="14935-157">The role of the staff member in the business.</span></span> <span data-ttu-id="14935-158">Возможные значения: `guest`, `administrator`, `viewer`, `externalGuest`.</span><span class="sxs-lookup"><span data-stu-id="14935-158">Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.</span></span> <span data-ttu-id="14935-159">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="14935-159">Required.</span></span>|
|<span data-ttu-id="14935-160">Усебусинесшаурс</span><span class="sxs-lookup"><span data-stu-id="14935-160">useBusinessHours</span></span>|<span data-ttu-id="14935-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="14935-161">Boolean</span></span>|<span data-ttu-id="14935-162">Значение true означает, что уровень доступности сотрудника указан в свойстве **businessHours** предприятия.</span><span class="sxs-lookup"><span data-stu-id="14935-162">True means the staff member's availability is as specified in the **businessHours** property of the business.</span></span> <span data-ttu-id="14935-163">Значение false означает, что доступность определяется значением свойства **воркингхаурс** сотрудника.</span><span class="sxs-lookup"><span data-stu-id="14935-163">False means the availability is determined by the staff member's **workingHours** property setting.</span></span>|
|<span data-ttu-id="14935-164">workingHours</span><span class="sxs-lookup"><span data-stu-id="14935-164">workingHours</span></span>|<span data-ttu-id="14935-165">Коллекция [букингворкхаурс](bookingworkhours.md)</span><span class="sxs-lookup"><span data-stu-id="14935-165">[bookingWorkHours](bookingworkhours.md) collection</span></span>|<span data-ttu-id="14935-166">Диапазон часов на каждый день недели, когда сотрудник становится доступен для резервирования.</span><span class="sxs-lookup"><span data-stu-id="14935-166">The range of hours each day of the week that the staff member is available for booking.</span></span> <span data-ttu-id="14935-167">По умолчанию они инициализируются так же, как свойство **businessHours** для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="14935-167">By default, they are initialized to be the same as the **businessHours** property of the business.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14935-168">Отношения</span><span class="sxs-lookup"><span data-stu-id="14935-168">Relationships</span></span>
<span data-ttu-id="14935-169">Нет</span><span class="sxs-lookup"><span data-stu-id="14935-169">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="14935-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="14935-170">JSON representation</span></span>

<span data-ttu-id="14935-171">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14935-171">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
