---
title: Тип ресурса NamedItem
description: Представляет определенное имя для диапазона ячеек или значения. Имена могут быть простыми именованными объектами (как показано ниже в столбце "Тип"), объектом диапазона и ссылкой на диапазон. Этот объект может использоваться для получения объекта диапазона, связанного с именами.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b53b223a3f9d894f8ab140014528c0cd02c224dc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036003"
---
# <a name="nameditem-resource-type"></a><span data-ttu-id="b0490-105">Тип ресурса NamedItem</span><span class="sxs-lookup"><span data-stu-id="b0490-105">NamedItem resource type</span></span>

<span data-ttu-id="b0490-p102">Представляет определенное имя для диапазона ячеек или значения. Имена могут быть простыми именованными объектами (как показано ниже в столбце "Тип"), объектом диапазона и ссылкой на диапазон. Этот объект может использоваться для получения объекта диапазона, связанного с именами.</span><span class="sxs-lookup"><span data-stu-id="b0490-p102">Represents a defined name for a range of cells or value. Names can be primitive named objects (as seen in the type below), range object, reference to a range. This object can be used to obtain range object associated with names.</span></span>


## <a name="methods"></a><span data-ttu-id="b0490-109">Методы</span><span class="sxs-lookup"><span data-stu-id="b0490-109">Methods</span></span>

