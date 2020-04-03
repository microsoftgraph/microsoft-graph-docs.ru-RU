---
title: Тип ресурса groupLifecyclePolicy
description: Представляет политику жизненного цикла для группы Office 365.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 1d2627057b12b18952e39d83b92bbeea73bf4804
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124828"
---
# <a name="grouplifecyclepolicy-resource-type"></a><span data-ttu-id="19926-103">Тип ресурса groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="19926-103">groupLifecyclePolicy resource type</span></span>

<span data-ttu-id="19926-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19926-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="19926-105">Представляет политику жизненного цикла для группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="19926-105">Represents a lifecycle policy for an Office 365 group.</span></span> <span data-ttu-id="19926-106">Политика жизненного цикла позволяет администраторам устанавливать срок действия групп.</span><span class="sxs-lookup"><span data-stu-id="19926-106">A group lifecycle policy allows administrators to set an expiration period for groups.</span></span> <span data-ttu-id="19926-107">Например, срок действия группы истекает через 180 дней.</span><span class="sxs-lookup"><span data-stu-id="19926-107">For example, after 180 days, a group expires.</span></span> <span data-ttu-id="19926-108">Когда срок действия группы истекает, ее владельцы должны продлить его в течение определенного администратором времени.</span><span class="sxs-lookup"><span data-stu-id="19926-108">When a group reaches its expiration, owners of the group are required to renew their group within a time interval defined by the administrator.</span></span> <span data-ttu-id="19926-109">После продления группа будет оставаться активной в течение определенного политикой количества дней.</span><span class="sxs-lookup"><span data-stu-id="19926-109">Once renewed, the group expiration is extended by the number of days defined in the policy.</span></span> <span data-ttu-id="19926-110">Например, срок действия группы истекает через 180 дней после продления.</span><span class="sxs-lookup"><span data-stu-id="19926-110">For example, the group's new expiration is 180 days after renewal.</span></span> <span data-ttu-id="19926-111">Если срок действия группы не продлить, она будет удалена.</span><span class="sxs-lookup"><span data-stu-id="19926-111">If the group is not renewed, it expires and is deleted.</span></span> <span data-ttu-id="19926-112">Группу можно восстановить в течение 30 дней после удаления.</span><span class="sxs-lookup"><span data-stu-id="19926-112">The group can be restored within a period of 30 days from deletion.</span></span>

## <a name="methods"></a><span data-ttu-id="19926-113">Методы</span><span class="sxs-lookup"><span data-stu-id="19926-113">Methods</span></span>

| <span data-ttu-id="19926-114">Метод</span><span class="sxs-lookup"><span data-stu-id="19926-114">Method</span></span> | <span data-ttu-id="19926-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="19926-115">Return Type</span></span> | <span data-ttu-id="19926-116">Описание</span><span class="sxs-lookup"><span data-stu-id="19926-116">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="19926-117">Get groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="19926-117">Get groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-get.md) | [<span data-ttu-id="19926-118">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="19926-118">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) |<span data-ttu-id="19926-119">Чтение свойств и связей объекта groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="19926-119">Read properties and relationships of a groupLifecyclePolicy object.</span></span>|
|[<span data-ttu-id="19926-120">Перечисление groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="19926-120">List groupLifecyclePolicies</span></span>](../api/grouplifecyclepolicy-list.md) | <span data-ttu-id="19926-121">Коллекция [groupLifecyclePolicy](grouplifecyclepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="19926-121">[groupLifecyclePolicy](grouplifecyclepolicy.md) collection</span></span> | <span data-ttu-id="19926-122">Перечисление всех объектов groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="19926-122">List all the groupLifecyclePolicies.</span></span> |
|[<span data-ttu-id="19926-123">Update groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="19926-123">Update groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-update.md) | [<span data-ttu-id="19926-124">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="19926-124">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) | <span data-ttu-id="19926-125">Обновление объекта groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="19926-125">Update a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="19926-126">Delete groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="19926-126">Delete groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-delete.md) | <span data-ttu-id="19926-127">Нет</span><span class="sxs-lookup"><span data-stu-id="19926-127">None</span></span> | <span data-ttu-id="19926-128">Удаление объекта groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="19926-128">Delete a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="19926-129">Add a group to a groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="19926-129">Add a group to a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-addgroup.md)|<span data-ttu-id="19926-130">Нет</span><span class="sxs-lookup"><span data-stu-id="19926-130">None</span></span>| <span data-ttu-id="19926-131">Добавление группы в политику жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="19926-131">Add a group to a lifecycle policy</span></span> |
|[<span data-ttu-id="19926-132">Remove a group from a groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="19926-132">Remove a group from a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-removegroup.md)|<span data-ttu-id="19926-133">None</span><span class="sxs-lookup"><span data-stu-id="19926-133">None</span></span>| <span data-ttu-id="19926-134">Удаление группы из политики жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="19926-134">Remove a group to a lifecycle policy.</span></span> |
|[<span data-ttu-id="19926-135">Обновление группы</span><span class="sxs-lookup"><span data-stu-id="19926-135">Renew a group</span></span>](../api/grouplifecyclepolicy-renewgroup.md)|<span data-ttu-id="19926-136">Нет</span><span class="sxs-lookup"><span data-stu-id="19926-136">None</span></span>| <span data-ttu-id="19926-137">Обновление даты окончания срока действия группы.</span><span class="sxs-lookup"><span data-stu-id="19926-137">Renew a group's expiration date.</span></span> |

