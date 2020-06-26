---
title: Тип ресурса Букингстаффмембер
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: c8676ce2e43e88ce53e4c79e13b9151a0eca2b58
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895715"
---
# <a name="bookingstaffmember-resource-type"></a><span data-ttu-id="02f06-104">Тип ресурса Букингстаффмембер</span><span class="sxs-lookup"><span data-stu-id="02f06-104">bookingStaffMember resource type</span></span>

<span data-ttu-id="02f06-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02f06-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="02f06-106">Представляет сотрудника, который предоставляет службы в [букингбусинесс](bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="02f06-106">Represents a staff member who provides services in a [bookingBusiness](bookingbusiness.md).</span></span>

<span data-ttu-id="02f06-107">Сотрудники могут входить в состав клиента Microsoft 365, на котором настроена Настройка бизнеса, или они могут использовать службы электронной почты от других поставщиков услуг электронной почты.</span><span class="sxs-lookup"><span data-stu-id="02f06-107">Staff members can be part of the Microsoft 365 tenant where the booking business is configured, or they can use email services from other email providers.</span></span>

<span data-ttu-id="02f06-108">При резервировании встреч API учета рассматривает следующие параметры для определения доступности сотрудников:</span><span class="sxs-lookup"><span data-stu-id="02f06-108">When booking appointments, the Bookings API considers the following settings to determine a staff member's availability:</span></span> 

