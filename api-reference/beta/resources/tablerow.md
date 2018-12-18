---
title: Тип ресурса TableRow
description: Представляет строку в таблице.
author: lumine2008
ms.openlocfilehash: de83ec8cae87f159c6f1f9687bd093873558c150
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309886"
---
# <a name="tablerow-resource-type"></a><span data-ttu-id="668e3-103">Тип ресурса TableRow</span><span class="sxs-lookup"><span data-stu-id="668e3-103">TableRow resource type</span></span>

> <span data-ttu-id="668e3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="668e3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="668e3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="668e3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="668e3-106">Представляет строку в таблице.</span><span class="sxs-lookup"><span data-stu-id="668e3-106">Represents a row in a table.</span></span>


## <a name="methods"></a><span data-ttu-id="668e3-107">Методы</span><span class="sxs-lookup"><span data-stu-id="668e3-107">Methods</span></span>

| <span data-ttu-id="668e3-108">Метод</span><span class="sxs-lookup"><span data-stu-id="668e3-108">Method</span></span>           | <span data-ttu-id="668e3-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="668e3-109">Return Type</span></span>    |<span data-ttu-id="668e3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="668e3-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="668e3-111">Получение объекта TableRow</span><span class="sxs-lookup"><span data-stu-id="668e3-111">Get TableRow</span></span>](../api/tablerow-get.md) | [<span data-ttu-id="668e3-112">TableRow</span><span class="sxs-lookup"><span data-stu-id="668e3-112">TableRow</span></span>](tablerow.md) |<span data-ttu-id="668e3-113">Чтение свойств и связей объекта tableRow.</span><span class="sxs-lookup"><span data-stu-id="668e3-113">Read properties and relationships of tableRow object.</span></span>|
|<span data-ttu-id="668e3-114">[обновление](../api/tablerow-update.md).</span><span class="sxs-lookup"><span data-stu-id="668e3-114">[Update](../api/tablerow-update.md)</span></span> | [<span data-ttu-id="668e3-115">TableRow</span><span class="sxs-lookup"><span data-stu-id="668e3-115">TableRow</span></span>](tablerow.md)  |<span data-ttu-id="668e3-116">Обновление объекта tableRow.</span><span class="sxs-lookup"><span data-stu-id="668e3-116">Update TableRow object.</span></span> |
|[<span data-ttu-id="668e3-117">Range</span><span class="sxs-lookup"><span data-stu-id="668e3-117">Range</span></span>](../api/tablerow-range.md)|[<span data-ttu-id="668e3-118">Range</span><span class="sxs-lookup"><span data-stu-id="668e3-118">Range</span></span>](range.md)|<span data-ttu-id="668e3-119">Возвращает объект диапазона, связанный со всей строкой.</span><span class="sxs-lookup"><span data-stu-id="668e3-119">Returns the range object associated with the entire row.</span></span>|
|[<span data-ttu-id="668e3-120">Delete</span><span class="sxs-lookup"><span data-stu-id="668e3-120">Delete</span></span>](../api/tablerow-delete.md)|<span data-ttu-id="668e3-121">Нет</span><span class="sxs-lookup"><span data-stu-id="668e3-121">None</span></span>|<span data-ttu-id="668e3-122">Удаляет строку из таблицы.</span><span class="sxs-lookup"><span data-stu-id="668e3-122">Deletes the row from the table.</span></span>|
|[<span data-ttu-id="668e3-123">List</span><span class="sxs-lookup"><span data-stu-id="668e3-123">List</span></span>](../api/tablerow-list.md) | <span data-ttu-id="668e3-124">Коллекция объектов [TableRow](tablerow.md)</span><span class="sxs-lookup"><span data-stu-id="668e3-124">[TableRow](tablerow.md) collection</span></span> |<span data-ttu-id="668e3-125">Получение коллекции объектов tableRow.</span><span class="sxs-lookup"><span data-stu-id="668e3-125">Get tableRow object collection.</span></span> |
|[<span data-ttu-id="668e3-126">Itemat</span><span class="sxs-lookup"><span data-stu-id="668e3-126">Itemat</span></span>](../api/tablerowcollection-itemat.md)|[<span data-ttu-id="668e3-127">TableRow</span><span class="sxs-lookup"><span data-stu-id="668e3-127">TableRow</span></span>](tablerow.md)|<span data-ttu-id="668e3-128">Получает строку на основании сведений о ее позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="668e3-128">Gets a row based on its position in the collection.</span></span>|
|[<span data-ttu-id="668e3-129">Add</span><span class="sxs-lookup"><span data-stu-id="668e3-129">Add</span></span>](../api/tablerowcollection-add.md)|[<span data-ttu-id="668e3-130">TableRow</span><span class="sxs-lookup"><span data-stu-id="668e3-130">TableRow</span></span>](tablerow.md)|<span data-ttu-id="668e3-131">Добавляет новую строку в таблицу.</span><span class="sxs-lookup"><span data-stu-id="668e3-131">Adds a new row to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="668e3-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="668e3-132">Properties</span></span>
| <span data-ttu-id="668e3-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="668e3-133">Property</span></span>     | <span data-ttu-id="668e3-134">Тип</span><span class="sxs-lookup"><span data-stu-id="668e3-134">Type</span></span>   |<span data-ttu-id="668e3-135">Описание</span><span class="sxs-lookup"><span data-stu-id="668e3-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="668e3-136">index</span><span class="sxs-lookup"><span data-stu-id="668e3-136">index</span></span>|<span data-ttu-id="668e3-137">целое</span><span class="sxs-lookup"><span data-stu-id="668e3-137">int</span></span>|<span data-ttu-id="668e3-p102">Возвращает номер индекса строки в коллекции строк таблицы. Используется нулевой индекс. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="668e3-p102">Returns the index number of the row within the rows collection of the table. Zero-indexed. Read-only.</span></span>|
|<span data-ttu-id="668e3-141">values</span><span class="sxs-lookup"><span data-stu-id="668e3-141">values</span></span>|<span data-ttu-id="668e3-142">json</span><span class="sxs-lookup"><span data-stu-id="668e3-142">json</span></span>|<span data-ttu-id="668e3-p103">Представляет необработанные значения указанного диапазона. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.</span><span class="sxs-lookup"><span data-stu-id="668e3-p103">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="relationships"></a><span data-ttu-id="668e3-146">Связи</span><span class="sxs-lookup"><span data-stu-id="668e3-146">Relationships</span></span>
<span data-ttu-id="668e3-147">Нет</span><span class="sxs-lookup"><span data-stu-id="668e3-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="668e3-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="668e3-148">JSON representation</span></span>

<span data-ttu-id="668e3-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="668e3-149">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tableRow"
}-->

```json
{
  "index": 1024,
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->