## <a name="properties"></a><span data-ttu-id="19926-138">Свойства</span><span class="sxs-lookup"><span data-stu-id="19926-138">Properties</span></span>

| <span data-ttu-id="19926-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="19926-139">Property</span></span> | <span data-ttu-id="19926-140">Тип</span><span class="sxs-lookup"><span data-stu-id="19926-140">Type</span></span> | <span data-ttu-id="19926-141">Описание</span><span class="sxs-lookup"><span data-stu-id="19926-141">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="19926-142">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="19926-142">alternateNotificationEmails</span></span>|<span data-ttu-id="19926-143">Строка</span><span class="sxs-lookup"><span data-stu-id="19926-143">String</span></span>| <span data-ttu-id="19926-144">Список адресов электронной почты для отправки уведомлений о группах без владельцев.</span><span class="sxs-lookup"><span data-stu-id="19926-144">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="19926-145">Можно указать несколько адресов электронной почты, разделив их точкой с запятой.</span><span class="sxs-lookup"><span data-stu-id="19926-145">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="19926-146">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="19926-146">groupLifetimeInDays</span></span>|<span data-ttu-id="19926-147">Int32</span><span class="sxs-lookup"><span data-stu-id="19926-147">Int32</span></span>| <span data-ttu-id="19926-148">Количество дней до истечения срока действия группы.</span><span class="sxs-lookup"><span data-stu-id="19926-148">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="19926-149">После продления группа будет оставаться активной в течение указанного количества дней.</span><span class="sxs-lookup"><span data-stu-id="19926-149">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="19926-150">id</span><span class="sxs-lookup"><span data-stu-id="19926-150">id</span></span>|<span data-ttu-id="19926-151">GUID</span><span class="sxs-lookup"><span data-stu-id="19926-151">Guid</span></span>| <span data-ttu-id="19926-152">Уникальный идентификатор политики.</span><span class="sxs-lookup"><span data-stu-id="19926-152">A unique identifier for a policy.</span></span> <span data-ttu-id="19926-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="19926-153">Read-only.</span></span>|
|<span data-ttu-id="19926-154">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="19926-154">managedGroupTypes</span></span>|<span data-ttu-id="19926-155">String</span><span class="sxs-lookup"><span data-stu-id="19926-155">String</span></span>| <span data-ttu-id="19926-156">Тип группы, к которому применяется политика истечения срока действия.</span><span class="sxs-lookup"><span data-stu-id="19926-156">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="19926-157">Возможные значения — **All**, **Selected** и **None**.</span><span class="sxs-lookup"><span data-stu-id="19926-157">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="19926-158">Связи</span><span class="sxs-lookup"><span data-stu-id="19926-158">Relationships</span></span>

<span data-ttu-id="19926-159">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="19926-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="19926-160">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="19926-160">JSON representation</span></span>

<span data-ttu-id="19926-161">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19926-161">Here is a JSON representation of the resource.</span></span>

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
