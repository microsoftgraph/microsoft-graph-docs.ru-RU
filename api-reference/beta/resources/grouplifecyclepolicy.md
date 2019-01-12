---
title: Тип ресурса groupLifecyclePolicy
description: Представляет политику жизненного цикла группы Office 365. Политика жизненного цикла позволяет администраторам устанавливать срок действия групп. Например, срок действия группы истекает через 180 дней. Когда срок действия группы истекает, ее владельцы должны продлить его в течение определенного администратором времени. После продления группа будет оставаться активной в течение определенного политикой количества дней. Например, срок действия группы истекает через 180 дней после продления. Если срок действия группы не продлить, она будет удалена. Группу можно восстановить в течение 30 дней после удаления.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: c69a54ef5323b1e3d171135d4b1b0231b6834c79
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970243"
---
# <a name="grouplifecyclepolicy-resource-type"></a><span data-ttu-id="bc355-110">Тип ресурса groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="bc355-110">groupLifecyclePolicy resource type</span></span>

<span data-ttu-id="bc355-111">Представляет политику жизненного цикла группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="bc355-111">Represents a a lifecycle policy for an Office 365 group.</span></span> <span data-ttu-id="bc355-112">Политика жизненного цикла позволяет администраторам устанавливать срок действия групп.</span><span class="sxs-lookup"><span data-stu-id="bc355-112">A group lifecycle policy allows administrators to set an expiration period for groups.</span></span> <span data-ttu-id="bc355-113">Например, срок действия группы истекает через 180 дней.</span><span class="sxs-lookup"><span data-stu-id="bc355-113">For example, after 180 days, a group expires.</span></span> <span data-ttu-id="bc355-114">Когда срок действия группы истекает, ее владельцы должны продлить его в течение определенного администратором времени.</span><span class="sxs-lookup"><span data-stu-id="bc355-114">When a group reaches its expiration, owners of the group are required to renew their group within a time interval defined by the administrator.</span></span> <span data-ttu-id="bc355-115">После продления группа будет оставаться активной в течение определенного политикой количества дней.</span><span class="sxs-lookup"><span data-stu-id="bc355-115">Once renewed, the group expiration is extended by the number of days defined in the policy.</span></span> <span data-ttu-id="bc355-116">Например, срок действия группы истекает через 180 дней после продления.</span><span class="sxs-lookup"><span data-stu-id="bc355-116">For example, the group's new expiration is 180 days after renewal.</span></span> <span data-ttu-id="bc355-117">Если срок действия группы не продлить, она будет удалена.</span><span class="sxs-lookup"><span data-stu-id="bc355-117">If the group is not renewed, it expires and is deleted.</span></span> <span data-ttu-id="bc355-118">Группу можно восстановить в течение 30 дней после удаления.</span><span class="sxs-lookup"><span data-stu-id="bc355-118">The group can be restored within a period of 30 days from deletion.</span></span>

## <a name="methods"></a><span data-ttu-id="bc355-119">Методы</span><span class="sxs-lookup"><span data-stu-id="bc355-119">Methods</span></span>

