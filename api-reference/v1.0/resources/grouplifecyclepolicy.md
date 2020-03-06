---
title: Тип ресурса groupLifecyclePolicy
description: Представляет политику жизненного цикла для группы Office 365. Политика жизненного цикла позволяет администраторам устанавливать срок действия групп. Например, срок действия группы истекает через 180 дней. Когда срок действия группы истекает, ее владельцы должны продлить его в течение определенного администратором времени. После продления группа будет оставаться активной в течение определенного политикой количества дней. Например, срок действия группы истекает через 180 дней после продления. Если срок действия группы не продлить, она будет удалена. Группу можно восстановить в течение 30 дней после удаления.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: acd1e2b8b66d7cb643e483ee099a3c9909df5d9b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532926"
---
# <a name="grouplifecyclepolicy-resource-type"></a><span data-ttu-id="88a62-110">Тип ресурса groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="88a62-110">groupLifecyclePolicy resource type</span></span>

<span data-ttu-id="88a62-111">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88a62-111">Namespace: microsoft.graph</span></span>

<span data-ttu-id="88a62-112">Представляет политику жизненного цикла для группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="88a62-112">Represents a lifecycle policy for an Office 365 group.</span></span> <span data-ttu-id="88a62-113">Политика жизненного цикла позволяет администраторам устанавливать срок действия групп.</span><span class="sxs-lookup"><span data-stu-id="88a62-113">A group lifecycle policy allows administrators to set an expiration period for groups.</span></span> <span data-ttu-id="88a62-114">Например, срок действия группы истекает через 180 дней.</span><span class="sxs-lookup"><span data-stu-id="88a62-114">For example, after 180 days, a group expires.</span></span> <span data-ttu-id="88a62-115">Когда срок действия группы истекает, ее владельцы должны продлить его в течение определенного администратором времени.</span><span class="sxs-lookup"><span data-stu-id="88a62-115">When a group reaches its expiration, owners of the group are required to renew their group within a time interval defined by the administrator.</span></span> <span data-ttu-id="88a62-116">После продления группа будет оставаться активной в течение определенного политикой количества дней.</span><span class="sxs-lookup"><span data-stu-id="88a62-116">Once renewed, the group expiration is extended by the number of days defined in the policy.</span></span> <span data-ttu-id="88a62-117">Например, срок действия группы истекает через 180 дней после продления.</span><span class="sxs-lookup"><span data-stu-id="88a62-117">For example, the group's new expiration is 180 days after renewal.</span></span> <span data-ttu-id="88a62-118">Если срок действия группы не продлить, она будет удалена.</span><span class="sxs-lookup"><span data-stu-id="88a62-118">If the group is not renewed, it expires and is deleted.</span></span> <span data-ttu-id="88a62-119">Группу можно восстановить в течение 30 дней после удаления.</span><span class="sxs-lookup"><span data-stu-id="88a62-119">The group can be restored within a period of 30 days from deletion.</span></span>

## <a name="methods"></a><span data-ttu-id="88a62-120">Методы</span><span class="sxs-lookup"><span data-stu-id="88a62-120">Methods</span></span>

| <span data-ttu-id="88a62-121">Метод</span><span class="sxs-lookup"><span data-stu-id="88a62-121">Method</span></span> | <span data-ttu-id="88a62-122">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="88a62-122">Return Type</span></span> | <span data-ttu-id="88a62-123">Описание</span><span class="sxs-lookup"><span data-stu-id="88a62-123">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="88a62-124">Get groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="88a62-124">Get groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-get.md) | [<span data-ttu-id="88a62-125">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="88a62-125">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) |<span data-ttu-id="88a62-126">Чтение свойств и связей объекта groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="88a62-126">Read properties and relationships of a groupLifecyclePolicy object.</span></span>|
|[<span data-ttu-id="88a62-127">Перечисление groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="88a62-127">List groupLifecyclePolicies</span></span>](../api/grouplifecyclepolicy-list.md) | <span data-ttu-id="88a62-128">Коллекция [groupLifecyclePolicy](grouplifecyclepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="88a62-128">[groupLifecyclePolicy](grouplifecyclepolicy.md) collection</span></span> | <span data-ttu-id="88a62-129">Перечисление всех объектов groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="88a62-129">List all the groupLifecyclePolicies.</span></span> |
|[<span data-ttu-id="88a62-130">Update groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="88a62-130">Update groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-update.md) | [<span data-ttu-id="88a62-131">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="88a62-131">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) | <span data-ttu-id="88a62-132">Обновление объекта groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="88a62-132">Update a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="88a62-133">Delete groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="88a62-133">Delete groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-delete.md) | <span data-ttu-id="88a62-134">Нет</span><span class="sxs-lookup"><span data-stu-id="88a62-134">None</span></span> | <span data-ttu-id="88a62-135">Удаление объекта groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="88a62-135">Delete a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="88a62-136">Add a group to a groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="88a62-136">Add a group to a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-addgroup.md)|<span data-ttu-id="88a62-137">Нет</span><span class="sxs-lookup"><span data-stu-id="88a62-137">None</span></span>| <span data-ttu-id="88a62-138">Добавление группы в политику жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="88a62-138">Add a group to a lifecycle policy</span></span> |
|[<span data-ttu-id="88a62-139">Remove a group from a groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="88a62-139">Remove a group from a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-removegroup.md)|<span data-ttu-id="88a62-140">None</span><span class="sxs-lookup"><span data-stu-id="88a62-140">None</span></span>| <span data-ttu-id="88a62-141">Удаление группы из политики жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="88a62-141">Remove a group to a lifecycle policy.</span></span> |

