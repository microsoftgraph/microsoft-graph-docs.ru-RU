---
title: Тип ресурса directory (удаленные элементы)
description: . Удаленные элементы можно восстановить в течение 30 дней. Через 30 дней элементы удаляются без возможности восстановления.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 09f6059ca10b64e30aab06f4dd9ee4f3dc281ef4
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34658038"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="8f84b-105">Тип ресурса directory (удаленные элементы)</span><span class="sxs-lookup"><span data-stu-id="8f84b-105">directory resource type (deleted items)</span></span>

<span data-ttu-id="8f84b-106">Представляет удаленный элемент в каталоге.</span><span class="sxs-lookup"><span data-stu-id="8f84b-106">Represents a deleted item in the directory.</span></span> <span data-ttu-id="8f84b-107">После удаления элемент добавляется в "контейнер" удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="8f84b-107">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="8f84b-108">Удаленные элементы можно восстановить в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="8f84b-108">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="8f84b-109">Через 30 дней элементы удаляются без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="8f84b-109">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="8f84b-110">В настоящее время хранение удаленных элементов поддерживается только для [групп](group.md) и [пользователей](users.md) Office 365.</span><span class="sxs-lookup"><span data-stu-id="8f84b-110">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="8f84b-111">Методы</span><span class="sxs-lookup"><span data-stu-id="8f84b-111">Methods</span></span>

| <span data-ttu-id="8f84b-112">Метод</span><span class="sxs-lookup"><span data-stu-id="8f84b-112">Method</span></span>         | <span data-ttu-id="8f84b-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8f84b-113">Return Type</span></span> | <span data-ttu-id="8f84b-114">Описание</span><span class="sxs-lookup"><span data-stu-id="8f84b-114">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="8f84b-115">Получение удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="8f84b-115">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="8f84b-116">directoryObject</span><span class="sxs-lookup"><span data-stu-id="8f84b-116">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="8f84b-117">Получает свойства удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="8f84b-117">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="8f84b-118">Восстановление удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="8f84b-118">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="8f84b-119">directoryObject</span><span class="sxs-lookup"><span data-stu-id="8f84b-119">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="8f84b-120">Восстанавливает недавно удаленный элемент.</span><span class="sxs-lookup"><span data-stu-id="8f84b-120">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="8f84b-121">Перечисление удаленных элементов</span><span class="sxs-lookup"><span data-stu-id="8f84b-121">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="8f84b-122">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="8f84b-122">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="8f84b-123">Получает список недавно удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="8f84b-123">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="8f84b-124">Окончательное удаление элемента</span><span class="sxs-lookup"><span data-stu-id="8f84b-124">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="8f84b-125">None</span><span class="sxs-lookup"><span data-stu-id="8f84b-125">None</span></span> | <span data-ttu-id="8f84b-126">Окончательно удаляет элемент.</span><span class="sxs-lookup"><span data-stu-id="8f84b-126">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="8f84b-127">Список удаленных элементов, принадлежащих пользователю</span><span class="sxs-lookup"><span data-stu-id="8f84b-127">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="8f84b-128">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="8f84b-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="8f84b-129">Список элементов каталога, принадлежащих пользователю.</span><span class="sxs-lookup"><span data-stu-id="8f84b-129">Lists directory items owned by a user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8f84b-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="8f84b-130">Relationships</span></span>
| <span data-ttu-id="8f84b-131">Отношение</span><span class="sxs-lookup"><span data-stu-id="8f84b-131">Relationship</span></span> | <span data-ttu-id="8f84b-132">Тип</span><span class="sxs-lookup"><span data-stu-id="8f84b-132">Type</span></span>   |<span data-ttu-id="8f84b-133">Описание</span><span class="sxs-lookup"><span data-stu-id="8f84b-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f84b-134">deletedItems</span><span class="sxs-lookup"><span data-stu-id="8f84b-134">deletedItems</span></span>|<span data-ttu-id="8f84b-135">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="8f84b-135">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="8f84b-136">Недавно удаленные элементы.</span><span class="sxs-lookup"><span data-stu-id="8f84b-136">Recently deleted items.</span></span> <span data-ttu-id="8f84b-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8f84b-137">Read-only.</span></span> <span data-ttu-id="8f84b-138">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="8f84b-138">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8f84b-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8f84b-139">JSON representation</span></span>
<span data-ttu-id="8f84b-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f84b-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="8f84b-141">Пример</span><span class="sxs-lookup"><span data-stu-id="8f84b-141">Example</span></span>

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