| <span data-ttu-id="bc355-120">Метод</span><span class="sxs-lookup"><span data-stu-id="bc355-120">Method</span></span> | <span data-ttu-id="bc355-121">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bc355-121">Return Type</span></span> | <span data-ttu-id="bc355-122">Описание</span><span class="sxs-lookup"><span data-stu-id="bc355-122">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="bc355-123">Get groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="bc355-123">Get groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-get.md) | [<span data-ttu-id="bc355-124">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="bc355-124">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) |<span data-ttu-id="bc355-125">Чтение свойств и связей объекта groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="bc355-125">Read properties and relationships of a groupLifecyclePolicy object.</span></span>|
|[<span data-ttu-id="bc355-126">List groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="bc355-126">List groupLifecyclePolicies</span></span>](../api/grouplifecyclepolicy-list.md) | <span data-ttu-id="bc355-127">Коллекция [groupLifecyclePolicy](grouplifecyclepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="bc355-127">[groupLifecyclePolicy](grouplifecyclepolicy.md) collection</span></span> | <span data-ttu-id="bc355-128">Перечисление всех объектов groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="bc355-128">List all the groupLifecyclePolicies.</span></span> |
|[<span data-ttu-id="bc355-129">Update groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="bc355-129">Update groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-update.md) | [<span data-ttu-id="bc355-130">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="bc355-130">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) | <span data-ttu-id="bc355-131">Обновление объекта groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="bc355-131">Update a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="bc355-132">Delete groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="bc355-132">Delete groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-delete.md) | <span data-ttu-id="bc355-133">None</span><span class="sxs-lookup"><span data-stu-id="bc355-133">None</span></span> | <span data-ttu-id="bc355-134">Удаление объекта groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="bc355-134">Delete a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="bc355-135">Add a group to a groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="bc355-135">Add a group to a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-addgroup.md)|<span data-ttu-id="bc355-136">None</span><span class="sxs-lookup"><span data-stu-id="bc355-136">None</span></span>| <span data-ttu-id="bc355-137">Добавление группы в политику жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="bc355-137">Add a group to a lifecycle policy</span></span> |
|[<span data-ttu-id="bc355-138">Remove a group from a groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="bc355-138">Remove a group from a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-removegroup.md)|<span data-ttu-id="bc355-139">None</span><span class="sxs-lookup"><span data-stu-id="bc355-139">None</span></span>| <span data-ttu-id="bc355-140">Удаление группы из политики жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="bc355-140">Remove a group to a lifecycle policy.</span></span> |
|[<span data-ttu-id="bc355-141">Обновление группы</span><span class="sxs-lookup"><span data-stu-id="bc355-141">Renew a group</span></span>](../api/grouplifecyclepolicy-renewgroup.md)|<span data-ttu-id="bc355-142">Нет</span><span class="sxs-lookup"><span data-stu-id="bc355-142">None</span></span>| <span data-ttu-id="bc355-143">Обновите срок действия группы.</span><span class="sxs-lookup"><span data-stu-id="bc355-143">Renew a group's expiration date.</span></span> |

## <a name="properties"></a><span data-ttu-id="bc355-144">Свойства</span><span class="sxs-lookup"><span data-stu-id="bc355-144">Properties</span></span>

| <span data-ttu-id="bc355-145">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc355-145">Property</span></span> | <span data-ttu-id="bc355-146">Тип</span><span class="sxs-lookup"><span data-stu-id="bc355-146">Type</span></span> | <span data-ttu-id="bc355-147">Описание</span><span class="sxs-lookup"><span data-stu-id="bc355-147">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="bc355-148">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="bc355-148">alternateNotificationEmails</span></span>|<span data-ttu-id="bc355-149">String</span><span class="sxs-lookup"><span data-stu-id="bc355-149">String</span></span>| <span data-ttu-id="bc355-150">Список адресов электронной почты для отправки уведомлений о группах без владельцев.</span><span class="sxs-lookup"><span data-stu-id="bc355-150">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="bc355-151">Можно указать несколько адресов электронной почты, разделив их точкой с запятой.</span><span class="sxs-lookup"><span data-stu-id="bc355-151">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="bc355-152">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="bc355-152">groupLifetimeInDays</span></span>|<span data-ttu-id="bc355-153">Int32</span><span class="sxs-lookup"><span data-stu-id="bc355-153">Int32</span></span>| <span data-ttu-id="bc355-154">Количество дней до истечения срока действия группы.</span><span class="sxs-lookup"><span data-stu-id="bc355-154">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="bc355-155">После продления группа будет оставаться активной в течение указанного количества дней.</span><span class="sxs-lookup"><span data-stu-id="bc355-155">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="bc355-156">id</span><span class="sxs-lookup"><span data-stu-id="bc355-156">id</span></span>|<span data-ttu-id="bc355-157">Guid</span><span class="sxs-lookup"><span data-stu-id="bc355-157">Guid</span></span>| <span data-ttu-id="bc355-158">Уникальный идентификатор политики.</span><span class="sxs-lookup"><span data-stu-id="bc355-158">A unique identifier for a policy.</span></span> <span data-ttu-id="bc355-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bc355-159">Read-only.</span></span>|
|<span data-ttu-id="bc355-160">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="bc355-160">managedGroupTypes</span></span>|<span data-ttu-id="bc355-161">String</span><span class="sxs-lookup"><span data-stu-id="bc355-161">String</span></span>| <span data-ttu-id="bc355-162">Тип группы, к которому применяется политика истечения срока действия.</span><span class="sxs-lookup"><span data-stu-id="bc355-162">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="bc355-163">Возможные значения — **All**, **Selected** и **None**.</span><span class="sxs-lookup"><span data-stu-id="bc355-163">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="bc355-164">Связи</span><span class="sxs-lookup"><span data-stu-id="bc355-164">Relationships</span></span>

<span data-ttu-id="bc355-165">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bc355-165">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc355-166">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="bc355-166">JSON representation</span></span>

<span data-ttu-id="bc355-167">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bc355-167">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