## <a name="properties"></a><span data-ttu-id="88a62-142">Свойства</span><span class="sxs-lookup"><span data-stu-id="88a62-142">Properties</span></span>

| <span data-ttu-id="88a62-143">Свойство</span><span class="sxs-lookup"><span data-stu-id="88a62-143">Property</span></span> | <span data-ttu-id="88a62-144">Тип</span><span class="sxs-lookup"><span data-stu-id="88a62-144">Type</span></span> | <span data-ttu-id="88a62-145">Описание</span><span class="sxs-lookup"><span data-stu-id="88a62-145">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="88a62-146">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="88a62-146">alternateNotificationEmails</span></span>|<span data-ttu-id="88a62-147">Строка</span><span class="sxs-lookup"><span data-stu-id="88a62-147">String</span></span>| <span data-ttu-id="88a62-148">Список адресов электронной почты для отправки уведомлений о группах без владельцев.</span><span class="sxs-lookup"><span data-stu-id="88a62-148">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="88a62-149">Можно указать несколько адресов электронной почты, разделив их точкой с запятой.</span><span class="sxs-lookup"><span data-stu-id="88a62-149">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="88a62-150">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="88a62-150">groupLifetimeInDays</span></span>|<span data-ttu-id="88a62-151">Int32</span><span class="sxs-lookup"><span data-stu-id="88a62-151">Int32</span></span>| <span data-ttu-id="88a62-152">Количество дней до истечения срока действия группы.</span><span class="sxs-lookup"><span data-stu-id="88a62-152">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="88a62-153">После продления группа будет оставаться активной в течение указанного количества дней.</span><span class="sxs-lookup"><span data-stu-id="88a62-153">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="88a62-154">id</span><span class="sxs-lookup"><span data-stu-id="88a62-154">id</span></span>|<span data-ttu-id="88a62-155">GUID</span><span class="sxs-lookup"><span data-stu-id="88a62-155">Guid</span></span>| <span data-ttu-id="88a62-156">Уникальный идентификатор политики.</span><span class="sxs-lookup"><span data-stu-id="88a62-156">A unique identifier for a policy.</span></span> <span data-ttu-id="88a62-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="88a62-157">Read-only.</span></span>|
|<span data-ttu-id="88a62-158">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="88a62-158">managedGroupTypes</span></span>|<span data-ttu-id="88a62-159">String</span><span class="sxs-lookup"><span data-stu-id="88a62-159">String</span></span>| <span data-ttu-id="88a62-160">Тип группы, к которому применяется политика истечения срока действия.</span><span class="sxs-lookup"><span data-stu-id="88a62-160">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="88a62-161">Возможные значения — **All**, **Selected** и **None**.</span><span class="sxs-lookup"><span data-stu-id="88a62-161">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="88a62-162">Связи</span><span class="sxs-lookup"><span data-stu-id="88a62-162">Relationships</span></span>

<span data-ttu-id="88a62-163">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="88a62-163">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="88a62-164">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="88a62-164">JSON representation</span></span>

<span data-ttu-id="88a62-165">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="88a62-165">Here is a JSON representation of the resource.</span></span>

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
