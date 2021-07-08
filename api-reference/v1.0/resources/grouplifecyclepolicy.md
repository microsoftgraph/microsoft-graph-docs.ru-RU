---
title: Тип ресурса groupLifecyclePolicy
description: Представляет политику жизненного цикла для Microsoft 365 группы.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 3122c297564981e75516ea602e699d3ebe49fa50
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317226"
---
# <a name="grouplifecyclepolicy-resource-type"></a><span data-ttu-id="2beaf-103">Тип ресурса groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="2beaf-103">groupLifecyclePolicy resource type</span></span>

<span data-ttu-id="2beaf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2beaf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2beaf-105">Представляет политику жизненного цикла для Microsoft 365 группы.</span><span class="sxs-lookup"><span data-stu-id="2beaf-105">Represents a lifecycle policy for a Microsoft 365 group.</span></span> <span data-ttu-id="2beaf-106">Политика жизненного цикла позволяет администраторам устанавливать срок действия групп.</span><span class="sxs-lookup"><span data-stu-id="2beaf-106">A group lifecycle policy allows administrators to set an expiration period for groups.</span></span> <span data-ttu-id="2beaf-107">Например, срок действия группы истекает через 180 дней.</span><span class="sxs-lookup"><span data-stu-id="2beaf-107">For example, after 180 days, a group expires.</span></span> <span data-ttu-id="2beaf-108">Когда срок действия группы истекает, ее владельцы должны продлить его в течение определенного администратором времени.</span><span class="sxs-lookup"><span data-stu-id="2beaf-108">When a group reaches its expiration, owners of the group are required to renew their group within a time interval defined by the administrator.</span></span> <span data-ttu-id="2beaf-109">После продления группа будет оставаться активной в течение определенного политикой количества дней.</span><span class="sxs-lookup"><span data-stu-id="2beaf-109">Once renewed, the group expiration is extended by the number of days defined in the policy.</span></span> <span data-ttu-id="2beaf-110">Например, срок действия группы истекает через 180 дней после продления.</span><span class="sxs-lookup"><span data-stu-id="2beaf-110">For example, the group's new expiration is 180 days after renewal.</span></span> <span data-ttu-id="2beaf-111">Если срок действия группы не продлить, она будет удалена.</span><span class="sxs-lookup"><span data-stu-id="2beaf-111">If the group is not renewed, it expires and is deleted.</span></span> <span data-ttu-id="2beaf-112">Группу можно восстановить в течение 30 дней после удаления.</span><span class="sxs-lookup"><span data-stu-id="2beaf-112">The group can be restored within a period of 30 days from deletion.</span></span>

## <a name="methods"></a><span data-ttu-id="2beaf-113">Методы</span><span class="sxs-lookup"><span data-stu-id="2beaf-113">Methods</span></span>

| <span data-ttu-id="2beaf-114">Метод</span><span class="sxs-lookup"><span data-stu-id="2beaf-114">Method</span></span> | <span data-ttu-id="2beaf-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2beaf-115">Return Type</span></span> | <span data-ttu-id="2beaf-116">Описание</span><span class="sxs-lookup"><span data-stu-id="2beaf-116">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="2beaf-117">Get groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="2beaf-117">Get groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-get.md) | [<span data-ttu-id="2beaf-118">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="2beaf-118">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) |<span data-ttu-id="2beaf-119">Чтение свойств и связей объекта groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="2beaf-119">Read properties and relationships of a groupLifecyclePolicy object.</span></span>|
|[<span data-ttu-id="2beaf-120">Перечисление groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="2beaf-120">List groupLifecyclePolicies</span></span>](../api/grouplifecyclepolicy-list.md) | <span data-ttu-id="2beaf-121">Коллекция [groupLifecyclePolicy](grouplifecyclepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2beaf-121">[groupLifecyclePolicy](grouplifecyclepolicy.md) collection</span></span> | <span data-ttu-id="2beaf-122">Перечисление всех объектов groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="2beaf-122">List all the groupLifecyclePolicies.</span></span> |
|[<span data-ttu-id="2beaf-123">Update groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="2beaf-123">Update groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-update.md) | [<span data-ttu-id="2beaf-124">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="2beaf-124">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) | <span data-ttu-id="2beaf-125">Обновление объекта groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="2beaf-125">Update a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="2beaf-126">Delete groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="2beaf-126">Delete groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-delete.md) | <span data-ttu-id="2beaf-127">None</span><span class="sxs-lookup"><span data-stu-id="2beaf-127">None</span></span> | <span data-ttu-id="2beaf-128">Удаление объекта groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="2beaf-128">Delete a groupLifecyclePolicy object.</span></span> |
|[<span data-ttu-id="2beaf-129">Add a group to a groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="2beaf-129">Add a group to a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-addgroup.md)|<span data-ttu-id="2beaf-130">None</span><span class="sxs-lookup"><span data-stu-id="2beaf-130">None</span></span>| <span data-ttu-id="2beaf-131">Добавление группы в политику жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="2beaf-131">Add a group to a lifecycle policy</span></span> |
|[<span data-ttu-id="2beaf-132">Remove a group from a groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="2beaf-132">Remove a group from a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy-removegroup.md)|<span data-ttu-id="2beaf-133">None</span><span class="sxs-lookup"><span data-stu-id="2beaf-133">None</span></span>| <span data-ttu-id="2beaf-134">Удаление группы из политики жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="2beaf-134">Remove a group to a lifecycle policy.</span></span> |

