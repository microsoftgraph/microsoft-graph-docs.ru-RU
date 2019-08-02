---
title: Тип ресурса directory (удаленные элементы)
description: . Удаленные элементы можно восстановить в течение 30 дней. Через 30 дней элементы удаляются без возможности восстановления.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4b35c2c56c7033cd668b311c17169f5c719e5948
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062084"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="4dfe0-105">Тип ресурса directory (удаленные элементы)</span><span class="sxs-lookup"><span data-stu-id="4dfe0-105">directory resource type (deleted items)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4dfe0-106">Представляет удаленный элемент в каталоге.</span><span class="sxs-lookup"><span data-stu-id="4dfe0-106">Represents a deleted item in the directory.</span></span> <span data-ttu-id="4dfe0-107">После удаления элемент добавляется в "контейнер" удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="4dfe0-107">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="4dfe0-108">Удаленные элементы можно восстановить в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="4dfe0-108">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="4dfe0-109">Через 30 дней элементы удаляются без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="4dfe0-109">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="4dfe0-110">В настоящее время хранение удаленных элементов поддерживается только для [групп](group.md) и [пользователей](users.md) Office 365.</span><span class="sxs-lookup"><span data-stu-id="4dfe0-110">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4dfe0-111">Методы</span><span class="sxs-lookup"><span data-stu-id="4dfe0-111">Methods</span></span>

