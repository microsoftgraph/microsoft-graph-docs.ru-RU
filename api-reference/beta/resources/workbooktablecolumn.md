---
title: Тип ресурса Воркбуктаблеколумн
description: Представляет столбец в таблице.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 32ebcbb4b4d0c8721b5cd1d1a421edb37d836821
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519129"
---
# <a name="workbooktablecolumn-resource-type"></a><span data-ttu-id="ff606-103">Тип ресурса Воркбуктаблеколумн</span><span class="sxs-lookup"><span data-stu-id="ff606-103">workbookTableColumn resource type</span></span>

<span data-ttu-id="ff606-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ff606-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff606-105">Представляет столбец в таблице.</span><span class="sxs-lookup"><span data-stu-id="ff606-105">Represents a column in a table.</span></span>


## <a name="methods"></a><span data-ttu-id="ff606-106">Методы</span><span class="sxs-lookup"><span data-stu-id="ff606-106">Methods</span></span>

| <span data-ttu-id="ff606-107">Метод</span><span class="sxs-lookup"><span data-stu-id="ff606-107">Method</span></span>           | <span data-ttu-id="ff606-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ff606-108">Return Type</span></span>    |<span data-ttu-id="ff606-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ff606-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ff606-110">Получение объекта TableColumn</span><span class="sxs-lookup"><span data-stu-id="ff606-110">Get TableColumn</span></span>](../api/tablecolumn-get.md) | [<span data-ttu-id="ff606-111">воркбуктаблеколумн</span><span class="sxs-lookup"><span data-stu-id="ff606-111">workbookTableColumn</span></span>](workbooktablecolumn.md) |<span data-ttu-id="ff606-112">Чтение свойств и связей объекта tableColumn.</span><span class="sxs-lookup"><span data-stu-id="ff606-112">Read properties and relationships of tableColumn object.</span></span>|
|[<span data-ttu-id="ff606-113">Обновление</span><span class="sxs-lookup"><span data-stu-id="ff606-113">Update</span></span>](../api/tablecolumn-update.md) | [<span data-ttu-id="ff606-114">воркбуктаблеколумн</span><span class="sxs-lookup"><span data-stu-id="ff606-114">workbookTableColumn</span></span>](workbooktablecolumn.md) |<span data-ttu-id="ff606-115">Обновление объекта TableColumn.</span><span class="sxs-lookup"><span data-stu-id="ff606-115">Update TableColumn object.</span></span> |
|[<span data-ttu-id="ff606-116">Databodyrange</span><span class="sxs-lookup"><span data-stu-id="ff606-116">Databodyrange</span></span>](../api/tablecolumn-databodyrange.md)|[<span data-ttu-id="ff606-117">workbookRange</span><span class="sxs-lookup"><span data-stu-id="ff606-117">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="ff606-118">Получает объект диапазона, связанный с основными данными столбца.</span><span class="sxs-lookup"><span data-stu-id="ff606-118">Gets the range object associated with the data body of the column.</span></span>|
|[<span data-ttu-id="ff606-119">Headerrowrange</span><span class="sxs-lookup"><span data-stu-id="ff606-119">Headerrowrange</span></span>](../api/tablecolumn-headerrowrange.md)|[<span data-ttu-id="ff606-120">workbookRange</span><span class="sxs-lookup"><span data-stu-id="ff606-120">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="ff606-121">Получает объект диапазона, связанный со строкой заголовков столбца.</span><span class="sxs-lookup"><span data-stu-id="ff606-121">Gets the range object associated with the header row of the column.</span></span>|
|[<span data-ttu-id="ff606-122">Range</span><span class="sxs-lookup"><span data-stu-id="ff606-122">Range</span></span>](../api/tablecolumn-range.md)|[<span data-ttu-id="ff606-123">workbookRange</span><span class="sxs-lookup"><span data-stu-id="ff606-123">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="ff606-124">Получает объект диапазона, связанный со всем столбцом.</span><span class="sxs-lookup"><span data-stu-id="ff606-124">Gets the range object associated with the entire column.</span></span>|
|[<span data-ttu-id="ff606-125">Totalrowrange</span><span class="sxs-lookup"><span data-stu-id="ff606-125">Totalrowrange</span></span>](../api/tablecolumn-totalrowrange.md)|[<span data-ttu-id="ff606-126">workbookRange</span><span class="sxs-lookup"><span data-stu-id="ff606-126">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="ff606-127">Получает объект диапазона, связанный со строкой итогов столбца.</span><span class="sxs-lookup"><span data-stu-id="ff606-127">Gets the range object associated with the totals row of the column.</span></span>|
|<span data-ttu-id="ff606-128">[удаление](../api/tablecolumn-delete.md);</span><span class="sxs-lookup"><span data-stu-id="ff606-128">[Delete](../api/tablecolumn-delete.md)</span></span>|<span data-ttu-id="ff606-129">Нет</span><span class="sxs-lookup"><span data-stu-id="ff606-129">None</span></span>|<span data-ttu-id="ff606-130">Удаляет столбец из таблицы.</span><span class="sxs-lookup"><span data-stu-id="ff606-130">Deletes the column from the table.</span></span>|
|[<span data-ttu-id="ff606-131">Список</span><span class="sxs-lookup"><span data-stu-id="ff606-131">List</span></span>](../api/tablecolumn-list.md) | <span data-ttu-id="ff606-132">Коллекция [воркбуктаблеколумн](workbooktablecolumn.md)</span><span class="sxs-lookup"><span data-stu-id="ff606-132">[workbookTableColumn](workbooktablecolumn.md) collection</span></span> |<span data-ttu-id="ff606-133">Получение коллекции объектов tableColumn.</span><span class="sxs-lookup"><span data-stu-id="ff606-133">Get tableColumn object collection.</span></span> |
|[<span data-ttu-id="ff606-134">Itemat</span><span class="sxs-lookup"><span data-stu-id="ff606-134">Itemat</span></span>](../api/tablecolumncollection-itemat.md)|[<span data-ttu-id="ff606-135">воркбуктаблеколумн</span><span class="sxs-lookup"><span data-stu-id="ff606-135">workbookTableColumn</span></span>](workbooktablecolumn.md)|<span data-ttu-id="ff606-136">Возвращает столбец на основании его позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="ff606-136">Gets a column based on its position in the collection.</span></span>|
|[<span data-ttu-id="ff606-137">Add</span><span class="sxs-lookup"><span data-stu-id="ff606-137">Add</span></span>](../api/tablecolumncollection-add.md)|[<span data-ttu-id="ff606-138">воркбуктаблеколумн</span><span class="sxs-lookup"><span data-stu-id="ff606-138">workbookTableColumn</span></span>](workbooktablecolumn.md)|<span data-ttu-id="ff606-139">Добавляет новый столбец в таблицу.</span><span class="sxs-lookup"><span data-stu-id="ff606-139">Adds a new column to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="ff606-140">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff606-140">Properties</span></span>
| <span data-ttu-id="ff606-141">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff606-141">Property</span></span>     | <span data-ttu-id="ff606-142">Тип</span><span class="sxs-lookup"><span data-stu-id="ff606-142">Type</span></span>   |<span data-ttu-id="ff606-143">Описание</span><span class="sxs-lookup"><span data-stu-id="ff606-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff606-144">id</span><span class="sxs-lookup"><span data-stu-id="ff606-144">id</span></span>|<span data-ttu-id="ff606-145">int</span><span class="sxs-lookup"><span data-stu-id="ff606-145">int</span></span>|<span data-ttu-id="ff606-p101">Возвращает уникальный ключ, идентифицирующий столбец в таблице. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff606-p101">Returns a unique key that identifies the column within the table. Read-only.</span></span>|
|<span data-ttu-id="ff606-148">index</span><span class="sxs-lookup"><span data-stu-id="ff606-148">index</span></span>|<span data-ttu-id="ff606-149">int</span><span class="sxs-lookup"><span data-stu-id="ff606-149">int</span></span>|<span data-ttu-id="ff606-p102">Возвращает номер индекса столбца в коллекции столбцов таблицы. Используется нулевой индекс. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff606-p102">Returns the index number of the column within the columns collection of the table. Zero-indexed. Read-only.</span></span>|
|<span data-ttu-id="ff606-153">name</span><span class="sxs-lookup"><span data-stu-id="ff606-153">name</span></span>|<span data-ttu-id="ff606-154">string</span><span class="sxs-lookup"><span data-stu-id="ff606-154">string</span></span>|<span data-ttu-id="ff606-155">Возвращает имя столбца таблицы.</span><span class="sxs-lookup"><span data-stu-id="ff606-155">Returns the name of the table column.</span></span>|
|<span data-ttu-id="ff606-156">values</span><span class="sxs-lookup"><span data-stu-id="ff606-156">values</span></span>|<span data-ttu-id="ff606-157">Json</span><span class="sxs-lookup"><span data-stu-id="ff606-157">Json</span></span>|<span data-ttu-id="ff606-p103">Представляет необработанные значения указанного диапазона. Могут возвращаться строковые и числовые данные, а также логические значения. Ячейка, которая содержит ошибку, вернет строку ошибки.</span><span class="sxs-lookup"><span data-stu-id="ff606-p103">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff606-161">Связи</span><span class="sxs-lookup"><span data-stu-id="ff606-161">Relationships</span></span>
| <span data-ttu-id="ff606-162">Связь</span><span class="sxs-lookup"><span data-stu-id="ff606-162">Relationship</span></span> | <span data-ttu-id="ff606-163">Тип</span><span class="sxs-lookup"><span data-stu-id="ff606-163">Type</span></span>   |<span data-ttu-id="ff606-164">Описание</span><span class="sxs-lookup"><span data-stu-id="ff606-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff606-165">filter</span><span class="sxs-lookup"><span data-stu-id="ff606-165">filter</span></span>|[<span data-ttu-id="ff606-166">воркбукфилтер</span><span class="sxs-lookup"><span data-stu-id="ff606-166">workbookFilter</span></span>](workbookfilter.md)|<span data-ttu-id="ff606-p104">Возвращает фильтр, применяемый к столбцу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff606-p104">Retrieve the filter applied to the column. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ff606-169">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff606-169">JSON representation</span></span>

<span data-ttu-id="ff606-170">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff606-170">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableColumn"
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
<!--
{
  "type": "#page.annotation",
  "description": "TableColumn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
