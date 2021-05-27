---
title: Тип ресурса groupLifecyclePolicy
description: Представляет политику жизненного цикла для Microsoft 365 группы.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 6b53fbb6b4a4b7de83bf342b2036b40d1b08fcdf
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682413"
---
# <a name="grouplifecyclepolicy-resource-type"></a><span data-ttu-id="7bdd9-103">Тип ресурса groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="7bdd9-103">groupLifecyclePolicy resource type</span></span>

<span data-ttu-id="7bdd9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bdd9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bdd9-105">Представляет политику жизненного цикла для Microsoft 365 группы.</span><span class="sxs-lookup"><span data-stu-id="7bdd9-105">Represents a lifecycle policy for a Microsoft 365 group.</span></span> <span data-ttu-id="7bdd9-106">Политика жизненного цикла позволяет администраторам устанавливать срок действия групп.</span><span class="sxs-lookup"><span data-stu-id="7bdd9-106">A group lifecycle policy allows administrators to set an expiration period for groups.</span></span> <span data-ttu-id="7bdd9-107">Например, срок действия группы истекает через 180 дней.</span><span class="sxs-lookup"><span data-stu-id="7bdd9-107">For example, after 180 days, a group expires.</span></span> <span data-ttu-id="7bdd9-108">Когда срок действия группы истекает, ее владельцы должны продлить его в течение определенного администратором времени.</span><span class="sxs-lookup"><span data-stu-id="7bdd9-108">When a group reaches its expiration, owners of the group are required to renew their group within a time interval defined by the administrator.</span></span> <span data-ttu-id="7bdd9-109">После продления группа будет оставаться активной в течение определенного политикой количества дней.</span><span class="sxs-lookup"><span data-stu-id="7bdd9-109">Once renewed, the group expiration is extended by the number of days defined in the policy.</span></span> <span data-ttu-id="7bdd9-110">Например, срок действия группы истекает через 180 дней после продления.</span><span class="sxs-lookup"><span data-stu-id="7bdd9-110">For example, the group's new expiration is 180 days after renewal.</span></span> <span data-ttu-id="7bdd9-111">Если срок действия группы не продлить, она будет удалена.</span><span class="sxs-lookup"><span data-stu-id="7bdd9-111">If the group is not renewed, it expires and is deleted.</span></span> <span data-ttu-id="7bdd9-112">Группу можно восстановить в течение 30 дней после удаления.</span><span class="sxs-lookup"><span data-stu-id="7bdd9-112">The group can be restored within a period of 30 days from deletion.</span></span>

## <a name="methods"></a><span data-ttu-id="7bdd9-113">Методы</span><span class="sxs-lookup"><span data-stu-id="7bdd9-113">Methods</span></span>

| <span data-ttu-id="7bdd9-114">Метод</span><span class="sxs-lookup"><span data-stu-id="7bdd9-114">Method</span></span> | <span data-ttu-id="7bdd9-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7bdd9-115">Return Type</span></span> | <span data-ttu-id="7bdd9-116">Описание</span><span class="sxs-lookup"><span data-stu-id="7bdd9-116">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="7bdd9-117">Get groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="7bdd9-117">Get groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-get.md) | [<span data-ttu-id="7bdd9-118">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="7bdd9-118">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) |<span data-ttu-id="7bdd9-119">Чтение свойств и связей объекта groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="7bdd9-119">Read properties and relationships of a groupLifecyclePolicy object.</span></span>|
|[<span data-ttu-id="7bdd9-120">Перечисление groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="7bdd9-120">List groupLifecyclePolicies</span></span>](../api/grouplifecyclepolicy-list.md) | <span data-ttu-id="7bdd9-121">Коллекция [groupLifecyclePolicy](grouplifecyclepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7bdd9-121">[groupLifecyclePolicy](grouplifecyclepolicy.md) collection</span></span> | <span data-ttu-id="7bdd9-122">Перечисление всех объектов groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="7bdd9-122">List all the groupLifecyclePolicies.</span></span> |
|[<span data-ttu-id="7bdd9-123">Update groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="7bdd9-123">Update groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-update.md) | [<span data-ttu-id="7bdd9-124">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="7bdd9-124">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) | <span data-ttu-id="7bdd9-125">Обновление объекта groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="7bdd9-125">Update a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="7bdd9-126">Delete groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="7bdd9-126">Delete groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-delete.md) | <span data-ttu-id="7bdd9-127">None</span><span class="sxs-lookup"><span data-stu-id="7bdd9-127">None</span></span> | <span data-ttu-id="7bdd9-128">Удаление объекта groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="7bdd9-128">Delete a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="7bdd9-129">Add a group to a groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="7bdd9-129">Add a group to a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-addgroup.md)|<span data-ttu-id="7bdd9-130">None</span><span class="sxs-lookup"><span data-stu-id="7bdd9-130">None</span></span>| <span data-ttu-id="7bdd9-131">Добавление группы в политику жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="7bdd9-131">Add a group to a lifecycle policy</span></span> |
|[<span data-ttu-id="7bdd9-132">Remove a group from a groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="7bdd9-132">Remove a group from a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-removegroup.md)|<span data-ttu-id="7bdd9-133">None</span><span class="sxs-lookup"><span data-stu-id="7bdd9-133">None</span></span>| <span data-ttu-id="7bdd9-134">Удаление группы из политики жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="7bdd9-134">Remove a group to a lifecycle policy.</span></span> |
|[<span data-ttu-id="7bdd9-135">Обновление группы</span><span class="sxs-lookup"><span data-stu-id="7bdd9-135">Renew a group</span></span>](../api/grouplifecyclepolicy-renewgroup.md)|<span data-ttu-id="7bdd9-136">Нет</span><span class="sxs-lookup"><span data-stu-id="7bdd9-136">None</span></span>| <span data-ttu-id="7bdd9-137">Продление срока действия группы.</span><span class="sxs-lookup"><span data-stu-id="7bdd9-137">Renew a group's expiration date.</span></span> |