## <a name="properties"></a><span data-ttu-id="2beaf-135">Свойства</span><span class="sxs-lookup"><span data-stu-id="2beaf-135">Properties</span></span>

| <span data-ttu-id="2beaf-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="2beaf-136">Property</span></span> | <span data-ttu-id="2beaf-137">Тип</span><span class="sxs-lookup"><span data-stu-id="2beaf-137">Type</span></span> | <span data-ttu-id="2beaf-138">Описание</span><span class="sxs-lookup"><span data-stu-id="2beaf-138">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2beaf-139">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="2beaf-139">alternateNotificationEmails</span></span>|<span data-ttu-id="2beaf-140">String</span><span class="sxs-lookup"><span data-stu-id="2beaf-140">String</span></span>| <span data-ttu-id="2beaf-141">Список адресов электронной почты для отправки уведомлений о группах без владельцев.</span><span class="sxs-lookup"><span data-stu-id="2beaf-141">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="2beaf-142">Можно указать несколько адресов электронной почты, разделив их точкой с запятой.</span><span class="sxs-lookup"><span data-stu-id="2beaf-142">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="2beaf-143">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="2beaf-143">groupLifetimeInDays</span></span>|<span data-ttu-id="2beaf-144">Int32</span><span class="sxs-lookup"><span data-stu-id="2beaf-144">Int32</span></span>| <span data-ttu-id="2beaf-145">Количество дней до истечения срока действия группы.</span><span class="sxs-lookup"><span data-stu-id="2beaf-145">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="2beaf-146">После продления группа будет оставаться активной в течение указанного количества дней.</span><span class="sxs-lookup"><span data-stu-id="2beaf-146">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="2beaf-147">id</span><span class="sxs-lookup"><span data-stu-id="2beaf-147">id</span></span>|<span data-ttu-id="2beaf-148">String</span><span class="sxs-lookup"><span data-stu-id="2beaf-148">String</span></span>| <span data-ttu-id="2beaf-149">Уникальный идентификатор политики.</span><span class="sxs-lookup"><span data-stu-id="2beaf-149">A unique identifier for a policy.</span></span> <span data-ttu-id="2beaf-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2beaf-150">Read-only.</span></span>|
|<span data-ttu-id="2beaf-151">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="2beaf-151">managedGroupTypes</span></span>|<span data-ttu-id="2beaf-152">String</span><span class="sxs-lookup"><span data-stu-id="2beaf-152">String</span></span>| <span data-ttu-id="2beaf-153">Тип группы, к которому применяется политика истечения срока действия.</span><span class="sxs-lookup"><span data-stu-id="2beaf-153">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="2beaf-154">Возможные значения — **All**, **Selected** и **None**.</span><span class="sxs-lookup"><span data-stu-id="2beaf-154">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2beaf-155">Связи</span><span class="sxs-lookup"><span data-stu-id="2beaf-155">Relationships</span></span>

<span data-ttu-id="2beaf-156">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2beaf-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2beaf-157">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2beaf-157">JSON representation</span></span>

<span data-ttu-id="2beaf-158">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2beaf-158">Here is a JSON representation of the resource.</span></span>

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

