---
title: Тип ресурса directory (удаленные элементы)
description: . Удаленные элементы можно восстановить в течение 30 дней. Через 30 дней элементы удаляются без возможности восстановления.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2593603afa145d30b5e26a240bb5cd471eab9942
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966554"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="1513a-105">Тип ресурса directory (удаленные элементы)</span><span class="sxs-lookup"><span data-stu-id="1513a-105">directory resource type (deleted items)</span></span>

> <span data-ttu-id="1513a-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1513a-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1513a-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1513a-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1513a-108">Представляет удаленный элемент в каталоге.</span><span class="sxs-lookup"><span data-stu-id="1513a-108">Represents a deleted item in the directory.</span></span> <span data-ttu-id="1513a-109">После удаления элемент добавляется в "контейнер" удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="1513a-109">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="1513a-110">Удаленные элементы можно восстановить в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="1513a-110">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="1513a-111">Через 30 дней элементы удаляются без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="1513a-111">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="1513a-112">В настоящее время хранение удаленных элементов поддерживается только для [групп](group.md) и [пользователей](users.md) Office 365.</span><span class="sxs-lookup"><span data-stu-id="1513a-112">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1513a-113">Методы</span><span class="sxs-lookup"><span data-stu-id="1513a-113">Methods</span></span>

| <span data-ttu-id="1513a-114">Метод</span><span class="sxs-lookup"><span data-stu-id="1513a-114">Method</span></span>         | <span data-ttu-id="1513a-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1513a-115">Return Type</span></span> | <span data-ttu-id="1513a-116">Описание</span><span class="sxs-lookup"><span data-stu-id="1513a-116">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="1513a-117">Получение удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="1513a-117">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="1513a-118">directoryObject</span><span class="sxs-lookup"><span data-stu-id="1513a-118">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="1513a-119">Получает свойства удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="1513a-119">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="1513a-120">Восстановление удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="1513a-120">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="1513a-121">directoryObject</span><span class="sxs-lookup"><span data-stu-id="1513a-121">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="1513a-122">Восстанавливает недавно удаленный элемент.</span><span class="sxs-lookup"><span data-stu-id="1513a-122">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="1513a-123">Перечисление удаленных элементов</span><span class="sxs-lookup"><span data-stu-id="1513a-123">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="1513a-124">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="1513a-124">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="1513a-125">Получает список недавно удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="1513a-125">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="1513a-126">Окончательное удаление элемента</span><span class="sxs-lookup"><span data-stu-id="1513a-126">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="1513a-127">None</span><span class="sxs-lookup"><span data-stu-id="1513a-127">None</span></span> | <span data-ttu-id="1513a-128">Окончательно удаляет элемент.</span><span class="sxs-lookup"><span data-stu-id="1513a-128">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="1513a-129">Список удаленных элементов, принадлежащие пользователю</span><span class="sxs-lookup"><span data-stu-id="1513a-129">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="1513a-130">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="1513a-130">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="1513a-131">Список элементов каталога, принадлежащие пользователю.</span><span class="sxs-lookup"><span data-stu-id="1513a-131">Lists directory items owned by a user.</span></span> |

## <a name="properties"></a><span data-ttu-id="1513a-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="1513a-132">Properties</span></span>
| <span data-ttu-id="1513a-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="1513a-133">Property</span></span>   | <span data-ttu-id="1513a-134">Тип</span><span class="sxs-lookup"><span data-stu-id="1513a-134">Type</span></span> |<span data-ttu-id="1513a-135">Описание</span><span class="sxs-lookup"><span data-stu-id="1513a-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1513a-136">id</span><span class="sxs-lookup"><span data-stu-id="1513a-136">id</span></span>|<span data-ttu-id="1513a-137">String</span><span class="sxs-lookup"><span data-stu-id="1513a-137">String</span></span>| <span data-ttu-id="1513a-138">Уникальный идентификатор объекта, например 12345678-9abc-def0-1234-56789abcde.</span><span class="sxs-lookup"><span data-stu-id="1513a-138">A unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="1513a-139">Ключ.</span><span class="sxs-lookup"><span data-stu-id="1513a-139">Key.</span></span> <span data-ttu-id="1513a-140">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="1513a-140">Not nullable.</span></span> <span data-ttu-id="1513a-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1513a-141">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1513a-142">Связи</span><span class="sxs-lookup"><span data-stu-id="1513a-142">Relationships</span></span>
| <span data-ttu-id="1513a-143">Связь</span><span class="sxs-lookup"><span data-stu-id="1513a-143">Relationship</span></span> | <span data-ttu-id="1513a-144">Тип</span><span class="sxs-lookup"><span data-stu-id="1513a-144">Type</span></span>   |<span data-ttu-id="1513a-145">Описание</span><span class="sxs-lookup"><span data-stu-id="1513a-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1513a-146">deleteditems</span><span class="sxs-lookup"><span data-stu-id="1513a-146">deleteditems</span></span>|<span data-ttu-id="1513a-147">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="1513a-147">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="1513a-148">Недавно удаленные элементы.</span><span class="sxs-lookup"><span data-stu-id="1513a-148">Recently deleted items.</span></span> <span data-ttu-id="1513a-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1513a-149">Read-only.</span></span> <span data-ttu-id="1513a-150">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="1513a-150">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1513a-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1513a-151">JSON representation</span></span>
<span data-ttu-id="1513a-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1513a-152">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
<!-- {
  "type": "#page.annotation",
  "description": "directory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
