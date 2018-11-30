---
title: Тип ресурса directory (удаленные элементы)
description: . Удаленные элементы можно восстановить в течение 30 дней. Через 30 дней элементы удаляются без возможности восстановления.
ms.openlocfilehash: 74b4d1ff94b567557fd90701b1c4bae479a8317e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082007"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="61461-105">Тип ресурса directory (удаленные элементы)</span><span class="sxs-lookup"><span data-stu-id="61461-105">directory resource type (deleted items)</span></span>

> <span data-ttu-id="61461-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="61461-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="61461-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61461-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="61461-108">Представляет удаленный элемент в каталоге.</span><span class="sxs-lookup"><span data-stu-id="61461-108">Represents a deleted item in the directory.</span></span> <span data-ttu-id="61461-109">После удаления элемент добавляется в "контейнер" удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="61461-109">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="61461-110">Удаленные элементы можно восстановить в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="61461-110">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="61461-111">Через 30 дней элементы удаляются без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="61461-111">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="61461-112">В настоящее время хранение удаленных элементов поддерживается только для [групп](group.md) и [пользователей](users.md) Office 365.</span><span class="sxs-lookup"><span data-stu-id="61461-112">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="61461-113">Методы</span><span class="sxs-lookup"><span data-stu-id="61461-113">Methods</span></span>

| <span data-ttu-id="61461-114">Метод</span><span class="sxs-lookup"><span data-stu-id="61461-114">Method</span></span>         | <span data-ttu-id="61461-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="61461-115">Return Type</span></span> | <span data-ttu-id="61461-116">Описание</span><span class="sxs-lookup"><span data-stu-id="61461-116">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="61461-117">Получение удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="61461-117">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="61461-118">directoryObject</span><span class="sxs-lookup"><span data-stu-id="61461-118">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="61461-119">Получает свойства удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="61461-119">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="61461-120">Восстановление удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="61461-120">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="61461-121">directoryObject</span><span class="sxs-lookup"><span data-stu-id="61461-121">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="61461-122">Восстанавливает недавно удаленный элемент.</span><span class="sxs-lookup"><span data-stu-id="61461-122">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="61461-123">Перечисление удаленных элементов</span><span class="sxs-lookup"><span data-stu-id="61461-123">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="61461-124">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="61461-124">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="61461-125">Получает список недавно удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="61461-125">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="61461-126">Окончательное удаление элемента</span><span class="sxs-lookup"><span data-stu-id="61461-126">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="61461-127">None</span><span class="sxs-lookup"><span data-stu-id="61461-127">None</span></span> | <span data-ttu-id="61461-128">Окончательно удаляет элемент.</span><span class="sxs-lookup"><span data-stu-id="61461-128">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="61461-129">Список удаленных элементов, принадлежащие пользователю</span><span class="sxs-lookup"><span data-stu-id="61461-129">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="61461-130">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="61461-130">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="61461-131">Список элементов каталога, принадлежащие пользователю.</span><span class="sxs-lookup"><span data-stu-id="61461-131">Lists directory items owned by a user.</span></span> |

## <a name="properties"></a><span data-ttu-id="61461-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="61461-132">Properties</span></span>
| <span data-ttu-id="61461-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="61461-133">Property</span></span>   | <span data-ttu-id="61461-134">Тип</span><span class="sxs-lookup"><span data-stu-id="61461-134">Type</span></span> |<span data-ttu-id="61461-135">Описание</span><span class="sxs-lookup"><span data-stu-id="61461-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61461-136">id</span><span class="sxs-lookup"><span data-stu-id="61461-136">id</span></span>|<span data-ttu-id="61461-137">String</span><span class="sxs-lookup"><span data-stu-id="61461-137">String</span></span>| <span data-ttu-id="61461-138">Уникальный идентификатор объекта, например 12345678-9abc-def0-1234-56789abcde.</span><span class="sxs-lookup"><span data-stu-id="61461-138">A unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="61461-139">Ключ.</span><span class="sxs-lookup"><span data-stu-id="61461-139">Key.</span></span> <span data-ttu-id="61461-140">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="61461-140">Not nullable.</span></span> <span data-ttu-id="61461-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="61461-141">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61461-142">Связи</span><span class="sxs-lookup"><span data-stu-id="61461-142">Relationships</span></span>
| <span data-ttu-id="61461-143">Связь</span><span class="sxs-lookup"><span data-stu-id="61461-143">Relationship</span></span> | <span data-ttu-id="61461-144">Тип</span><span class="sxs-lookup"><span data-stu-id="61461-144">Type</span></span>   |<span data-ttu-id="61461-145">Описание</span><span class="sxs-lookup"><span data-stu-id="61461-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61461-146">deleteditems</span><span class="sxs-lookup"><span data-stu-id="61461-146">deleteditems</span></span>|<span data-ttu-id="61461-147">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="61461-147">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="61461-148">Недавно удаленные элементы.</span><span class="sxs-lookup"><span data-stu-id="61461-148">Recently deleted items.</span></span> <span data-ttu-id="61461-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="61461-149">Read-only.</span></span> <span data-ttu-id="61461-150">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="61461-150">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="61461-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="61461-151">JSON representation</span></span>
<span data-ttu-id="61461-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="61461-152">Here is a JSON representation of the resource.</span></span>

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