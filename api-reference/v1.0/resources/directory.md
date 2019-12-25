---
title: Тип ресурса directory (удаленные элементы)
description: . Удаленные элементы можно восстановить в течение 30 дней. Через 30 дней элементы удаляются без возможности восстановления.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f820e0b3111a73f0f88be5d01a37d7891e48ac42
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863909"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="ba884-105">Тип ресурса directory (удаленные элементы)</span><span class="sxs-lookup"><span data-stu-id="ba884-105">directory resource type (deleted items)</span></span>

<span data-ttu-id="ba884-106">Представляет удаленный элемент в каталоге.</span><span class="sxs-lookup"><span data-stu-id="ba884-106">Represents a deleted item in the directory.</span></span> <span data-ttu-id="ba884-107">После удаления элемент добавляется в "контейнер" удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="ba884-107">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="ba884-108">Удаленные элементы можно восстановить в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="ba884-108">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="ba884-109">Через 30 дней элементы удаляются без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="ba884-109">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="ba884-110">В настоящее время функции удаленных элементов поддерживаются только для ресурсов [приложения](application.md), [групп](group.md) и [пользователей](user.md) .</span><span class="sxs-lookup"><span data-stu-id="ba884-110">Currently, deleted items functionality is only supported for the [application](application.md), [group](group.md) and [user](user.md) resources.</span></span>

## <a name="methods"></a><span data-ttu-id="ba884-111">Методы</span><span class="sxs-lookup"><span data-stu-id="ba884-111">Methods</span></span>

| <span data-ttu-id="ba884-112">Метод</span><span class="sxs-lookup"><span data-stu-id="ba884-112">Method</span></span>         | <span data-ttu-id="ba884-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ba884-113">Return Type</span></span> | <span data-ttu-id="ba884-114">Описание</span><span class="sxs-lookup"><span data-stu-id="ba884-114">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="ba884-115">Получение удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="ba884-115">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="ba884-116">directoryObject</span><span class="sxs-lookup"><span data-stu-id="ba884-116">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="ba884-117">Получает свойства удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="ba884-117">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="ba884-118">Восстановление удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="ba884-118">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="ba884-119">directoryObject</span><span class="sxs-lookup"><span data-stu-id="ba884-119">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="ba884-120">Восстанавливает недавно удаленный элемент.</span><span class="sxs-lookup"><span data-stu-id="ba884-120">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="ba884-121">Перечисление удаленных элементов</span><span class="sxs-lookup"><span data-stu-id="ba884-121">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="ba884-122">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="ba884-122">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="ba884-123">Получает список недавно удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="ba884-123">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="ba884-124">Окончательное удаление элемента</span><span class="sxs-lookup"><span data-stu-id="ba884-124">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="ba884-125">None</span><span class="sxs-lookup"><span data-stu-id="ba884-125">None</span></span> | <span data-ttu-id="ba884-126">Окончательно удаляет элемент.</span><span class="sxs-lookup"><span data-stu-id="ba884-126">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="ba884-127">Список удаленных элементов, принадлежащих пользователю</span><span class="sxs-lookup"><span data-stu-id="ba884-127">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="ba884-128">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="ba884-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="ba884-129">Список элементов каталога, принадлежащих пользователю.</span><span class="sxs-lookup"><span data-stu-id="ba884-129">Lists directory items owned by a user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ba884-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="ba884-130">Relationships</span></span>
| <span data-ttu-id="ba884-131">Связь</span><span class="sxs-lookup"><span data-stu-id="ba884-131">Relationship</span></span> | <span data-ttu-id="ba884-132">Тип</span><span class="sxs-lookup"><span data-stu-id="ba884-132">Type</span></span>   |<span data-ttu-id="ba884-133">Описание</span><span class="sxs-lookup"><span data-stu-id="ba884-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba884-134">deletedItems</span><span class="sxs-lookup"><span data-stu-id="ba884-134">deletedItems</span></span>|<span data-ttu-id="ba884-135">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="ba884-135">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="ba884-136">Недавно удаленные элементы.</span><span class="sxs-lookup"><span data-stu-id="ba884-136">Recently deleted items.</span></span> <span data-ttu-id="ba884-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ba884-137">Read-only.</span></span> <span data-ttu-id="ba884-138">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ba884-138">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ba884-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ba884-139">JSON representation</span></span>
<span data-ttu-id="ba884-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba884-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="ba884-141">Пример</span><span class="sxs-lookup"><span data-stu-id="ba884-141">Example</span></span>

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/directory
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.directory"}-->
```json
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