| <span data-ttu-id="4dfe0-112">Метод</span><span class="sxs-lookup"><span data-stu-id="4dfe0-112">Method</span></span>         | <span data-ttu-id="4dfe0-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4dfe0-113">Return Type</span></span> | <span data-ttu-id="4dfe0-114">Описание</span><span class="sxs-lookup"><span data-stu-id="4dfe0-114">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="4dfe0-115">Получение удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="4dfe0-115">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="4dfe0-116">directoryObject</span><span class="sxs-lookup"><span data-stu-id="4dfe0-116">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="4dfe0-117">Получает свойства удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="4dfe0-117">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="4dfe0-118">Восстановление удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="4dfe0-118">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="4dfe0-119">directoryObject</span><span class="sxs-lookup"><span data-stu-id="4dfe0-119">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="4dfe0-120">Восстанавливает недавно удаленный элемент.</span><span class="sxs-lookup"><span data-stu-id="4dfe0-120">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="4dfe0-121">Перечисление удаленных элементов</span><span class="sxs-lookup"><span data-stu-id="4dfe0-121">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="4dfe0-122">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="4dfe0-122">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="4dfe0-123">Получает список недавно удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="4dfe0-123">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="4dfe0-124">Окончательное удаление элемента</span><span class="sxs-lookup"><span data-stu-id="4dfe0-124">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="4dfe0-125">None</span><span class="sxs-lookup"><span data-stu-id="4dfe0-125">None</span></span> | <span data-ttu-id="4dfe0-126">Окончательно удаляет элемент.</span><span class="sxs-lookup"><span data-stu-id="4dfe0-126">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="4dfe0-127">Список удаленных элементов, принадлежащих пользователю</span><span class="sxs-lookup"><span data-stu-id="4dfe0-127">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="4dfe0-128">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="4dfe0-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="4dfe0-129">Список элементов каталога, принадлежащих пользователю.</span><span class="sxs-lookup"><span data-stu-id="4dfe0-129">Lists directory items owned by a user.</span></span> |
|[<span data-ttu-id="4dfe0-130">Список ФеатурероллаутполиЦиес</span><span class="sxs-lookup"><span data-stu-id="4dfe0-130">List featureRolloutPolicies</span></span>](../api/directory-list-featurerolloutpolicies.md) | <span data-ttu-id="4dfe0-131">Коллекция [феатурероллаутполици](featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4dfe0-131">[featureRolloutPolicy](featurerolloutpolicy.md) collection</span></span> | <span data-ttu-id="4dfe0-132">Получение списка объектов Феатурероллаутполици.</span><span class="sxs-lookup"><span data-stu-id="4dfe0-132">Retrieve a list of featureRolloutPolicy objects.</span></span> |
|[<span data-ttu-id="4dfe0-133">Создание Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="4dfe0-133">Create featureRolloutPolicy</span></span>](../api/directory-post-featurerolloutpolicies.md) | [<span data-ttu-id="4dfe0-134">Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="4dfe0-134">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="4dfe0-135">Создание нового объекта Феатурероллаутполици.</span><span class="sxs-lookup"><span data-stu-id="4dfe0-135">Create a new featureRolloutPolicy object.</span></span> |
| [<span data-ttu-id="4dfe0-136">Получение Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="4dfe0-136">Get featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-get.md) | [<span data-ttu-id="4dfe0-137">Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="4dfe0-137">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="4dfe0-138">Получение свойств и связей объекта феатурероллаутполици.</span><span class="sxs-lookup"><span data-stu-id="4dfe0-138">Retrieve the properties and relationships of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="4dfe0-139">Обновление Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="4dfe0-139">Update featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-update.md) | [<span data-ttu-id="4dfe0-140">Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="4dfe0-140">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="4dfe0-141">Обновление свойств объекта феатурероллаутполици.</span><span class="sxs-lookup"><span data-stu-id="4dfe0-141">Update the properties of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="4dfe0-142">Удаление Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="4dfe0-142">Delete featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-delete.md) | <span data-ttu-id="4dfe0-143">Нет</span><span class="sxs-lookup"><span data-stu-id="4dfe0-143">None</span></span> | <span data-ttu-id="4dfe0-144">Удаление объекта Феатурероллаутполици.</span><span class="sxs-lookup"><span data-stu-id="4dfe0-144">Delete a featureRolloutPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4dfe0-145">Свойства</span><span class="sxs-lookup"><span data-stu-id="4dfe0-145">Properties</span></span>
| <span data-ttu-id="4dfe0-146">Свойство</span><span class="sxs-lookup"><span data-stu-id="4dfe0-146">Property</span></span>   | <span data-ttu-id="4dfe0-147">Тип</span><span class="sxs-lookup"><span data-stu-id="4dfe0-147">Type</span></span> |<span data-ttu-id="4dfe0-148">Описание</span><span class="sxs-lookup"><span data-stu-id="4dfe0-148">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4dfe0-149">id</span><span class="sxs-lookup"><span data-stu-id="4dfe0-149">id</span></span>|<span data-ttu-id="4dfe0-150">String</span><span class="sxs-lookup"><span data-stu-id="4dfe0-150">String</span></span>| <span data-ttu-id="4dfe0-151">Уникальный идентификатор объекта, например 12345678-9abc-def0-1234-56789abcde.</span><span class="sxs-lookup"><span data-stu-id="4dfe0-151">A unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="4dfe0-152">Ключ.</span><span class="sxs-lookup"><span data-stu-id="4dfe0-152">Key.</span></span> <span data-ttu-id="4dfe0-153">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="4dfe0-153">Not nullable.</span></span> <span data-ttu-id="4dfe0-154">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4dfe0-154">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4dfe0-155">Отношения</span><span class="sxs-lookup"><span data-stu-id="4dfe0-155">Relationships</span></span>
| <span data-ttu-id="4dfe0-156">Отношение</span><span class="sxs-lookup"><span data-stu-id="4dfe0-156">Relationship</span></span> | <span data-ttu-id="4dfe0-157">Тип</span><span class="sxs-lookup"><span data-stu-id="4dfe0-157">Type</span></span>   |<span data-ttu-id="4dfe0-158">Описание</span><span class="sxs-lookup"><span data-stu-id="4dfe0-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4dfe0-159">deleteditems</span><span class="sxs-lookup"><span data-stu-id="4dfe0-159">deleteditems</span></span>|<span data-ttu-id="4dfe0-160">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="4dfe0-160">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="4dfe0-161">Недавно удаленные элементы.</span><span class="sxs-lookup"><span data-stu-id="4dfe0-161">Recently deleted items.</span></span> <span data-ttu-id="4dfe0-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4dfe0-162">Read-only.</span></span> <span data-ttu-id="4dfe0-163">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4dfe0-163">Nullable.</span></span>|
|<span data-ttu-id="4dfe0-164">ФеатурероллаутполиЦиес</span><span class="sxs-lookup"><span data-stu-id="4dfe0-164">featureRolloutPolicies</span></span>|<span data-ttu-id="4dfe0-165">Коллекция [феатурероллаутполици](featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="4dfe0-165">[featureRolloutPolicy](featurerolloutpolicy.md) collection</span></span>| <span data-ttu-id="4dfe0-166">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4dfe0-166">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4dfe0-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4dfe0-167">JSON representation</span></span>
<span data-ttu-id="4dfe0-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4dfe0-168">Here is a JSON representation of the resource.</span></span>

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
