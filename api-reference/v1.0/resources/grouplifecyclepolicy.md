---
title: Тип ресурса groupLifecyclePolicy
description: Представляет политику жизненного цикла для группы Office 365. Политика жизненного цикла позволяет администраторам устанавливать срок действия групп. Например, срок действия группы истекает через 180 дней. Когда срок действия группы истекает, ее владельцы должны продлить его в течение определенного администратором времени. После продления группа будет оставаться активной в течение определенного политикой количества дней. Например, срок действия группы истекает через 180 дней после продления. Если срок действия группы не продлить, она будет удалена. Группу можно восстановить в течение 30 дней после удаления.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 11f42c07857f94e081d79c6555e4608283dd9381
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030270"
---
# <a name="grouplifecyclepolicy-resource-type"></a><span data-ttu-id="a50e5-110">Тип ресурса groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="a50e5-110">groupLifecyclePolicy resource type</span></span>

<span data-ttu-id="a50e5-111">Представляет политику жизненного цикла для группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="a50e5-111">Represents a lifecycle policy for an Office 365 group.</span></span> <span data-ttu-id="a50e5-112">Политика жизненного цикла позволяет администраторам устанавливать срок действия групп.</span><span class="sxs-lookup"><span data-stu-id="a50e5-112">A group lifecycle policy allows administrators to set an expiration period for groups.</span></span> <span data-ttu-id="a50e5-113">Например, срок действия группы истекает через 180 дней.</span><span class="sxs-lookup"><span data-stu-id="a50e5-113">For example, after 180 days, a group expires.</span></span> <span data-ttu-id="a50e5-114">Когда срок действия группы истекает, ее владельцы должны продлить его в течение определенного администратором времени.</span><span class="sxs-lookup"><span data-stu-id="a50e5-114">When a group reaches its expiration, owners of the group are required to renew their group within a time interval defined by the administrator.</span></span> <span data-ttu-id="a50e5-115">После продления группа будет оставаться активной в течение определенного политикой количества дней.</span><span class="sxs-lookup"><span data-stu-id="a50e5-115">Once renewed, the group expiration is extended by the number of days defined in the policy.</span></span> <span data-ttu-id="a50e5-116">Например, срок действия группы истекает через 180 дней после продления.</span><span class="sxs-lookup"><span data-stu-id="a50e5-116">For example, the group's new expiration is 180 days after renewal.</span></span> <span data-ttu-id="a50e5-117">Если срок действия группы не продлить, она будет удалена.</span><span class="sxs-lookup"><span data-stu-id="a50e5-117">If the group is not renewed, it expires and is deleted.</span></span> <span data-ttu-id="a50e5-118">Группу можно восстановить в течение 30 дней после удаления.</span><span class="sxs-lookup"><span data-stu-id="a50e5-118">The group can be restored within a period of 30 days from deletion.</span></span>

## <a name="methods"></a><span data-ttu-id="a50e5-119">Методы</span><span class="sxs-lookup"><span data-stu-id="a50e5-119">Methods</span></span>

| <span data-ttu-id="a50e5-120">Метод</span><span class="sxs-lookup"><span data-stu-id="a50e5-120">Method</span></span> | <span data-ttu-id="a50e5-121">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a50e5-121">Return Type</span></span> | <span data-ttu-id="a50e5-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a50e5-122">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="a50e5-123">Get groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="a50e5-123">Get groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-get.md) | [<span data-ttu-id="a50e5-124">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="a50e5-124">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) |<span data-ttu-id="a50e5-125">Чтение свойств и связей объекта groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="a50e5-125">Read properties and relationships of a groupLifecyclePolicy object.</span></span>|
|[<span data-ttu-id="a50e5-126">Перечисление groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="a50e5-126">List groupLifecyclePolicies</span></span>](../api/grouplifecyclepolicy-list.md) | <span data-ttu-id="a50e5-127">Коллекция [groupLifecyclePolicy](grouplifecyclepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a50e5-127">[groupLifecyclePolicy](grouplifecyclepolicy.md) collection</span></span> | <span data-ttu-id="a50e5-128">Перечисление всех объектов groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="a50e5-128">List all the groupLifecyclePolicies.</span></span> |
|[<span data-ttu-id="a50e5-129">Update groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="a50e5-129">Update groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-update.md) | [<span data-ttu-id="a50e5-130">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="a50e5-130">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) | <span data-ttu-id="a50e5-131">Обновление объекта groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="a50e5-131">Update a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="a50e5-132">Delete groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="a50e5-132">Delete groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-delete.md) | <span data-ttu-id="a50e5-133">Нет</span><span class="sxs-lookup"><span data-stu-id="a50e5-133">None</span></span> | <span data-ttu-id="a50e5-134">Удаление объекта groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="a50e5-134">Delete a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="a50e5-135">Add a group to a groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="a50e5-135">Add a group to a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-addgroup.md)|<span data-ttu-id="a50e5-136">Нет</span><span class="sxs-lookup"><span data-stu-id="a50e5-136">None</span></span>| <span data-ttu-id="a50e5-137">Добавление группы в политику жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="a50e5-137">Add a group to a lifecycle policy</span></span> |
|[<span data-ttu-id="a50e5-138">Remove a group from a groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="a50e5-138">Remove a group from a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-removegroup.md)|<span data-ttu-id="a50e5-139">None</span><span class="sxs-lookup"><span data-stu-id="a50e5-139">None</span></span>| <span data-ttu-id="a50e5-140">Удаление группы из политики жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="a50e5-140">Remove a group to a lifecycle policy.</span></span> |

