---
title: Тип ресурса directory (удаленные элементы)
description: . Удаленные элементы можно восстановить в течение 30 дней. Через 30 дней элементы удаляются без возможности восстановления.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ba2c40e5987ee8b6bd89e4385c4c6bf242084edd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012809"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="fc4b3-105">Тип ресурса directory (удаленные элементы)</span><span class="sxs-lookup"><span data-stu-id="fc4b3-105">directory resource type (deleted items)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc4b3-106">Представляет удаленный элемент в каталоге.</span><span class="sxs-lookup"><span data-stu-id="fc4b3-106">Represents a deleted item in the directory.</span></span> <span data-ttu-id="fc4b3-107">После удаления элемент добавляется в "контейнер" удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="fc4b3-107">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="fc4b3-108">Удаленные элементы можно восстановить в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="fc4b3-108">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="fc4b3-109">Через 30 дней элементы удаляются без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="fc4b3-109">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="fc4b3-110">В настоящее время хранение удаленных элементов поддерживается только для [групп](group.md) и [пользователей](users.md) Office 365.</span><span class="sxs-lookup"><span data-stu-id="fc4b3-110">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="fc4b3-111">Методы</span><span class="sxs-lookup"><span data-stu-id="fc4b3-111">Methods</span></span>

| <span data-ttu-id="fc4b3-112">Метод</span><span class="sxs-lookup"><span data-stu-id="fc4b3-112">Method</span></span>         | <span data-ttu-id="fc4b3-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fc4b3-113">Return Type</span></span> | <span data-ttu-id="fc4b3-114">Описание</span><span class="sxs-lookup"><span data-stu-id="fc4b3-114">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="fc4b3-115">Получение удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="fc4b3-115">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="fc4b3-116">directoryObject</span><span class="sxs-lookup"><span data-stu-id="fc4b3-116">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="fc4b3-117">Получает свойства удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="fc4b3-117">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="fc4b3-118">Восстановление удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="fc4b3-118">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="fc4b3-119">directoryObject</span><span class="sxs-lookup"><span data-stu-id="fc4b3-119">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="fc4b3-120">Восстанавливает недавно удаленный элемент.</span><span class="sxs-lookup"><span data-stu-id="fc4b3-120">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="fc4b3-121">Перечисление удаленных элементов</span><span class="sxs-lookup"><span data-stu-id="fc4b3-121">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="fc4b3-122">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="fc4b3-122">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="fc4b3-123">Получает список недавно удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="fc4b3-123">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="fc4b3-124">Окончательное удаление элемента</span><span class="sxs-lookup"><span data-stu-id="fc4b3-124">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="fc4b3-125">None</span><span class="sxs-lookup"><span data-stu-id="fc4b3-125">None</span></span> | <span data-ttu-id="fc4b3-126">Окончательно удаляет элемент.</span><span class="sxs-lookup"><span data-stu-id="fc4b3-126">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="fc4b3-127">Список удаленных элементов, принадлежащих пользователю</span><span class="sxs-lookup"><span data-stu-id="fc4b3-127">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="fc4b3-128">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="fc4b3-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="fc4b3-129">Список элементов каталога, принадлежащих пользователю.</span><span class="sxs-lookup"><span data-stu-id="fc4b3-129">Lists directory items owned by a user.</span></span> |

## <a name="properties"></a><span data-ttu-id="fc4b3-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc4b3-130">Properties</span></span>
| <span data-ttu-id="fc4b3-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc4b3-131">Property</span></span>   | <span data-ttu-id="fc4b3-132">Тип</span><span class="sxs-lookup"><span data-stu-id="fc4b3-132">Type</span></span> |<span data-ttu-id="fc4b3-133">Описание</span><span class="sxs-lookup"><span data-stu-id="fc4b3-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc4b3-134">id</span><span class="sxs-lookup"><span data-stu-id="fc4b3-134">id</span></span>|<span data-ttu-id="fc4b3-135">String</span><span class="sxs-lookup"><span data-stu-id="fc4b3-135">String</span></span>| <span data-ttu-id="fc4b3-136">Уникальный идентификатор объекта, например 12345678-9abc-def0-1234-56789abcde.</span><span class="sxs-lookup"><span data-stu-id="fc4b3-136">A unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="fc4b3-137">Ключ.</span><span class="sxs-lookup"><span data-stu-id="fc4b3-137">Key.</span></span> <span data-ttu-id="fc4b3-138">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="fc4b3-138">Not nullable.</span></span> <span data-ttu-id="fc4b3-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fc4b3-139">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc4b3-140">Отношения</span><span class="sxs-lookup"><span data-stu-id="fc4b3-140">Relationships</span></span>
| <span data-ttu-id="fc4b3-141">Отношение</span><span class="sxs-lookup"><span data-stu-id="fc4b3-141">Relationship</span></span> | <span data-ttu-id="fc4b3-142">Тип</span><span class="sxs-lookup"><span data-stu-id="fc4b3-142">Type</span></span>   |<span data-ttu-id="fc4b3-143">Описание</span><span class="sxs-lookup"><span data-stu-id="fc4b3-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc4b3-144">deleteditems</span><span class="sxs-lookup"><span data-stu-id="fc4b3-144">deleteditems</span></span>|<span data-ttu-id="fc4b3-145">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="fc4b3-145">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="fc4b3-146">Недавно удаленные элементы.</span><span class="sxs-lookup"><span data-stu-id="fc4b3-146">Recently deleted items.</span></span> <span data-ttu-id="fc4b3-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fc4b3-147">Read-only.</span></span> <span data-ttu-id="fc4b3-148">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="fc4b3-148">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fc4b3-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fc4b3-149">JSON representation</span></span>
<span data-ttu-id="fc4b3-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc4b3-150">Here is a JSON representation of the resource.</span></span>

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
