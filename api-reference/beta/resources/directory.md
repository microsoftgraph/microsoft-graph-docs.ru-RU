---
title: Тип ресурса directory (удаленные элементы)
description: . Удаленные элементы можно восстановить в течение 30 дней. Через 30 дней элементы удаляются без возможности восстановления.
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 4eb1cbdcbf0a1256c2bf2bf0cec35479b8bbc2cc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962625"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="5359f-105">Тип ресурса directory (удаленные элементы)</span><span class="sxs-lookup"><span data-stu-id="5359f-105">directory resource type (deleted items)</span></span>

<span data-ttu-id="5359f-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5359f-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5359f-107">Представляет удаленный элемент в каталоге.</span><span class="sxs-lookup"><span data-stu-id="5359f-107">Represents a deleted item in the directory.</span></span> <span data-ttu-id="5359f-108">После удаления элемент добавляется в "контейнер" удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="5359f-108">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="5359f-109">Удаленные элементы можно восстановить в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="5359f-109">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="5359f-110">Через 30 дней элементы удаляются без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="5359f-110">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="5359f-111">В настоящее время функции удаленных элементов поддерживаются только для [приложений,](application.md) [групповых и](group.md) [пользовательских](user.md) ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5359f-111">Currently, deleted items functionality is only supported for the [application](application.md), [group](group.md) and [user](user.md) resources.</span></span>

## <a name="methods"></a><span data-ttu-id="5359f-112">Методы</span><span class="sxs-lookup"><span data-stu-id="5359f-112">Methods</span></span>

