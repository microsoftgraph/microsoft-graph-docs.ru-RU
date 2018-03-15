# <a name="grouplifecyclepolicy-resource-type"></a><span data-ttu-id="d4853-101">Тип ресурса groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="d4853-101">groupLifecyclePolicy resource type</span></span>

<span data-ttu-id="d4853-102">Представляет политику жизненного цикла группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="d4853-102">Represents a a lifecycle policy for an Office 365 group.</span></span> <span data-ttu-id="d4853-103">Политика жизненного цикла позволяет администраторам устанавливать срок действия групп.</span><span class="sxs-lookup"><span data-stu-id="d4853-103">A group lifecycle policy allows administrators to set an expiration period for groups.</span></span> <span data-ttu-id="d4853-104">Например, срок действия группы истекает через 180 дней.</span><span class="sxs-lookup"><span data-stu-id="d4853-104">For example, after 180 days, a group expires.</span></span> <span data-ttu-id="d4853-105">Когда срок действия группы истекает, ее владельцы должны продлить его в течение определенного администратором времени.</span><span class="sxs-lookup"><span data-stu-id="d4853-105">When a group reaches its expiration, owners of the group are required to renew their group within a time interval defined by the administrator.</span></span> <span data-ttu-id="d4853-106">После продления группа будет оставаться активной в течение определенного политикой количества дней.</span><span class="sxs-lookup"><span data-stu-id="d4853-106">Once renewed, the group expiration is extended by the number of days defined in the policy.</span></span> <span data-ttu-id="d4853-107">Например, срок действия группы истекает через 180 дней после продления.</span><span class="sxs-lookup"><span data-stu-id="d4853-107">For example, the group's new expiration is 180 days after renewal.</span></span> <span data-ttu-id="d4853-108">Если срок действия группы не продлить, она будет удалена.</span><span class="sxs-lookup"><span data-stu-id="d4853-108">If the group is not renewed, it expires and is deleted.</span></span> <span data-ttu-id="d4853-109">Группу можно восстановить в течение 30 дней после удаления.</span><span class="sxs-lookup"><span data-stu-id="d4853-109">The group can be restored within a period of 30 days from deletion.</span></span>

## <a name="methods"></a><span data-ttu-id="d4853-110">Методы</span><span class="sxs-lookup"><span data-stu-id="d4853-110">Methods</span></span>

