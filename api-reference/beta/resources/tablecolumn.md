---
title: Тип ресурса TableColumn
description: Представляет столбец в таблице.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 8534a2f47478a68c305f2acbe98b87df032982e6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885493"
---
# <a name="tablecolumn-resource-type"></a><span data-ttu-id="50ce2-103">Тип ресурса TableColumn</span><span class="sxs-lookup"><span data-stu-id="50ce2-103">TableColumn resource type</span></span>

> <span data-ttu-id="50ce2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="50ce2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="50ce2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50ce2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="50ce2-106">Представляет столбец в таблице.</span><span class="sxs-lookup"><span data-stu-id="50ce2-106">Represents a column in a table.</span></span>


## <a name="methods"></a><span data-ttu-id="50ce2-107">Методы</span><span class="sxs-lookup"><span data-stu-id="50ce2-107">Methods</span></span>

| <span data-ttu-id="50ce2-108">Метод</span><span class="sxs-lookup"><span data-stu-id="50ce2-108">Method</span></span>           | <span data-ttu-id="50ce2-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="50ce2-109">Return Type</span></span>    |<span data-ttu-id="50ce2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="50ce2-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="50ce2-111">Получение объекта TableColumn</span><span class="sxs-lookup"><span data-stu-id="50ce2-111">Get TableColumn</span></span>](../api/tablecolumn-get.md) | [<span data-ttu-id="50ce2-112">TableColumn</span><span class="sxs-lookup"><span data-stu-id="50ce2-112">TableColumn</span></span>](tablecolumn.md) |<span data-ttu-id="50ce2-113">Чтение свойств и связей объекта tableColumn.</span><span class="sxs-lookup"><span data-stu-id="50ce2-113">Read properties and relationships of tableColumn object.</span></span>|
|[<span data-ttu-id="50ce2-114">Обновление</span><span class="sxs-lookup"><span data-stu-id="50ce2-114">Update</span></span>](../api/tablecolumn-update.md) | [<span data-ttu-id="50ce2-115">TableColumn</span><span class="sxs-lookup"><span data-stu-id="50ce2-115">TableColumn</span></span>](tablecolumn.md) |<span data-ttu-id="50ce2-116">Обновление объекта TableColumn.</span><span class="sxs-lookup"><span data-stu-id="50ce2-116">Update TableColumn object.</span></span> |
|[<span data-ttu-id="50ce2-117">Databodyrange</span><span class="sxs-lookup"><span data-stu-id="50ce2-117">Databodyrange</span></span>](../api/tablecolumn-databodyrange.md)|[<span data-ttu-id="50ce2-118">Range</span><span class="sxs-lookup"><span data-stu-id="50ce2-118">Range</span></span>](range.md)|<span data-ttu-id="50ce2-119">Получает объект диапазона, связанный с основными данными столбца.</span><span class="sxs-lookup"><span data-stu-id="50ce2-119">Gets the range object associated with the data body of the column.</span></span>|
|[<span data-ttu-id="50ce2-120">Headerrowrange</span><span class="sxs-lookup"><span data-stu-id="50ce2-120">Headerrowrange</span></span>](../api/tablecolumn-headerrowrange.md)|[<span data-ttu-id="50ce2-121">Range</span><span class="sxs-lookup"><span data-stu-id="50ce2-121">Range</span></span>](range.md)|<span data-ttu-id="50ce2-122">Получает объект диапазона, связанный со строкой заголовков столбца.</span><span class="sxs-lookup"><span data-stu-id="50ce2-122">Gets the range object associated with the header row of the column.</span></span>|
|[<span data-ttu-id="50ce2-123">Range</span><span class="sxs-lookup"><span data-stu-id="50ce2-123">Range</span></span>](../api/tablecolumn-range.md)|[<span data-ttu-id="50ce2-124">Range</span><span class="sxs-lookup"><span data-stu-id="50ce2-124">Range</span></span>](range.md)|<span data-ttu-id="50ce2-125">Получает объект диапазона, связанный со всем столбцом.</span><span class="sxs-lookup"><span data-stu-id="50ce2-125">Gets the range object associated with the entire column.</span></span>|
|[<span data-ttu-id="50ce2-126">Totalrowrange</span><span class="sxs-lookup"><span data-stu-id="50ce2-126">Totalrowrange</span></span>](../api/tablecolumn-totalrowrange.md)|[<span data-ttu-id="50ce2-127">Range</span><span class="sxs-lookup"><span data-stu-id="50ce2-127">Range</span></span>](range.md)|<span data-ttu-id="50ce2-128">Получает объект диапазона, связанный со строкой итогов столбца.</span><span class="sxs-lookup"><span data-stu-id="50ce2-128">Gets the range object associated with the totals row of the column.</span></span>|
|[<span data-ttu-id="50ce2-129">Delete</span><span class="sxs-lookup"><span data-stu-id="50ce2-129">Delete</span></span>](../api/tablecolumn-delete.md)|<span data-ttu-id="50ce2-130">Нет</span><span class="sxs-lookup"><span data-stu-id="50ce2-130">None</span></span>|<span data-ttu-id="50ce2-131">Удаляет столбец из таблицы.</span><span class="sxs-lookup"><span data-stu-id="50ce2-131">Deletes the column from the table.</span></span>|
|[<span data-ttu-id="50ce2-132">Список</span><span class="sxs-lookup"><span data-stu-id="50ce2-132">List</span></span>](../api/tablecolumn-list.md) | <span data-ttu-id="50ce2-133">Коллекция объектов [TableColumn](tablecolumn.md)</span><span class="sxs-lookup"><span data-stu-id="50ce2-133">[TableColumn](tablecolumn.md) collection</span></span> |<span data-ttu-id="50ce2-134">Получение коллекции объектов tableColumn.</span><span class="sxs-lookup"><span data-stu-id="50ce2-134">Get tableColumn object collection.</span></span> |
|[<span data-ttu-id="50ce2-135">Itemat</span><span class="sxs-lookup"><span data-stu-id="50ce2-135">Itemat</span></span>](../api/tablecolumncollection-itemat.md)|[<span data-ttu-id="50ce2-136">TableColumn</span><span class="sxs-lookup"><span data-stu-id="50ce2-136">TableColumn</span></span>](tablecolumn.md)|<span data-ttu-id="50ce2-137">Возвращает столбец на основании его позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="50ce2-137">Gets a column based on its position in the collection.</span></span>|
|[<span data-ttu-id="50ce2-138">Add</span><span class="sxs-lookup"><span data-stu-id="50ce2-138">Add</span></span>](../api/tablecolumncollection-add.md)|[<span data-ttu-id="50ce2-139">TableColumn</span><span class="sxs-lookup"><span data-stu-id="50ce2-139">TableColumn</span></span>](tablecolumn.md)|<span data-ttu-id="50ce2-140">Добавляет новый столбец в таблицу.</span><span class="sxs-lookup"><span data-stu-id="50ce2-140">Adds a new column to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="50ce2-141">Свойства</span><span class="sxs-lookup"><span data-stu-id="50ce2-141">Properties</span></span>
| <span data-ttu-id="50ce2-142">Свойство</span><span class="sxs-lookup"><span data-stu-id="50ce2-142">Property</span></span>     | <span data-ttu-id="50ce2-143">Тип</span><span class="sxs-lookup"><span data-stu-id="50ce2-143">Type</span></span>   |<span data-ttu-id="50ce2-144">Описание</span><span class="sxs-lookup"><span data-stu-id="50ce2-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50ce2-145">id</span><span class="sxs-lookup"><span data-stu-id="50ce2-145">id</span></span>|<span data-ttu-id="50ce2-146">int</span><span class="sxs-lookup"><span data-stu-id="50ce2-146">int</span></span>|<span data-ttu-id="50ce2-p102">Возвращает уникальный ключ, идентифицирующий столбец в таблице. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="50ce2-p102">Returns a unique key that identifies the column within the table. Read-only.</span></span>|
|<span data-ttu-id="50ce2-149">index</span><span class="sxs-lookup"><span data-stu-id="50ce2-149">index</span></span>|<span data-ttu-id="50ce2-150">int</span><span class="sxs-lookup"><span data-stu-id="50ce2-150">int</span></span>|<span data-ttu-id="50ce2-p103">Возвращает номер индекса столбца в коллекции столбцов таблицы. Используется нулевой индекс. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="50ce2-p103">Returns the index number of the column within the columns collection of the table. Zero-indexed. Read-only.</span></span>|
|<span data-ttu-id="50ce2-154">name</span><span class="sxs-lookup"><span data-stu-id="50ce2-154">name</span></span>|<span data-ttu-id="50ce2-155">строка</span><span class="sxs-lookup"><span data-stu-id="50ce2-155">string</span></span>|<span data-ttu-id="50ce2-p104">Возвращает имя столбца таблицы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="50ce2-p104">Returns the name of the table column. Read-only.</span></span>|
|<span data-ttu-id="50ce2-158">values</span><span class="sxs-lookup"><span data-stu-id="50ce2-158">values</span></span>|<span data-ttu-id="50ce2-159">json</span><span class="sxs-lookup"><span data-stu-id="50ce2-159">json</span></span>|<span data-ttu-id="50ce2-p105">Представляет необработанные значения указанного диапазона. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.</span><span class="sxs-lookup"><span data-stu-id="50ce2-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="relationships"></a><span data-ttu-id="50ce2-163">Связи</span><span class="sxs-lookup"><span data-stu-id="50ce2-163">Relationships</span></span>
| <span data-ttu-id="50ce2-164">Связь</span><span class="sxs-lookup"><span data-stu-id="50ce2-164">Relationship</span></span> | <span data-ttu-id="50ce2-165">Тип</span><span class="sxs-lookup"><span data-stu-id="50ce2-165">Type</span></span>   |<span data-ttu-id="50ce2-166">Описание</span><span class="sxs-lookup"><span data-stu-id="50ce2-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50ce2-167">filter</span><span class="sxs-lookup"><span data-stu-id="50ce2-167">filter</span></span>|[<span data-ttu-id="50ce2-168">Filter</span><span class="sxs-lookup"><span data-stu-id="50ce2-168">Filter</span></span>](filter.md)|<span data-ttu-id="50ce2-p106">Возвращает фильтр, применяемый к столбцу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="50ce2-p106">Retrieve the filter applied to the column. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="50ce2-171">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="50ce2-171">JSON representation</span></span>

<span data-ttu-id="50ce2-172">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50ce2-172">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tableColumn"
}-->

```json
{
  "id": 1024,
  "index": 1024,
  "name": "string",
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