| <span data-ttu-id="b0490-110">Метод</span><span class="sxs-lookup"><span data-stu-id="b0490-110">Method</span></span>           | <span data-ttu-id="b0490-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b0490-111">Return Type</span></span>    |<span data-ttu-id="b0490-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b0490-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b0490-113">Add</span><span class="sxs-lookup"><span data-stu-id="b0490-113">Add</span></span>](../api/nameditem-add.md)|[<span data-ttu-id="b0490-114">Воркбукнамедитем</span><span class="sxs-lookup"><span data-stu-id="b0490-114">WorkbookNamedItem</span></span>](nameditem.md)|<span data-ttu-id="b0490-115">Добавляет новое имя в определенную коллекцию.</span><span class="sxs-lookup"><span data-stu-id="b0490-115">Adds a new name to the collection of the given scope.</span></span>|
|[<span data-ttu-id="b0490-116">AddFormulaLocal</span><span class="sxs-lookup"><span data-stu-id="b0490-116">AddFormulaLocal</span></span>](../api/nameditem-addformulalocal.md)|[<span data-ttu-id="b0490-117">Воркбукнамедитем</span><span class="sxs-lookup"><span data-stu-id="b0490-117">WorkbookNamedItem</span></span>](nameditem.md)|<span data-ttu-id="b0490-118">Добавляет новое имя в определенную коллекцию, используя языковой стандарт пользователя для формулы.</span><span class="sxs-lookup"><span data-stu-id="b0490-118">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>|
|[<span data-ttu-id="b0490-119">Get NamedItem</span><span class="sxs-lookup"><span data-stu-id="b0490-119">Get NamedItem</span></span>](../api/nameditem-get.md) | [<span data-ttu-id="b0490-120">Воркбукнамедитем</span><span class="sxs-lookup"><span data-stu-id="b0490-120">WorkbookNamedItem</span></span>](nameditem.md) |<span data-ttu-id="b0490-121">Чтение свойств и связей объекта namedItem.</span><span class="sxs-lookup"><span data-stu-id="b0490-121">Read properties and relationships of namedItem object.</span></span>|
|[<span data-ttu-id="b0490-122">Обновление</span><span class="sxs-lookup"><span data-stu-id="b0490-122">Update</span></span>](../api/nameditem-update.md) | [<span data-ttu-id="b0490-123">Воркбукнамедитем</span><span class="sxs-lookup"><span data-stu-id="b0490-123">WorkbookNamedItem</span></span>](nameditem.md)   |<span data-ttu-id="b0490-124">Обновление объекта NamedItem.</span><span class="sxs-lookup"><span data-stu-id="b0490-124">Update NamedItem object.</span></span> |
|[<span data-ttu-id="b0490-125">Range</span><span class="sxs-lookup"><span data-stu-id="b0490-125">Range</span></span>](../api/nameditem-range.md)|[<span data-ttu-id="b0490-126">Range</span><span class="sxs-lookup"><span data-stu-id="b0490-126">Range</span></span>](range.md)|<span data-ttu-id="b0490-p103">Возвращает объект Range, сопоставленный с именем. Вызывает исключение, если тип именованного элемента не является диапазоном.</span><span class="sxs-lookup"><span data-stu-id="b0490-p103">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>|
|[<span data-ttu-id="b0490-129">Список</span><span class="sxs-lookup"><span data-stu-id="b0490-129">List</span></span>](../api/nameditem-list.md) | <span data-ttu-id="b0490-130">Коллекция [WorkbookNamedItem](nameditem.md)</span><span class="sxs-lookup"><span data-stu-id="b0490-130">[WorkbookNamedItem](nameditem.md) collection</span></span> |<span data-ttu-id="b0490-131">Получение коллекции объектов namedItem.</span><span class="sxs-lookup"><span data-stu-id="b0490-131">Get namedItem object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="b0490-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="b0490-132">Properties</span></span>
| <span data-ttu-id="b0490-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0490-133">Property</span></span>     | <span data-ttu-id="b0490-134">Тип</span><span class="sxs-lookup"><span data-stu-id="b0490-134">Type</span></span>   |<span data-ttu-id="b0490-135">Описание</span><span class="sxs-lookup"><span data-stu-id="b0490-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0490-136">name</span><span class="sxs-lookup"><span data-stu-id="b0490-136">name</span></span>|<span data-ttu-id="b0490-137">string</span><span class="sxs-lookup"><span data-stu-id="b0490-137">string</span></span>|<span data-ttu-id="b0490-p104">Имя объекта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b0490-p104">The name of the object. Read-only.</span></span>|
|<span data-ttu-id="b0490-140">comment</span><span class="sxs-lookup"><span data-stu-id="b0490-140">comment</span></span>|<span data-ttu-id="b0490-141">строка</span><span class="sxs-lookup"><span data-stu-id="b0490-141">string</span></span>|<span data-ttu-id="b0490-142">Представляет примечание, связанное с этим именем.</span><span class="sxs-lookup"><span data-stu-id="b0490-142">Represents the comment associated with this name.</span></span>|
|<span data-ttu-id="b0490-143">scope</span><span class="sxs-lookup"><span data-stu-id="b0490-143">scope</span></span>|<span data-ttu-id="b0490-144">string</span><span class="sxs-lookup"><span data-stu-id="b0490-144">string</span></span>|<span data-ttu-id="b0490-p105">Указывает, относится ли имя к книге или определенному листу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b0490-p105">Indicates whether the name is scoped to the workbook or to a specific worksheet. Read-only.</span></span>|
|<span data-ttu-id="b0490-147">type</span><span class="sxs-lookup"><span data-stu-id="b0490-147">type</span></span>|<span data-ttu-id="b0490-148">string</span><span class="sxs-lookup"><span data-stu-id="b0490-148">string</span></span>|<span data-ttu-id="b0490-149">Указывает тип ссылки, связанный с именем.</span><span class="sxs-lookup"><span data-stu-id="b0490-149">Indicates what type of reference is associated with the name.</span></span> <span data-ttu-id="b0490-150">Допустимые значения: `String`, `Integer`, `Double`, `Boolean`, `Range`.</span><span class="sxs-lookup"><span data-stu-id="b0490-150">The possible values are: `String`, `Integer`, `Double`, `Boolean`, `Range`.</span></span> <span data-ttu-id="b0490-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b0490-151">Read-only.</span></span>|
|<span data-ttu-id="b0490-152">value</span><span class="sxs-lookup"><span data-stu-id="b0490-152">value</span></span>|<span data-ttu-id="b0490-153">Json</span><span class="sxs-lookup"><span data-stu-id="b0490-153">Json</span></span>|<span data-ttu-id="b0490-p107">Представляет формулу, на которую ссылается имя. Например, =Sheet14!$B$2:$H$12, =4,75 и т. д. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b0490-p107">Represents the formula that the name is defined to refer to. E.g. =Sheet14!$B$2:$H$12, =4.75, etc. Read-only.</span></span>|
|<span data-ttu-id="b0490-157">visible</span><span class="sxs-lookup"><span data-stu-id="b0490-157">visible</span></span>|<span data-ttu-id="b0490-158">boolean</span><span class="sxs-lookup"><span data-stu-id="b0490-158">boolean</span></span>|<span data-ttu-id="b0490-159">Определяет, является ли объект видимым.</span><span class="sxs-lookup"><span data-stu-id="b0490-159">Specifies whether the object is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0490-160">Отношения</span><span class="sxs-lookup"><span data-stu-id="b0490-160">Relationships</span></span>
| <span data-ttu-id="b0490-161">Отношение</span><span class="sxs-lookup"><span data-stu-id="b0490-161">Relationship</span></span>     | <span data-ttu-id="b0490-162">Тип</span><span class="sxs-lookup"><span data-stu-id="b0490-162">Type</span></span>   |<span data-ttu-id="b0490-163">Описание</span><span class="sxs-lookup"><span data-stu-id="b0490-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0490-164">worksheet</span><span class="sxs-lookup"><span data-stu-id="b0490-164">worksheet</span></span>|[<span data-ttu-id="b0490-165">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="b0490-165">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="b0490-p108">Возвращает лист, к которому относится именованный элемент. Доступно, только если элемент относится к листу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b0490-p108">Returns the worksheet on which the named item is scoped to. Available only if the item is scoped to the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b0490-169">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b0490-169">JSON representation</span></span>

<span data-ttu-id="b0490-170">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0490-170">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookNamedItem"
}-->

```json
{
  "name": "string",
  "comment": "string",
  "scope": "string",
  "type": "string",
  "value": {"@odata.type": "microsoft.graph.Json"},
  "visible": true
  
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