| <span data-ttu-id="5359f-113">Метод</span><span class="sxs-lookup"><span data-stu-id="5359f-113">Method</span></span>         | <span data-ttu-id="5359f-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5359f-114">Return Type</span></span> | <span data-ttu-id="5359f-115">Описание</span><span class="sxs-lookup"><span data-stu-id="5359f-115">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="5359f-116">Получение удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="5359f-116">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="5359f-117">directoryObject</span><span class="sxs-lookup"><span data-stu-id="5359f-117">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="5359f-118">Получает свойства удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="5359f-118">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="5359f-119">Восстановление удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="5359f-119">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="5359f-120">directoryObject</span><span class="sxs-lookup"><span data-stu-id="5359f-120">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="5359f-121">Восстанавливает недавно удаленный элемент.</span><span class="sxs-lookup"><span data-stu-id="5359f-121">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="5359f-122">Перечисление удаленных элементов</span><span class="sxs-lookup"><span data-stu-id="5359f-122">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="5359f-123">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="5359f-123">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="5359f-124">Получает список недавно удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="5359f-124">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="5359f-125">Окончательное удаление элемента</span><span class="sxs-lookup"><span data-stu-id="5359f-125">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="5359f-126">None</span><span class="sxs-lookup"><span data-stu-id="5359f-126">None</span></span> | <span data-ttu-id="5359f-127">Окончательно удаляет элемент.</span><span class="sxs-lookup"><span data-stu-id="5359f-127">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="5359f-128">Список удаленных элементов, которые принадлежат пользователю</span><span class="sxs-lookup"><span data-stu-id="5359f-128">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="5359f-129">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="5359f-129">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="5359f-130">Списки элементов каталогов, которые принадлежат пользователю.</span><span class="sxs-lookup"><span data-stu-id="5359f-130">Lists directory items owned by a user.</span></span> |
|[<span data-ttu-id="5359f-131">Функция ListRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="5359f-131">List featureRolloutPolicies</span></span>](../api/list-featurerolloutpolicies.md) | <span data-ttu-id="5359f-132">[коллекция featureRolloutPolicy](featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5359f-132">[featureRolloutPolicy](featurerolloutpolicy.md) collection</span></span> | <span data-ttu-id="5359f-133">Извлечение списка объектов featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="5359f-133">Retrieve a list of featureRolloutPolicy objects.</span></span> |
|[<span data-ttu-id="5359f-134">Создание featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="5359f-134">Create featureRolloutPolicy</span></span>](../api/post-featurerolloutpolicies.md) | [<span data-ttu-id="5359f-135">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="5359f-135">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="5359f-136">Создайте новый объект featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="5359f-136">Create a new featureRolloutPolicy object.</span></span> |
| [<span data-ttu-id="5359f-137">Get featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="5359f-137">Get featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-get.md) | [<span data-ttu-id="5359f-138">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="5359f-138">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="5359f-139">Извлечение свойств и связей объекта featurerolloutpolicy.</span><span class="sxs-lookup"><span data-stu-id="5359f-139">Retrieve the properties and relationships of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="5359f-140">Обновление функцииRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="5359f-140">Update featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-update.md) | [<span data-ttu-id="5359f-141">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="5359f-141">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="5359f-142">Обновление свойств объекта featurerolloutpolicy.</span><span class="sxs-lookup"><span data-stu-id="5359f-142">Update the properties of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="5359f-143">Удаление featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="5359f-143">Delete featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-delete.md) | <span data-ttu-id="5359f-144">Нет</span><span class="sxs-lookup"><span data-stu-id="5359f-144">None</span></span> | <span data-ttu-id="5359f-145">Удаление объекта featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="5359f-145">Delete a featureRolloutPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5359f-146">Свойства</span><span class="sxs-lookup"><span data-stu-id="5359f-146">Properties</span></span>
| <span data-ttu-id="5359f-147">Свойство</span><span class="sxs-lookup"><span data-stu-id="5359f-147">Property</span></span>   | <span data-ttu-id="5359f-148">Тип</span><span class="sxs-lookup"><span data-stu-id="5359f-148">Type</span></span> |<span data-ttu-id="5359f-149">Описание</span><span class="sxs-lookup"><span data-stu-id="5359f-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5359f-150">id</span><span class="sxs-lookup"><span data-stu-id="5359f-150">id</span></span>|<span data-ttu-id="5359f-151">Строка</span><span class="sxs-lookup"><span data-stu-id="5359f-151">String</span></span>| <span data-ttu-id="5359f-152">Уникальный идентификатор объекта, например 12345678-9abc-def0-1234-56789abcde.</span><span class="sxs-lookup"><span data-stu-id="5359f-152">A unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="5359f-153">Ключ.</span><span class="sxs-lookup"><span data-stu-id="5359f-153">Key.</span></span> <span data-ttu-id="5359f-154">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="5359f-154">Not nullable.</span></span> <span data-ttu-id="5359f-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5359f-155">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5359f-156">Связи</span><span class="sxs-lookup"><span data-stu-id="5359f-156">Relationships</span></span>
| <span data-ttu-id="5359f-157">Связь</span><span class="sxs-lookup"><span data-stu-id="5359f-157">Relationship</span></span> | <span data-ttu-id="5359f-158">Тип</span><span class="sxs-lookup"><span data-stu-id="5359f-158">Type</span></span>   |<span data-ttu-id="5359f-159">Описание</span><span class="sxs-lookup"><span data-stu-id="5359f-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5359f-160">deleteditems</span><span class="sxs-lookup"><span data-stu-id="5359f-160">deleteditems</span></span>|<span data-ttu-id="5359f-161">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="5359f-161">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="5359f-162">Недавно удаленные элементы.</span><span class="sxs-lookup"><span data-stu-id="5359f-162">Recently deleted items.</span></span> <span data-ttu-id="5359f-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5359f-163">Read-only.</span></span> <span data-ttu-id="5359f-164">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5359f-164">Nullable.</span></span>|
|<span data-ttu-id="5359f-165">featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="5359f-165">featureRolloutPolicies</span></span>|<span data-ttu-id="5359f-166">[коллекция featureRolloutPolicy](featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5359f-166">[featureRolloutPolicy](featurerolloutpolicy.md) collection</span></span>| <span data-ttu-id="5359f-167">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5359f-167">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5359f-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5359f-168">JSON representation</span></span>
<span data-ttu-id="5359f-169">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5359f-169">Here is a JSON representation of the resource.</span></span>

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