1. <span data-ttu-id="02f06-109">По умолчанию часы работы бизнеса (свойство **businessHours** объекта [букингбусинесс](bookingbusiness.md) ) представляют общую доступность сотрудника.</span><span class="sxs-lookup"><span data-stu-id="02f06-109">By default, the hours of operation of the business (the **businessHours** property of the [bookingBusiness](bookingbusiness.md) entity) represents the general availability of the staff member.</span></span>
2. <span data-ttu-id="02f06-110">Если **усебусинесшаурс** имеет значение false, то характер рабочего времени сотрудника (свойства**воркингхаурс** объекта **букингстаффмембер** ) представляет общую доступность этого члена.</span><span class="sxs-lookup"><span data-stu-id="02f06-110">If **useBusinessHours** is false, then the staff member's specific work hours (**workingHours** property of the **bookingStaffmember** entity) represents that member's general availability.</span></span>
3. <span data-ttu-id="02f06-111">Если **аваилабилитисаффектедбиперсоналкалендар** имеет значение true, то API для резервирования будет сначала просматривать доступные часы сотрудника (как определено #1, так #2), а также проверять доступность в течение этих часов в личном календаре сотрудника перед выполнением резервирования.</span><span class="sxs-lookup"><span data-stu-id="02f06-111">If **availabilityIsAffectedByPersonalCalendar** is true, then the Bookings API would first look at the staff member's generally available hours (as determined by either #1 or #2), and verify availability during those hours in the staff member's personal calendar, before making a booking.</span></span>

## <a name="methods"></a><span data-ttu-id="02f06-112">Методы</span><span class="sxs-lookup"><span data-stu-id="02f06-112">Methods</span></span>

| <span data-ttu-id="02f06-113">Метод</span><span class="sxs-lookup"><span data-stu-id="02f06-113">Method</span></span>           | <span data-ttu-id="02f06-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="02f06-114">Return Type</span></span>    |<span data-ttu-id="02f06-115">Описание</span><span class="sxs-lookup"><span data-stu-id="02f06-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="02f06-116">Список сотрудников</span><span class="sxs-lookup"><span data-stu-id="02f06-116">List staff members</span></span>](../api/bookingbusiness-list-staffmembers.md) | <span data-ttu-id="02f06-117">Коллекция [букингстаффмембер](bookingstaffmember.md)</span><span class="sxs-lookup"><span data-stu-id="02f06-117">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="02f06-118">Получение списка объектов **букингстаффмембер** в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="02f06-118">Get a list of **bookingStaffMember** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="02f06-119">Создание Букингстафф</span><span class="sxs-lookup"><span data-stu-id="02f06-119">Create bookingStaff</span></span>](../api/bookingbusiness-post-staffmembers.md) | <span data-ttu-id="02f06-120">Коллекция [букингстаффмембер](bookingstaffmember.md)</span><span class="sxs-lookup"><span data-stu-id="02f06-120">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="02f06-121">Создание нового **букингстаффмембер** в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="02f06-121">Create a new **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="02f06-122">Получение Букингстаффмембер</span><span class="sxs-lookup"><span data-stu-id="02f06-122">Get bookingStaffMember</span></span>](../api/bookingstaffmember-get.md) | [<span data-ttu-id="02f06-123">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="02f06-123">bookingStaffMember</span></span>](bookingstaffmember.md) |<span data-ttu-id="02f06-124">Получение свойств и связей объекта **букингстаффмембер** в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="02f06-124">Get the properties and relationships of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="02f06-125">Update</span><span class="sxs-lookup"><span data-stu-id="02f06-125">Update</span></span>](../api/bookingstaffmember-update.md) | [<span data-ttu-id="02f06-126">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="02f06-126">bookingStaffMember</span></span>](bookingstaffmember.md)    |<span data-ttu-id="02f06-127">Обновление свойств объекта **букингстаффмембер** в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="02f06-127">Update the properties of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="02f06-128">Delete</span><span class="sxs-lookup"><span data-stu-id="02f06-128">Delete</span></span>](../api/bookingstaffmember-delete.md) | <span data-ttu-id="02f06-129">Нет</span><span class="sxs-lookup"><span data-stu-id="02f06-129">None</span></span> |<span data-ttu-id="02f06-130">Удаление сотрудника в заданном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="02f06-130">Delete a staff member in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="02f06-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="02f06-131">Properties</span></span>
| <span data-ttu-id="02f06-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="02f06-132">Property</span></span>     | <span data-ttu-id="02f06-133">Тип</span><span class="sxs-lookup"><span data-stu-id="02f06-133">Type</span></span>   |<span data-ttu-id="02f06-134">Описание</span><span class="sxs-lookup"><span data-stu-id="02f06-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02f06-135">аваилабилитисаффектедбиперсоналкалендар</span><span class="sxs-lookup"><span data-stu-id="02f06-135">availabilityIsAffectedByPersonalCalendar</span></span>|<span data-ttu-id="02f06-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="02f06-136">Boolean</span></span>|<span data-ttu-id="02f06-137">True означает, что если сотрудник является пользователем Microsoft 365, то API для резервирования будет проверять доступность сотрудников в личном календаре в Microsoft 365 перед выполнением резервирования.</span><span class="sxs-lookup"><span data-stu-id="02f06-137">True means that if the staff member is a Microsoft 365 user, the Bookings API would verify the staff member's availability in their personal calendar in Microsoft 365, before making a booking.</span></span> |
|<span data-ttu-id="02f06-138">colorIndex</span><span class="sxs-lookup"><span data-stu-id="02f06-138">colorIndex</span></span>|<span data-ttu-id="02f06-139">Int32</span><span class="sxs-lookup"><span data-stu-id="02f06-139">Int32</span></span>|<span data-ttu-id="02f06-140">Определяет цвет для представления сотрудника.</span><span class="sxs-lookup"><span data-stu-id="02f06-140">Identifies a color to represent the staff member.</span></span> <span data-ttu-id="02f06-141">Цвет соответствует цветовой палитре на странице " **сведения о персонале** " в приложении "книги".</span><span class="sxs-lookup"><span data-stu-id="02f06-141">The color corresponds to the color palette in the **Staff details** page in the Bookings app.</span></span>|
|<span data-ttu-id="02f06-142">displayName</span><span class="sxs-lookup"><span data-stu-id="02f06-142">displayName</span></span>|<span data-ttu-id="02f06-143">Строка</span><span class="sxs-lookup"><span data-stu-id="02f06-143">String</span></span>|<span data-ttu-id="02f06-144">Имя сотрудника, отображаемое для клиентов.</span><span class="sxs-lookup"><span data-stu-id="02f06-144">The name of the staff member, as displayed to customers.</span></span> <span data-ttu-id="02f06-145">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="02f06-145">Required.</span></span>|
|<span data-ttu-id="02f06-146">emailAddress</span><span class="sxs-lookup"><span data-stu-id="02f06-146">emailAddress</span></span>|<span data-ttu-id="02f06-147">String</span><span class="sxs-lookup"><span data-stu-id="02f06-147">String</span></span>|<span data-ttu-id="02f06-148">Адрес электронной почты сотрудника.</span><span class="sxs-lookup"><span data-stu-id="02f06-148">The email address of the staff member.</span></span> <span data-ttu-id="02f06-149">Это может быть тот же клиент Microsoft 365, что и в Организации, или в другом домене электронной почты.</span><span class="sxs-lookup"><span data-stu-id="02f06-149">This can be in the same Microsoft 365 tenant as the business, or in a different email domain.</span></span> <span data-ttu-id="02f06-150">Этот адрес электронной почты можно использовать, если для свойства **сендконфирматионстувнер** в политике планирования бизнеса задано значение true.</span><span class="sxs-lookup"><span data-stu-id="02f06-150">This email address can be used if the **sendConfirmationsToOwner** property is set to true in the scheduling policy of the business.</span></span> <span data-ttu-id="02f06-151">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="02f06-151">Required.</span></span>|
|<span data-ttu-id="02f06-152">id</span><span class="sxs-lookup"><span data-stu-id="02f06-152">id</span></span>|<span data-ttu-id="02f06-153">String</span><span class="sxs-lookup"><span data-stu-id="02f06-153">String</span></span>| <span data-ttu-id="02f06-154">Идентификатор сотрудника в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="02f06-154">The ID of the staff member, in a GUID format.</span></span> <span data-ttu-id="02f06-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="02f06-155">Read-only.</span></span>|
|<span data-ttu-id="02f06-156">role</span><span class="sxs-lookup"><span data-stu-id="02f06-156">role</span></span>|<span data-ttu-id="02f06-157">string</span><span class="sxs-lookup"><span data-stu-id="02f06-157">string</span></span>| <span data-ttu-id="02f06-158">Роль сотрудника в Организации.</span><span class="sxs-lookup"><span data-stu-id="02f06-158">The role of the staff member in the business.</span></span> <span data-ttu-id="02f06-159">Возможные значения: `guest`, `administrator`, `viewer`, `externalGuest`.</span><span class="sxs-lookup"><span data-stu-id="02f06-159">Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.</span></span> <span data-ttu-id="02f06-160">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="02f06-160">Required.</span></span>|
|<span data-ttu-id="02f06-161">усебусинесшаурс</span><span class="sxs-lookup"><span data-stu-id="02f06-161">useBusinessHours</span></span>|<span data-ttu-id="02f06-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="02f06-162">Boolean</span></span>|<span data-ttu-id="02f06-163">Значение true означает, что уровень доступности сотрудника указан в свойстве **businessHours** предприятия.</span><span class="sxs-lookup"><span data-stu-id="02f06-163">True means the staff member's availability is as specified in the **businessHours** property of the business.</span></span> <span data-ttu-id="02f06-164">Значение false означает, что доступность определяется значением свойства **воркингхаурс** сотрудника.</span><span class="sxs-lookup"><span data-stu-id="02f06-164">False means the availability is determined by the staff member's **workingHours** property setting.</span></span>|
|<span data-ttu-id="02f06-165">workingHours</span><span class="sxs-lookup"><span data-stu-id="02f06-165">workingHours</span></span>|<span data-ttu-id="02f06-166">Коллекция [букингворкхаурс](bookingworkhours.md)</span><span class="sxs-lookup"><span data-stu-id="02f06-166">[bookingWorkHours](bookingworkhours.md) collection</span></span>|<span data-ttu-id="02f06-167">Диапазон часов на каждый день недели, когда сотрудник становится доступен для резервирования.</span><span class="sxs-lookup"><span data-stu-id="02f06-167">The range of hours each day of the week that the staff member is available for booking.</span></span> <span data-ttu-id="02f06-168">По умолчанию они инициализируются так же, как свойство **businessHours** для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="02f06-168">By default, they are initialized to be the same as the **businessHours** property of the business.</span></span>|

## <a name="relationships"></a><span data-ttu-id="02f06-169">Связи</span><span class="sxs-lookup"><span data-stu-id="02f06-169">Relationships</span></span>
<span data-ttu-id="02f06-170">Нет</span><span class="sxs-lookup"><span data-stu-id="02f06-170">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="02f06-171">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="02f06-171">JSON representation</span></span>

<span data-ttu-id="02f06-172">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="02f06-172">The following is a JSON representation of the resource.</span></span>

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
