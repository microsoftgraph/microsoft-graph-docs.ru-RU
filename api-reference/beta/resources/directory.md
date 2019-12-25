---
title: Тип ресурса directory (удаленные элементы)
description: . Удаленные элементы можно восстановить в течение 30 дней. Через 30 дней элементы удаляются без возможности восстановления.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fb03e368a8a9c5cf929f314714a3a5d2fdee4b93
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866849"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="816de-105">Тип ресурса directory (удаленные элементы)</span><span class="sxs-lookup"><span data-stu-id="816de-105">directory resource type (deleted items)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="816de-106">Представляет удаленный элемент в каталоге.</span><span class="sxs-lookup"><span data-stu-id="816de-106">Represents a deleted item in the directory.</span></span> <span data-ttu-id="816de-107">После удаления элемент добавляется в "контейнер" удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="816de-107">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="816de-108">Удаленные элементы можно восстановить в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="816de-108">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="816de-109">Через 30 дней элементы удаляются без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="816de-109">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="816de-110">В настоящее время функции удаленных элементов поддерживаются только для ресурсов [приложения](application.md), [групп](group.md) и [пользователей](user.md) .</span><span class="sxs-lookup"><span data-stu-id="816de-110">Currently, deleted items functionality is only supported for the [application](application.md), [group](group.md) and [user](user.md) resources.</span></span>

## <a name="methods"></a><span data-ttu-id="816de-111">Методы</span><span class="sxs-lookup"><span data-stu-id="816de-111">Methods</span></span>

