---
title: Тип ресурса directory (удаленные элементы)
description: . Удаленные элементы можно восстановить в течение 30 дней. Через 30 дней элементы удаляются без возможности восстановления.
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9e2c3e750754f7932e55a315c909c5186bb5a4f6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049823"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="a9604-105">Тип ресурса directory (удаленные элементы)</span><span class="sxs-lookup"><span data-stu-id="a9604-105">directory resource type (deleted items)</span></span>

<span data-ttu-id="a9604-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9604-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9604-107">Представляет удаленный элемент в каталоге.</span><span class="sxs-lookup"><span data-stu-id="a9604-107">Represents a deleted item in the directory.</span></span> <span data-ttu-id="a9604-108">После удаления элемент добавляется в "контейнер" удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="a9604-108">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="a9604-109">Удаленные элементы можно восстановить в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="a9604-109">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="a9604-110">Через 30 дней элементы удаляются без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="a9604-110">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="a9604-111">В настоящее время функции удаленных элементов поддерживаются только для ресурсов [приложения](application.md), [групп](group.md) и [пользователей](user.md) .</span><span class="sxs-lookup"><span data-stu-id="a9604-111">Currently, deleted items functionality is only supported for the [application](application.md), [group](group.md) and [user](user.md) resources.</span></span>

## <a name="methods"></a><span data-ttu-id="a9604-112">Методы</span><span class="sxs-lookup"><span data-stu-id="a9604-112">Methods</span></span>

