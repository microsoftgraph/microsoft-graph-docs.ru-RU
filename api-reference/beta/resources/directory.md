---
title: Тип ресурса directory (удаленные элементы)
description: . Удаленные элементы можно восстановить в течение 30 дней. Через 30 дней элементы удаляются без возможности восстановления.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e9437f2f57c1ac53dc8f227149e679edd32d1ff1
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657688"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="21955-105">Тип ресурса directory (удаленные элементы)</span><span class="sxs-lookup"><span data-stu-id="21955-105">directory resource type (deleted items)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21955-106">Представляет удаленный элемент в каталоге.</span><span class="sxs-lookup"><span data-stu-id="21955-106">Represents a deleted item in the directory.</span></span> <span data-ttu-id="21955-107">После удаления элемент добавляется в "контейнер" удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="21955-107">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="21955-108">Удаленные элементы можно восстановить в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="21955-108">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="21955-109">Через 30 дней элементы удаляются без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="21955-109">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="21955-110">В настоящее время хранение удаленных элементов поддерживается только для [групп](group.md) и [пользователей](users.md) Office 365.</span><span class="sxs-lookup"><span data-stu-id="21955-110">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="21955-111">Методы</span><span class="sxs-lookup"><span data-stu-id="21955-111">Methods</span></span>

| <span data-ttu-id="21955-112">Метод</span><span class="sxs-lookup"><span data-stu-id="21955-112">Method</span></span>         | <span data-ttu-id="21955-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="21955-113">Return Type</span></span> | <span data-ttu-id="21955-114">Описание</span><span class="sxs-lookup"><span data-stu-id="21955-114">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="21955-115">Получение удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="21955-115">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="21955-116">directoryObject</span><span class="sxs-lookup"><span data-stu-id="21955-116">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="21955-117">Получает свойства удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="21955-117">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="21955-118">Восстановление удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="21955-118">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="21955-119">directoryObject</span><span class="sxs-lookup"><span data-stu-id="21955-119">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="21955-120">Восстанавливает недавно удаленный элемент.</span><span class="sxs-lookup"><span data-stu-id="21955-120">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="21955-121">Перечисление удаленных элементов</span><span class="sxs-lookup"><span data-stu-id="21955-121">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="21955-122">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="21955-122">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="21955-123">Получает список недавно удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="21955-123">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="21955-124">Окончательное удаление элемента</span><span class="sxs-lookup"><span data-stu-id="21955-124">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="21955-125">None</span><span class="sxs-lookup"><span data-stu-id="21955-125">None</span></span> | <span data-ttu-id="21955-126">Окончательно удаляет элемент.</span><span class="sxs-lookup"><span data-stu-id="21955-126">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="21955-127">Список удаленных элементов, принадлежащих пользователю</span><span class="sxs-lookup"><span data-stu-id="21955-127">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="21955-128">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="21955-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="21955-129">Список элементов каталога, принадлежащих пользователю.</span><span class="sxs-lookup"><span data-stu-id="21955-129">Lists directory items owned by a user.</span></span> |

## <a name="properties"></a><span data-ttu-id="21955-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="21955-130">Properties</span></span>
| <span data-ttu-id="21955-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="21955-131">Property</span></span>   | <span data-ttu-id="21955-132">Тип</span><span class="sxs-lookup"><span data-stu-id="21955-132">Type</span></span> |<span data-ttu-id="21955-133">Описание</span><span class="sxs-lookup"><span data-stu-id="21955-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21955-134">id</span><span class="sxs-lookup"><span data-stu-id="21955-134">id</span></span>|<span data-ttu-id="21955-135">String</span><span class="sxs-lookup"><span data-stu-id="21955-135">String</span></span>| <span data-ttu-id="21955-136">Уникальный идентификатор объекта, например 12345678-9abc-def0-1234-56789abcde.</span><span class="sxs-lookup"><span data-stu-id="21955-136">A unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="21955-137">Ключ.</span><span class="sxs-lookup"><span data-stu-id="21955-137">Key.</span></span> <span data-ttu-id="21955-138">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="21955-138">Not nullable.</span></span> <span data-ttu-id="21955-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="21955-139">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21955-140">Отношения</span><span class="sxs-lookup"><span data-stu-id="21955-140">Relationships</span></span>
| <span data-ttu-id="21955-141">Отношение</span><span class="sxs-lookup"><span data-stu-id="21955-141">Relationship</span></span> | <span data-ttu-id="21955-142">Тип</span><span class="sxs-lookup"><span data-stu-id="21955-142">Type</span></span>   |<span data-ttu-id="21955-143">Описание</span><span class="sxs-lookup"><span data-stu-id="21955-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21955-144">deleteditems</span><span class="sxs-lookup"><span data-stu-id="21955-144">deleteditems</span></span>|<span data-ttu-id="21955-145">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="21955-145">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="21955-146">Недавно удаленные элементы.</span><span class="sxs-lookup"><span data-stu-id="21955-146">Recently deleted items.</span></span> <span data-ttu-id="21955-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="21955-147">Read-only.</span></span> <span data-ttu-id="21955-148">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="21955-148">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="21955-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="21955-149">JSON representation</span></span>
<span data-ttu-id="21955-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21955-150">Here is a JSON representation of the resource.</span></span>

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
