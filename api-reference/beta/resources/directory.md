---
title: Тип ресурса directory (удаленные элементы)
description: . Удаленные элементы можно восстановить в течение 30 дней. Через 30 дней элементы удаляются без возможности восстановления.
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: c79e21600ed03a8239c0baaf1f436f074a4377bc
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547241"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="7bfbb-105">Тип ресурса directory (удаленные элементы)</span><span class="sxs-lookup"><span data-stu-id="7bfbb-105">directory resource type (deleted items)</span></span>

<span data-ttu-id="7bfbb-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bfbb-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bfbb-107">Представляет удаленный элемент в каталоге.</span><span class="sxs-lookup"><span data-stu-id="7bfbb-107">Represents a deleted item in the directory.</span></span> <span data-ttu-id="7bfbb-108">После удаления элемент добавляется в "контейнер" удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="7bfbb-108">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="7bfbb-109">Удаленные элементы можно восстановить в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="7bfbb-109">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="7bfbb-110">Через 30 дней элементы удаляются без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="7bfbb-110">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="7bfbb-111">В настоящее время функции удаленных элементов поддерживаются только для [приложений,](application.md) [групповых и](group.md) [пользовательских](user.md) ресурсов.</span><span class="sxs-lookup"><span data-stu-id="7bfbb-111">Currently, deleted items functionality is only supported for the [application](application.md), [group](group.md) and [user](user.md) resources.</span></span>

## <a name="methods"></a><span data-ttu-id="7bfbb-112">Методы</span><span class="sxs-lookup"><span data-stu-id="7bfbb-112">Methods</span></span>

