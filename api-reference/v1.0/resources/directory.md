---
title: Тип ресурса directory (удаленные элементы)
description: . Удаленные элементы можно восстановить в течение 30 дней. Через 30 дней элементы удаляются без возможности восстановления.
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 9c46e671f707a8e31c172e4a078647cd7d103d48
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472736"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="c060d-105">Тип ресурса directory (удаленные элементы)</span><span class="sxs-lookup"><span data-stu-id="c060d-105">directory resource type (deleted items)</span></span>

<span data-ttu-id="c060d-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c060d-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c060d-107">Представляет удаленный элемент в каталоге.</span><span class="sxs-lookup"><span data-stu-id="c060d-107">Represents a deleted item in the directory.</span></span> <span data-ttu-id="c060d-108">После удаления элемент добавляется в "контейнер" удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="c060d-108">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="c060d-109">Удаленные элементы можно восстановить в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="c060d-109">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="c060d-110">Через 30 дней элементы удаляются без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="c060d-110">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="c060d-111">В настоящее время функции удаленных элементов поддерживаются только для [приложений,](application.md) [групповых и](group.md) [пользовательских](user.md) ресурсов.</span><span class="sxs-lookup"><span data-stu-id="c060d-111">Currently, deleted items functionality is only supported for the [application](application.md), [group](group.md) and [user](user.md) resources.</span></span>

## <a name="methods"></a><span data-ttu-id="c060d-112">Методы</span><span class="sxs-lookup"><span data-stu-id="c060d-112">Methods</span></span>

| <span data-ttu-id="c060d-113">Метод</span><span class="sxs-lookup"><span data-stu-id="c060d-113">Method</span></span>         | <span data-ttu-id="c060d-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c060d-114">Return Type</span></span> | <span data-ttu-id="c060d-115">Описание</span><span class="sxs-lookup"><span data-stu-id="c060d-115">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="c060d-116">Получение удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="c060d-116">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="c060d-117">directoryObject</span><span class="sxs-lookup"><span data-stu-id="c060d-117">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="c060d-118">Получает свойства удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="c060d-118">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="c060d-119">Восстановление удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="c060d-119">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="c060d-120">directoryObject</span><span class="sxs-lookup"><span data-stu-id="c060d-120">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="c060d-121">Восстанавливает недавно удаленный элемент.</span><span class="sxs-lookup"><span data-stu-id="c060d-121">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="c060d-122">Перечисление удаленных элементов</span><span class="sxs-lookup"><span data-stu-id="c060d-122">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="c060d-123">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="c060d-123">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="c060d-124">Получает список недавно удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="c060d-124">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="c060d-125">Окончательное удаление элемента</span><span class="sxs-lookup"><span data-stu-id="c060d-125">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="c060d-126">None</span><span class="sxs-lookup"><span data-stu-id="c060d-126">None</span></span> | <span data-ttu-id="c060d-127">Окончательно удаляет элемент.</span><span class="sxs-lookup"><span data-stu-id="c060d-127">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="c060d-128">Список удаленных элементов, которые принадлежат пользователю</span><span class="sxs-lookup"><span data-stu-id="c060d-128">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="c060d-129">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="c060d-129">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="c060d-130">Списки элементов каталогов, которые принадлежат пользователю.</span><span class="sxs-lookup"><span data-stu-id="c060d-130">Lists directory items owned by a user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c060d-131">Связи</span><span class="sxs-lookup"><span data-stu-id="c060d-131">Relationships</span></span>
| <span data-ttu-id="c060d-132">Связь</span><span class="sxs-lookup"><span data-stu-id="c060d-132">Relationship</span></span> | <span data-ttu-id="c060d-133">Тип</span><span class="sxs-lookup"><span data-stu-id="c060d-133">Type</span></span>   |<span data-ttu-id="c060d-134">Описание</span><span class="sxs-lookup"><span data-stu-id="c060d-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c060d-135">deletedItems</span><span class="sxs-lookup"><span data-stu-id="c060d-135">deletedItems</span></span>|<span data-ttu-id="c060d-136">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="c060d-136">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="c060d-137">Недавно удаленные элементы.</span><span class="sxs-lookup"><span data-stu-id="c060d-137">Recently deleted items.</span></span> <span data-ttu-id="c060d-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c060d-138">Read-only.</span></span> <span data-ttu-id="c060d-139">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c060d-139">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c060d-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c060d-140">JSON representation</span></span>
<span data-ttu-id="c060d-141">Ниже показано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c060d-141">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="c060d-142">Пример</span><span class="sxs-lookup"><span data-stu-id="c060d-142">Example</span></span>

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/directory
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.directory"}-->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
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