| <span data-ttu-id="d4853-111">Метод</span><span class="sxs-lookup"><span data-stu-id="d4853-111">Method</span></span> | <span data-ttu-id="d4853-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d4853-112">Return Type</span></span> | <span data-ttu-id="d4853-113">Описание</span><span class="sxs-lookup"><span data-stu-id="d4853-113">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="d4853-114">Get groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="d4853-114">Get groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy_get.md) | [<span data-ttu-id="d4853-115">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="d4853-115">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) |<span data-ttu-id="d4853-116">Чтение свойств и связей объекта groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="d4853-116">Read properties and relationships of plannerPlan object.</span></span>|
|[<span data-ttu-id="d4853-117">List groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="d4853-117">List groupLifecyclePolicies</span></span>](../api/grouplifecyclepolicy_list.md) | <span data-ttu-id="d4853-118">Коллекция [groupLifecyclePolicy](grouplifecyclepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="d4853-118">[groupLifecyclePolicy](grouplifecyclepolicy.md) collection</span></span> | <span data-ttu-id="d4853-119">Перечисление всех объектов groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="d4853-119">List all the groupLifecyclePolicies.</span></span> |
|[<span data-ttu-id="d4853-120">Update groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="d4853-120">Update groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy_update.md) | [<span data-ttu-id="d4853-121">groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="d4853-121">groupLifecyclePolicy</span></span>](grouplifecyclepolicy.md) | <span data-ttu-id="d4853-122">Обновление объекта groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="d4853-122">Update a setting object.</span></span> |
|[<span data-ttu-id="d4853-123">Delete groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="d4853-123">Delete groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy_delete.md) | <span data-ttu-id="d4853-124">None</span><span class="sxs-lookup"><span data-stu-id="d4853-124">None</span></span> | <span data-ttu-id="d4853-125">Удаление объекта groupLifecyclePolicy.</span><span class="sxs-lookup"><span data-stu-id="d4853-125">Delete a device object.</span></span> |
|[<span data-ttu-id="d4853-126">Add a group to a groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="d4853-126">Add a group to a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy_addgroup.md)|<span data-ttu-id="d4853-127">None</span><span class="sxs-lookup"><span data-stu-id="d4853-127">None</span></span>| <span data-ttu-id="d4853-128">Добавление группы в политику жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="d4853-128">Add a group to a lifecycle policy</span></span> |
|[<span data-ttu-id="d4853-129">Remove a group from a groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="d4853-129">Remove a group from a groupLifecyclePolicy</span></span>](../api/grouplifecyclepolicy_removegroup.md)|<span data-ttu-id="d4853-130">None</span><span class="sxs-lookup"><span data-stu-id="d4853-130">None</span></span>| <span data-ttu-id="d4853-131">Удаление группы из политики жизненного цикла.</span><span class="sxs-lookup"><span data-stu-id="d4853-131">Remove a group to a lifecycle policy.</span></span> |

## <a name="properties"></a><span data-ttu-id="d4853-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="d4853-132">Properties</span></span>

| <span data-ttu-id="d4853-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4853-133">Property</span></span> | <span data-ttu-id="d4853-134">Тип</span><span class="sxs-lookup"><span data-stu-id="d4853-134">Type</span></span> | <span data-ttu-id="d4853-135">Описание</span><span class="sxs-lookup"><span data-stu-id="d4853-135">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d4853-136">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="d4853-136">alternateNotificationEmails</span></span>|<span data-ttu-id="d4853-137">String</span><span class="sxs-lookup"><span data-stu-id="d4853-137">String</span></span>| <span data-ttu-id="d4853-138">Список адресов электронной почты для отправки уведомлений о группах без владельцев.</span><span class="sxs-lookup"><span data-stu-id="d4853-138">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="d4853-139">Можно указать несколько адресов электронной почты, разделив их точкой с запятой.</span><span class="sxs-lookup"><span data-stu-id="d4853-139">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="d4853-140">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="d4853-140">groupLifetimeInDays</span></span>|<span data-ttu-id="d4853-141">Int32</span><span class="sxs-lookup"><span data-stu-id="d4853-141">Int32</span></span>| <span data-ttu-id="d4853-142">Количество дней до истечения срока действия группы.</span><span class="sxs-lookup"><span data-stu-id="d4853-142">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="d4853-143">После продления группа будет оставаться активной в течение указанного количества дней.</span><span class="sxs-lookup"><span data-stu-id="d4853-143">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="d4853-144">id</span><span class="sxs-lookup"><span data-stu-id="d4853-144">id</span></span>|<span data-ttu-id="d4853-145">Guid</span><span class="sxs-lookup"><span data-stu-id="d4853-145">Guid</span></span>| <span data-ttu-id="d4853-146">Уникальный идентификатор политики.</span><span class="sxs-lookup"><span data-stu-id="d4853-146">A unique identifier for a specified replica.</span></span> <span data-ttu-id="d4853-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d4853-147">Read-only.</span></span>|
|<span data-ttu-id="d4853-148">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="d4853-148">managedGroupTypes</span></span>|<span data-ttu-id="d4853-149">String</span><span class="sxs-lookup"><span data-stu-id="d4853-149">String</span></span>| <span data-ttu-id="d4853-150">Тип группы, к которому применяется политика истечения срока действия.</span><span class="sxs-lookup"><span data-stu-id="d4853-150">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="d4853-151">Возможные значения — **All**, **Selected** и **None**.</span><span class="sxs-lookup"><span data-stu-id="d4853-151">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d4853-152">Связи</span><span class="sxs-lookup"><span data-stu-id="d4853-152">Relationships</span></span>

<span data-ttu-id="d4853-153">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d4853-153">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4853-154">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d4853-154">JSON representation</span></span>

<span data-ttu-id="d4853-155">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4853-155">Here is a JSON representation of the resource.</span></span>

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