## <a name="properties"></a><span data-ttu-id="a50e5-141">Свойства</span><span class="sxs-lookup"><span data-stu-id="a50e5-141">Properties</span></span>

| <span data-ttu-id="a50e5-142">Свойство</span><span class="sxs-lookup"><span data-stu-id="a50e5-142">Property</span></span> | <span data-ttu-id="a50e5-143">Тип</span><span class="sxs-lookup"><span data-stu-id="a50e5-143">Type</span></span> | <span data-ttu-id="a50e5-144">Описание</span><span class="sxs-lookup"><span data-stu-id="a50e5-144">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a50e5-145">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="a50e5-145">alternateNotificationEmails</span></span>|<span data-ttu-id="a50e5-146">String</span><span class="sxs-lookup"><span data-stu-id="a50e5-146">String</span></span>| <span data-ttu-id="a50e5-147">Список адресов электронной почты для отправки уведомлений о группах без владельцев.</span><span class="sxs-lookup"><span data-stu-id="a50e5-147">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="a50e5-148">Можно указать несколько адресов электронной почты, разделив их точкой с запятой.</span><span class="sxs-lookup"><span data-stu-id="a50e5-148">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="a50e5-149">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="a50e5-149">groupLifetimeInDays</span></span>|<span data-ttu-id="a50e5-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a50e5-150">Int32</span></span>| <span data-ttu-id="a50e5-151">Количество дней до истечения срока действия группы.</span><span class="sxs-lookup"><span data-stu-id="a50e5-151">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="a50e5-152">После продления группа будет оставаться активной в течение указанного количества дней.</span><span class="sxs-lookup"><span data-stu-id="a50e5-152">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="a50e5-153">id</span><span class="sxs-lookup"><span data-stu-id="a50e5-153">id</span></span>|<span data-ttu-id="a50e5-154">GUID</span><span class="sxs-lookup"><span data-stu-id="a50e5-154">Guid</span></span>| <span data-ttu-id="a50e5-155">Уникальный идентификатор политики.</span><span class="sxs-lookup"><span data-stu-id="a50e5-155">A unique identifier for a policy.</span></span> <span data-ttu-id="a50e5-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a50e5-156">Read-only.</span></span>|
|<span data-ttu-id="a50e5-157">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="a50e5-157">managedGroupTypes</span></span>|<span data-ttu-id="a50e5-158">String</span><span class="sxs-lookup"><span data-stu-id="a50e5-158">String</span></span>| <span data-ttu-id="a50e5-159">Тип группы, к которому применяется политика истечения срока действия.</span><span class="sxs-lookup"><span data-stu-id="a50e5-159">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="a50e5-160">Возможные значения — **All**, **Selected** и **None**.</span><span class="sxs-lookup"><span data-stu-id="a50e5-160">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a50e5-161">Отношения</span><span class="sxs-lookup"><span data-stu-id="a50e5-161">Relationships</span></span>

<span data-ttu-id="a50e5-162">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a50e5-162">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a50e5-163">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a50e5-163">JSON representation</span></span>

<span data-ttu-id="a50e5-164">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a50e5-164">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
}-->

```json
{
  "alternateNotificationEmails": "String",
  "groupLifetimeInDays": 180,
  "id": "Guid (identifier)",
  "managedGroupTypes": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