| <span data-ttu-id="816de-112">Метод</span><span class="sxs-lookup"><span data-stu-id="816de-112">Method</span></span>         | <span data-ttu-id="816de-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="816de-113">Return Type</span></span> | <span data-ttu-id="816de-114">Описание</span><span class="sxs-lookup"><span data-stu-id="816de-114">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="816de-115">Получение удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="816de-115">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="816de-116">directoryObject</span><span class="sxs-lookup"><span data-stu-id="816de-116">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="816de-117">Получает свойства удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="816de-117">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="816de-118">Восстановление удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="816de-118">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="816de-119">directoryObject</span><span class="sxs-lookup"><span data-stu-id="816de-119">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="816de-120">Восстанавливает недавно удаленный элемент.</span><span class="sxs-lookup"><span data-stu-id="816de-120">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="816de-121">Перечисление удаленных элементов</span><span class="sxs-lookup"><span data-stu-id="816de-121">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="816de-122">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="816de-122">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="816de-123">Получает список недавно удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="816de-123">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="816de-124">Окончательное удаление элемента</span><span class="sxs-lookup"><span data-stu-id="816de-124">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="816de-125">None</span><span class="sxs-lookup"><span data-stu-id="816de-125">None</span></span> | <span data-ttu-id="816de-126">Окончательно удаляет элемент.</span><span class="sxs-lookup"><span data-stu-id="816de-126">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="816de-127">Список удаленных элементов, принадлежащих пользователю</span><span class="sxs-lookup"><span data-stu-id="816de-127">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="816de-128">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="816de-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="816de-129">Список элементов каталога, принадлежащих пользователю.</span><span class="sxs-lookup"><span data-stu-id="816de-129">Lists directory items owned by a user.</span></span> |
|[<span data-ttu-id="816de-130">Список ФеатурероллаутполиЦиес</span><span class="sxs-lookup"><span data-stu-id="816de-130">List featureRolloutPolicies</span></span>](../api/directory-list-featurerolloutpolicies.md) | <span data-ttu-id="816de-131">Коллекция [феатурероллаутполици](featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="816de-131">[featureRolloutPolicy](featurerolloutpolicy.md) collection</span></span> | <span data-ttu-id="816de-132">Получение списка объектов Феатурероллаутполици.</span><span class="sxs-lookup"><span data-stu-id="816de-132">Retrieve a list of featureRolloutPolicy objects.</span></span> |
|[<span data-ttu-id="816de-133">Создание Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="816de-133">Create featureRolloutPolicy</span></span>](../api/directory-post-featurerolloutpolicies.md) | [<span data-ttu-id="816de-134">феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="816de-134">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="816de-135">Создание нового объекта Феатурероллаутполици.</span><span class="sxs-lookup"><span data-stu-id="816de-135">Create a new featureRolloutPolicy object.</span></span> |
| [<span data-ttu-id="816de-136">Получение Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="816de-136">Get featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-get.md) | [<span data-ttu-id="816de-137">феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="816de-137">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="816de-138">Получение свойств и связей объекта феатурероллаутполици.</span><span class="sxs-lookup"><span data-stu-id="816de-138">Retrieve the properties and relationships of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="816de-139">Обновление Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="816de-139">Update featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-update.md) | [<span data-ttu-id="816de-140">феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="816de-140">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="816de-141">Обновление свойств объекта феатурероллаутполици.</span><span class="sxs-lookup"><span data-stu-id="816de-141">Update the properties of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="816de-142">Удаление Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="816de-142">Delete featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-delete.md) | <span data-ttu-id="816de-143">Нет.</span><span class="sxs-lookup"><span data-stu-id="816de-143">None</span></span> | <span data-ttu-id="816de-144">Удаление объекта Феатурероллаутполици.</span><span class="sxs-lookup"><span data-stu-id="816de-144">Delete a featureRolloutPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="816de-145">Свойства</span><span class="sxs-lookup"><span data-stu-id="816de-145">Properties</span></span>
| <span data-ttu-id="816de-146">Свойство</span><span class="sxs-lookup"><span data-stu-id="816de-146">Property</span></span>   | <span data-ttu-id="816de-147">Тип</span><span class="sxs-lookup"><span data-stu-id="816de-147">Type</span></span> |<span data-ttu-id="816de-148">Описание</span><span class="sxs-lookup"><span data-stu-id="816de-148">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="816de-149">id</span><span class="sxs-lookup"><span data-stu-id="816de-149">id</span></span>|<span data-ttu-id="816de-150">String</span><span class="sxs-lookup"><span data-stu-id="816de-150">String</span></span>| <span data-ttu-id="816de-151">Уникальный идентификатор объекта, например 12345678-9abc-def0-1234-56789abcde.</span><span class="sxs-lookup"><span data-stu-id="816de-151">A unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="816de-152">Ключ.</span><span class="sxs-lookup"><span data-stu-id="816de-152">Key.</span></span> <span data-ttu-id="816de-153">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="816de-153">Not nullable.</span></span> <span data-ttu-id="816de-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="816de-154">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="816de-155">Отношения</span><span class="sxs-lookup"><span data-stu-id="816de-155">Relationships</span></span>
| <span data-ttu-id="816de-156">Связь</span><span class="sxs-lookup"><span data-stu-id="816de-156">Relationship</span></span> | <span data-ttu-id="816de-157">Тип</span><span class="sxs-lookup"><span data-stu-id="816de-157">Type</span></span>   |<span data-ttu-id="816de-158">Описание</span><span class="sxs-lookup"><span data-stu-id="816de-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="816de-159">deleteditems</span><span class="sxs-lookup"><span data-stu-id="816de-159">deleteditems</span></span>|<span data-ttu-id="816de-160">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="816de-160">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="816de-161">Недавно удаленные элементы.</span><span class="sxs-lookup"><span data-stu-id="816de-161">Recently deleted items.</span></span> <span data-ttu-id="816de-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="816de-162">Read-only.</span></span> <span data-ttu-id="816de-163">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="816de-163">Nullable.</span></span>|
|<span data-ttu-id="816de-164">феатурероллаутполиЦиес</span><span class="sxs-lookup"><span data-stu-id="816de-164">featureRolloutPolicies</span></span>|<span data-ttu-id="816de-165">Коллекция [феатурероллаутполици](featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="816de-165">[featureRolloutPolicy](featurerolloutpolicy.md) collection</span></span>| <span data-ttu-id="816de-166">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="816de-166">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="816de-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="816de-167">JSON representation</span></span>
<span data-ttu-id="816de-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="816de-168">Here is a JSON representation of the resource.</span></span>

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