| <span data-ttu-id="7bfbb-113">Метод</span><span class="sxs-lookup"><span data-stu-id="7bfbb-113">Method</span></span>         | <span data-ttu-id="7bfbb-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7bfbb-114">Return Type</span></span> | <span data-ttu-id="7bfbb-115">Описание</span><span class="sxs-lookup"><span data-stu-id="7bfbb-115">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="7bfbb-116">Получение удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="7bfbb-116">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="7bfbb-117">directoryObject</span><span class="sxs-lookup"><span data-stu-id="7bfbb-117">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="7bfbb-118">Получает свойства удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="7bfbb-118">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="7bfbb-119">Восстановление удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="7bfbb-119">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="7bfbb-120">directoryObject</span><span class="sxs-lookup"><span data-stu-id="7bfbb-120">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="7bfbb-121">Восстанавливает недавно удаленный элемент.</span><span class="sxs-lookup"><span data-stu-id="7bfbb-121">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="7bfbb-122">Перечисление удаленных элементов</span><span class="sxs-lookup"><span data-stu-id="7bfbb-122">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="7bfbb-123">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="7bfbb-123">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="7bfbb-124">Получает список недавно удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="7bfbb-124">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="7bfbb-125">Окончательное удаление элемента</span><span class="sxs-lookup"><span data-stu-id="7bfbb-125">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="7bfbb-126">None</span><span class="sxs-lookup"><span data-stu-id="7bfbb-126">None</span></span> | <span data-ttu-id="7bfbb-127">Окончательно удаляет элемент.</span><span class="sxs-lookup"><span data-stu-id="7bfbb-127">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="7bfbb-128">Список удаленных элементов, которые принадлежат пользователю</span><span class="sxs-lookup"><span data-stu-id="7bfbb-128">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="7bfbb-129">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="7bfbb-129">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="7bfbb-130">Списки элементов каталогов, которые принадлежат пользователю.</span><span class="sxs-lookup"><span data-stu-id="7bfbb-130">Lists directory items owned by a user.</span></span> |
|[<span data-ttu-id="7bfbb-131">Функция ListRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="7bfbb-131">List featureRolloutPolicies</span></span>](../api/list-featurerolloutpolicies.md) | <span data-ttu-id="7bfbb-132">[коллекция featureRolloutPolicy](featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7bfbb-132">[featureRolloutPolicy](featurerolloutpolicy.md) collection</span></span> | <span data-ttu-id="7bfbb-133">Извлечение списка объектов featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="7bfbb-133">Retrieve a list of featureRolloutPolicy objects.</span></span> |
|[<span data-ttu-id="7bfbb-134">Создание featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="7bfbb-134">Create featureRolloutPolicy</span></span>](../api/post-featurerolloutpolicies.md) | [<span data-ttu-id="7bfbb-135">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="7bfbb-135">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="7bfbb-136">Создайте новый объект featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="7bfbb-136">Create a new featureRolloutPolicy object.</span></span> |
| [<span data-ttu-id="7bfbb-137">Get featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="7bfbb-137">Get featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-get.md) | [<span data-ttu-id="7bfbb-138">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="7bfbb-138">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="7bfbb-139">Извлечение свойств и связей объекта featurerolloutpolicy.</span><span class="sxs-lookup"><span data-stu-id="7bfbb-139">Retrieve the properties and relationships of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="7bfbb-140">Обновление функцииRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="7bfbb-140">Update featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-update.md) | [<span data-ttu-id="7bfbb-141">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="7bfbb-141">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="7bfbb-142">Обновление свойств объекта featurerolloutpolicy.</span><span class="sxs-lookup"><span data-stu-id="7bfbb-142">Update the properties of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="7bfbb-143">Удаление featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="7bfbb-143">Delete featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-delete.md) | <span data-ttu-id="7bfbb-144">Нет</span><span class="sxs-lookup"><span data-stu-id="7bfbb-144">None</span></span> | <span data-ttu-id="7bfbb-145">Удаление объекта featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="7bfbb-145">Delete a featureRolloutPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7bfbb-146">Свойства</span><span class="sxs-lookup"><span data-stu-id="7bfbb-146">Properties</span></span>
| <span data-ttu-id="7bfbb-147">Свойство</span><span class="sxs-lookup"><span data-stu-id="7bfbb-147">Property</span></span>   | <span data-ttu-id="7bfbb-148">Тип</span><span class="sxs-lookup"><span data-stu-id="7bfbb-148">Type</span></span> |<span data-ttu-id="7bfbb-149">Описание</span><span class="sxs-lookup"><span data-stu-id="7bfbb-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7bfbb-150">id</span><span class="sxs-lookup"><span data-stu-id="7bfbb-150">id</span></span>|<span data-ttu-id="7bfbb-151">String</span><span class="sxs-lookup"><span data-stu-id="7bfbb-151">String</span></span>| <span data-ttu-id="7bfbb-152">Уникальный идентификатор объекта, например 12345678-9abc-def0-1234-56789abcde.</span><span class="sxs-lookup"><span data-stu-id="7bfbb-152">A unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="7bfbb-153">Ключ.</span><span class="sxs-lookup"><span data-stu-id="7bfbb-153">Key.</span></span> <span data-ttu-id="7bfbb-154">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="7bfbb-154">Not nullable.</span></span> <span data-ttu-id="7bfbb-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7bfbb-155">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7bfbb-156">Связи</span><span class="sxs-lookup"><span data-stu-id="7bfbb-156">Relationships</span></span>
| <span data-ttu-id="7bfbb-157">Связь</span><span class="sxs-lookup"><span data-stu-id="7bfbb-157">Relationship</span></span> | <span data-ttu-id="7bfbb-158">Тип</span><span class="sxs-lookup"><span data-stu-id="7bfbb-158">Type</span></span>   |<span data-ttu-id="7bfbb-159">Описание</span><span class="sxs-lookup"><span data-stu-id="7bfbb-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7bfbb-160">deleteditems</span><span class="sxs-lookup"><span data-stu-id="7bfbb-160">deleteditems</span></span>|<span data-ttu-id="7bfbb-161">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="7bfbb-161">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="7bfbb-162">Недавно удаленные элементы.</span><span class="sxs-lookup"><span data-stu-id="7bfbb-162">Recently deleted items.</span></span> <span data-ttu-id="7bfbb-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7bfbb-163">Read-only.</span></span> <span data-ttu-id="7bfbb-164">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7bfbb-164">Nullable.</span></span>|
|<span data-ttu-id="7bfbb-165">featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="7bfbb-165">featureRolloutPolicies</span></span>|<span data-ttu-id="7bfbb-166">[коллекция featureRolloutPolicy](featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="7bfbb-166">[featureRolloutPolicy](featurerolloutpolicy.md) collection</span></span>| <span data-ttu-id="7bfbb-167">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="7bfbb-167">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7bfbb-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7bfbb-168">JSON representation</span></span>
<span data-ttu-id="7bfbb-169">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7bfbb-169">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
  "id": "String (identifier)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


