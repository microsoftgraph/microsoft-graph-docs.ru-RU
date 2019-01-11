---
title: Тип ресурса directory (удаленные элементы)
description: . Удаленные элементы можно восстановить в течение 30 дней. Через 30 дней элементы удаляются без возможности восстановления.
localization_priority: Normal
ms.openlocfilehash: e8ccecfd0d8cffa383ecc96cc908d31452db5fb0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835772"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="60b75-105">Тип ресурса directory (удаленные элементы)</span><span class="sxs-lookup"><span data-stu-id="60b75-105">directory resource type (deleted items)</span></span>

<span data-ttu-id="60b75-106">Представляет удаленный элемент в каталоге.</span><span class="sxs-lookup"><span data-stu-id="60b75-106">Represents a deleted item in the directory.</span></span> <span data-ttu-id="60b75-107">После удаления элемент добавляется в "контейнер" удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="60b75-107">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="60b75-108">Удаленные элементы можно восстановить в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="60b75-108">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="60b75-109">Через 30 дней элементы удаляются без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="60b75-109">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="60b75-110">В настоящее время хранение удаленных элементов поддерживается только для [групп](group.md) и [пользователей](users.md) Office 365.</span><span class="sxs-lookup"><span data-stu-id="60b75-110">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="60b75-111">Методы</span><span class="sxs-lookup"><span data-stu-id="60b75-111">Methods</span></span>

| <span data-ttu-id="60b75-112">Метод</span><span class="sxs-lookup"><span data-stu-id="60b75-112">Method</span></span>         | <span data-ttu-id="60b75-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="60b75-113">Return Type</span></span> | <span data-ttu-id="60b75-114">Описание</span><span class="sxs-lookup"><span data-stu-id="60b75-114">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="60b75-115">Получение удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="60b75-115">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="60b75-116">directoryObject</span><span class="sxs-lookup"><span data-stu-id="60b75-116">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="60b75-117">Получает свойства удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="60b75-117">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="60b75-118">Восстановление удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="60b75-118">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="60b75-119">directoryObject</span><span class="sxs-lookup"><span data-stu-id="60b75-119">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="60b75-120">Восстанавливает недавно удаленный элемент.</span><span class="sxs-lookup"><span data-stu-id="60b75-120">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="60b75-121">Перечисление удаленных элементов</span><span class="sxs-lookup"><span data-stu-id="60b75-121">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="60b75-122">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="60b75-122">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="60b75-123">Получает список недавно удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="60b75-123">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="60b75-124">Окончательное удаление элемента</span><span class="sxs-lookup"><span data-stu-id="60b75-124">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="60b75-125">None</span><span class="sxs-lookup"><span data-stu-id="60b75-125">None</span></span> | <span data-ttu-id="60b75-126">Окончательно удаляет элемент.</span><span class="sxs-lookup"><span data-stu-id="60b75-126">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="60b75-127">Список удаленных элементов, принадлежащие пользователю</span><span class="sxs-lookup"><span data-stu-id="60b75-127">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="60b75-128">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="60b75-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="60b75-129">Список элементов каталога, принадлежащие пользователю.</span><span class="sxs-lookup"><span data-stu-id="60b75-129">Lists directory items owned by a user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="60b75-130">Связи</span><span class="sxs-lookup"><span data-stu-id="60b75-130">Relationships</span></span>
| <span data-ttu-id="60b75-131">Связь</span><span class="sxs-lookup"><span data-stu-id="60b75-131">Relationship</span></span> | <span data-ttu-id="60b75-132">Тип</span><span class="sxs-lookup"><span data-stu-id="60b75-132">Type</span></span>   |<span data-ttu-id="60b75-133">Описание</span><span class="sxs-lookup"><span data-stu-id="60b75-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60b75-134">deletedItems</span><span class="sxs-lookup"><span data-stu-id="60b75-134">deletedItems</span></span>|<span data-ttu-id="60b75-135">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="60b75-135">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="60b75-136">Недавно удаленные элементы.</span><span class="sxs-lookup"><span data-stu-id="60b75-136">Recently deleted items.</span></span> <span data-ttu-id="60b75-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="60b75-137">Read-only.</span></span> <span data-ttu-id="60b75-138">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="60b75-138">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="60b75-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="60b75-139">JSON representation</span></span>
<span data-ttu-id="60b75-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60b75-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="60b75-141">Пример</span><span class="sxs-lookup"><span data-stu-id="60b75-141">Example</span></span>

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