| <span data-ttu-id="a9604-113">Метод</span><span class="sxs-lookup"><span data-stu-id="a9604-113">Method</span></span>         | <span data-ttu-id="a9604-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a9604-114">Return Type</span></span> | <span data-ttu-id="a9604-115">Описание</span><span class="sxs-lookup"><span data-stu-id="a9604-115">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="a9604-116">Получение удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="a9604-116">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="a9604-117">directoryObject</span><span class="sxs-lookup"><span data-stu-id="a9604-117">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="a9604-118">Получает свойства удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="a9604-118">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="a9604-119">Восстановление удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="a9604-119">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="a9604-120">directoryObject</span><span class="sxs-lookup"><span data-stu-id="a9604-120">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="a9604-121">Восстанавливает недавно удаленный элемент.</span><span class="sxs-lookup"><span data-stu-id="a9604-121">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="a9604-122">Перечисление удаленных элементов</span><span class="sxs-lookup"><span data-stu-id="a9604-122">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="a9604-123">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="a9604-123">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="a9604-124">Получает список недавно удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="a9604-124">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="a9604-125">Окончательное удаление элемента</span><span class="sxs-lookup"><span data-stu-id="a9604-125">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="a9604-126">None</span><span class="sxs-lookup"><span data-stu-id="a9604-126">None</span></span> | <span data-ttu-id="a9604-127">Окончательно удаляет элемент.</span><span class="sxs-lookup"><span data-stu-id="a9604-127">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="a9604-128">Список удаленных элементов, принадлежащих пользователю</span><span class="sxs-lookup"><span data-stu-id="a9604-128">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="a9604-129">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="a9604-129">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="a9604-130">Список элементов каталога, принадлежащих пользователю.</span><span class="sxs-lookup"><span data-stu-id="a9604-130">Lists directory items owned by a user.</span></span> |
|[<span data-ttu-id="a9604-131">Список ФеатурероллаутполиЦиес</span><span class="sxs-lookup"><span data-stu-id="a9604-131">List featureRolloutPolicies</span></span>](../api/directory-list-featurerolloutpolicies.md) | <span data-ttu-id="a9604-132">Коллекция [феатурероллаутполици](featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a9604-132">[featureRolloutPolicy](featurerolloutpolicy.md) collection</span></span> | <span data-ttu-id="a9604-133">Получение списка объектов Феатурероллаутполици.</span><span class="sxs-lookup"><span data-stu-id="a9604-133">Retrieve a list of featureRolloutPolicy objects.</span></span> |
|[<span data-ttu-id="a9604-134">Создание Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="a9604-134">Create featureRolloutPolicy</span></span>](../api/directory-post-featurerolloutpolicies.md) | [<span data-ttu-id="a9604-135">феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="a9604-135">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="a9604-136">Создание нового объекта Феатурероллаутполици.</span><span class="sxs-lookup"><span data-stu-id="a9604-136">Create a new featureRolloutPolicy object.</span></span> |
| [<span data-ttu-id="a9604-137">Получение Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="a9604-137">Get featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-get.md) | [<span data-ttu-id="a9604-138">феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="a9604-138">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="a9604-139">Получение свойств и связей объекта феатурероллаутполици.</span><span class="sxs-lookup"><span data-stu-id="a9604-139">Retrieve the properties and relationships of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="a9604-140">Обновление Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="a9604-140">Update featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-update.md) | [<span data-ttu-id="a9604-141">феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="a9604-141">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="a9604-142">Обновление свойств объекта феатурероллаутполици.</span><span class="sxs-lookup"><span data-stu-id="a9604-142">Update the properties of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="a9604-143">Удаление Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="a9604-143">Delete featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-delete.md) | <span data-ttu-id="a9604-144">Нет</span><span class="sxs-lookup"><span data-stu-id="a9604-144">None</span></span> | <span data-ttu-id="a9604-145">Удаление объекта Феатурероллаутполици.</span><span class="sxs-lookup"><span data-stu-id="a9604-145">Delete a featureRolloutPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a9604-146">Свойства</span><span class="sxs-lookup"><span data-stu-id="a9604-146">Properties</span></span>
| <span data-ttu-id="a9604-147">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9604-147">Property</span></span>   | <span data-ttu-id="a9604-148">Тип</span><span class="sxs-lookup"><span data-stu-id="a9604-148">Type</span></span> |<span data-ttu-id="a9604-149">Описание</span><span class="sxs-lookup"><span data-stu-id="a9604-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a9604-150">id</span><span class="sxs-lookup"><span data-stu-id="a9604-150">id</span></span>|<span data-ttu-id="a9604-151">Строка</span><span class="sxs-lookup"><span data-stu-id="a9604-151">String</span></span>| <span data-ttu-id="a9604-152">Уникальный идентификатор объекта, например 12345678-9abc-def0-1234-56789abcde.</span><span class="sxs-lookup"><span data-stu-id="a9604-152">A unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="a9604-153">Ключ.</span><span class="sxs-lookup"><span data-stu-id="a9604-153">Key.</span></span> <span data-ttu-id="a9604-154">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="a9604-154">Not nullable.</span></span> <span data-ttu-id="a9604-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a9604-155">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9604-156">Отношения</span><span class="sxs-lookup"><span data-stu-id="a9604-156">Relationships</span></span>
| <span data-ttu-id="a9604-157">Связь</span><span class="sxs-lookup"><span data-stu-id="a9604-157">Relationship</span></span> | <span data-ttu-id="a9604-158">Тип</span><span class="sxs-lookup"><span data-stu-id="a9604-158">Type</span></span>   |<span data-ttu-id="a9604-159">Описание</span><span class="sxs-lookup"><span data-stu-id="a9604-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a9604-160">deleteditems</span><span class="sxs-lookup"><span data-stu-id="a9604-160">deleteditems</span></span>|<span data-ttu-id="a9604-161">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="a9604-161">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="a9604-162">Недавно удаленные элементы.</span><span class="sxs-lookup"><span data-stu-id="a9604-162">Recently deleted items.</span></span> <span data-ttu-id="a9604-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a9604-163">Read-only.</span></span> <span data-ttu-id="a9604-164">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="a9604-164">Nullable.</span></span>|
|<span data-ttu-id="a9604-165">феатурероллаутполиЦиес</span><span class="sxs-lookup"><span data-stu-id="a9604-165">featureRolloutPolicies</span></span>|<span data-ttu-id="a9604-166">Коллекция [феатурероллаутполици](featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a9604-166">[featureRolloutPolicy](featurerolloutpolicy.md) collection</span></span>| <span data-ttu-id="a9604-167">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="a9604-167">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a9604-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a9604-168">JSON representation</span></span>
<span data-ttu-id="a9604-169">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9604-169">Here is a JSON representation of the resource.</span></span>

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