## <a name="properties"></a><span data-ttu-id="7bdd9-138">Свойства</span><span class="sxs-lookup"><span data-stu-id="7bdd9-138">Properties</span></span>

| <span data-ttu-id="7bdd9-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="7bdd9-139">Property</span></span> | <span data-ttu-id="7bdd9-140">Тип</span><span class="sxs-lookup"><span data-stu-id="7bdd9-140">Type</span></span> | <span data-ttu-id="7bdd9-141">Описание</span><span class="sxs-lookup"><span data-stu-id="7bdd9-141">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="7bdd9-142">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="7bdd9-142">alternateNotificationEmails</span></span>|<span data-ttu-id="7bdd9-143">String</span><span class="sxs-lookup"><span data-stu-id="7bdd9-143">String</span></span>| <span data-ttu-id="7bdd9-144">Список адресов электронной почты для отправки уведомлений о группах без владельцев.</span><span class="sxs-lookup"><span data-stu-id="7bdd9-144">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="7bdd9-145">Можно указать несколько адресов электронной почты, разделив их точкой с запятой.</span><span class="sxs-lookup"><span data-stu-id="7bdd9-145">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="7bdd9-146">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="7bdd9-146">groupLifetimeInDays</span></span>|<span data-ttu-id="7bdd9-147">Int32</span><span class="sxs-lookup"><span data-stu-id="7bdd9-147">Int32</span></span>| <span data-ttu-id="7bdd9-148">Количество дней до истечения срока действия группы.</span><span class="sxs-lookup"><span data-stu-id="7bdd9-148">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="7bdd9-149">После продления группа будет оставаться активной в течение указанного количества дней.</span><span class="sxs-lookup"><span data-stu-id="7bdd9-149">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="7bdd9-150">id</span><span class="sxs-lookup"><span data-stu-id="7bdd9-150">id</span></span>|<span data-ttu-id="7bdd9-151">GUID</span><span class="sxs-lookup"><span data-stu-id="7bdd9-151">Guid</span></span>| <span data-ttu-id="7bdd9-152">Уникальный идентификатор политики.</span><span class="sxs-lookup"><span data-stu-id="7bdd9-152">A unique identifier for a policy.</span></span> <span data-ttu-id="7bdd9-153">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7bdd9-153">Read-only.</span></span>|
|<span data-ttu-id="7bdd9-154">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="7bdd9-154">managedGroupTypes</span></span>|<span data-ttu-id="7bdd9-155">String</span><span class="sxs-lookup"><span data-stu-id="7bdd9-155">String</span></span>| <span data-ttu-id="7bdd9-156">Тип группы, к которому применяется политика истечения срока действия.</span><span class="sxs-lookup"><span data-stu-id="7bdd9-156">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="7bdd9-157">Возможные значения — **All**, **Selected** и **None**.</span><span class="sxs-lookup"><span data-stu-id="7bdd9-157">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7bdd9-158">Связи</span><span class="sxs-lookup"><span data-stu-id="7bdd9-158">Relationships</span></span>

<span data-ttu-id="7bdd9-159">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7bdd9-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7bdd9-160">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7bdd9-160">JSON representation</span></span>

<span data-ttu-id="7bdd9-161">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7bdd9-161">Here is a JSON representation of the resource.</span></span>

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


