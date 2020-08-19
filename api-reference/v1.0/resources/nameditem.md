---
title: Тип ресурса NamedItem
description: Представляет определенное имя для диапазона ячеек или значения. Имена могут быть простыми именованными объектами (как показано ниже в столбце "Тип"), объектом диапазона и ссылкой на диапазон. Этот объект может использоваться для получения объекта диапазона, связанного с именами.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3be31cd34f1fe880c079bba50e7e612dfa26da45
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808216"
---
# <a name="nameditem-resource-type"></a><span data-ttu-id="3e6dc-105">Тип ресурса NamedItem</span><span class="sxs-lookup"><span data-stu-id="3e6dc-105">NamedItem resource type</span></span>

<span data-ttu-id="3e6dc-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e6dc-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3e6dc-p102">Представляет определенное имя для диапазона ячеек или значения. Имена могут быть простыми именованными объектами (как показано ниже в столбце "Тип"), объектом диапазона и ссылкой на диапазон. Этот объект может использоваться для получения объекта диапазона, связанного с именами.</span><span class="sxs-lookup"><span data-stu-id="3e6dc-p102">Represents a defined name for a range of cells or value. Names can be primitive named objects (as seen in the type below), range object, reference to a range. This object can be used to obtain range object associated with names.</span></span>


## <a name="methods"></a><span data-ttu-id="3e6dc-110">Методы</span><span class="sxs-lookup"><span data-stu-id="3e6dc-110">Methods</span></span>

| <span data-ttu-id="3e6dc-111">Метод</span><span class="sxs-lookup"><span data-stu-id="3e6dc-111">Method</span></span>           | <span data-ttu-id="3e6dc-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3e6dc-112">Return Type</span></span>    |<span data-ttu-id="3e6dc-113">Описание</span><span class="sxs-lookup"><span data-stu-id="3e6dc-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3e6dc-114">Add</span><span class="sxs-lookup"><span data-stu-id="3e6dc-114">Add</span></span>](../api/nameditem-add.md)|[<span data-ttu-id="3e6dc-115">воркбукнамедитем</span><span class="sxs-lookup"><span data-stu-id="3e6dc-115">WorkbookNamedItem</span></span>](nameditem.md)|<span data-ttu-id="3e6dc-116">Добавляет новое имя в определенную коллекцию.</span><span class="sxs-lookup"><span data-stu-id="3e6dc-116">Adds a new name to the collection of the given scope.</span></span>|
|[<span data-ttu-id="3e6dc-117">AddFormulaLocal</span><span class="sxs-lookup"><span data-stu-id="3e6dc-117">AddFormulaLocal</span></span>](../api/nameditem-addformulalocal.md)|[<span data-ttu-id="3e6dc-118">воркбукнамедитем</span><span class="sxs-lookup"><span data-stu-id="3e6dc-118">WorkbookNamedItem</span></span>](nameditem.md)|<span data-ttu-id="3e6dc-119">Добавляет новое имя в определенную коллекцию, используя языковой стандарт пользователя для формулы.</span><span class="sxs-lookup"><span data-stu-id="3e6dc-119">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>|
|[<span data-ttu-id="3e6dc-120">Get NamedItem</span><span class="sxs-lookup"><span data-stu-id="3e6dc-120">Get NamedItem</span></span>](../api/nameditem-get.md) | [<span data-ttu-id="3e6dc-121">воркбукнамедитем</span><span class="sxs-lookup"><span data-stu-id="3e6dc-121">WorkbookNamedItem</span></span>](nameditem.md) |<span data-ttu-id="3e6dc-122">Чтение свойств и связей объекта namedItem.</span><span class="sxs-lookup"><span data-stu-id="3e6dc-122">Read properties and relationships of namedItem object.</span></span>|
|[<span data-ttu-id="3e6dc-123">Обновление</span><span class="sxs-lookup"><span data-stu-id="3e6dc-123">Update</span></span>](../api/nameditem-update.md) | [<span data-ttu-id="3e6dc-124">воркбукнамедитем</span><span class="sxs-lookup"><span data-stu-id="3e6dc-124">WorkbookNamedItem</span></span>](nameditem.md)   |<span data-ttu-id="3e6dc-125">Обновление объекта NamedItem.</span><span class="sxs-lookup"><span data-stu-id="3e6dc-125">Update NamedItem object.</span></span> |
|[<span data-ttu-id="3e6dc-126">Range</span><span class="sxs-lookup"><span data-stu-id="3e6dc-126">Range</span></span>](../api/nameditem-range.md)|[<span data-ttu-id="3e6dc-127">Range</span><span class="sxs-lookup"><span data-stu-id="3e6dc-127">Range</span></span>](range.md)|<span data-ttu-id="3e6dc-p103">Возвращает объект Range, сопоставленный с именем. Вызывает исключение, если тип именованного элемента не является диапазоном.</span><span class="sxs-lookup"><span data-stu-id="3e6dc-p103">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>|
|[<span data-ttu-id="3e6dc-130">Список</span><span class="sxs-lookup"><span data-stu-id="3e6dc-130">List</span></span>](../api/nameditem-list.md) | <span data-ttu-id="3e6dc-131">Коллекция [WorkbookNamedItem](nameditem.md)</span><span class="sxs-lookup"><span data-stu-id="3e6dc-131">[WorkbookNamedItem](nameditem.md) collection</span></span> |<span data-ttu-id="3e6dc-132">Получение коллекции объектов namedItem.</span><span class="sxs-lookup"><span data-stu-id="3e6dc-132">Get namedItem object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="3e6dc-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="3e6dc-133">Properties</span></span>
| <span data-ttu-id="3e6dc-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e6dc-134">Property</span></span>     | <span data-ttu-id="3e6dc-135">Тип</span><span class="sxs-lookup"><span data-stu-id="3e6dc-135">Type</span></span>   |<span data-ttu-id="3e6dc-136">Описание</span><span class="sxs-lookup"><span data-stu-id="3e6dc-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e6dc-137">name</span><span class="sxs-lookup"><span data-stu-id="3e6dc-137">name</span></span>|<span data-ttu-id="3e6dc-138">string</span><span class="sxs-lookup"><span data-stu-id="3e6dc-138">string</span></span>|<span data-ttu-id="3e6dc-p104">Имя объекта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e6dc-p104">The name of the object. Read-only.</span></span>|
|<span data-ttu-id="3e6dc-141">comment</span><span class="sxs-lookup"><span data-stu-id="3e6dc-141">comment</span></span>|<span data-ttu-id="3e6dc-142">string</span><span class="sxs-lookup"><span data-stu-id="3e6dc-142">string</span></span>|<span data-ttu-id="3e6dc-143">Представляет примечание, связанное с этим именем.</span><span class="sxs-lookup"><span data-stu-id="3e6dc-143">Represents the comment associated with this name.</span></span>|
|<span data-ttu-id="3e6dc-144">scope</span><span class="sxs-lookup"><span data-stu-id="3e6dc-144">scope</span></span>|<span data-ttu-id="3e6dc-145">string</span><span class="sxs-lookup"><span data-stu-id="3e6dc-145">string</span></span>|<span data-ttu-id="3e6dc-p105">Указывает, относится ли имя к книге или определенному листу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e6dc-p105">Indicates whether the name is scoped to the workbook or to a specific worksheet. Read-only.</span></span>|
|<span data-ttu-id="3e6dc-148">type</span><span class="sxs-lookup"><span data-stu-id="3e6dc-148">type</span></span>|<span data-ttu-id="3e6dc-149">string</span><span class="sxs-lookup"><span data-stu-id="3e6dc-149">string</span></span>|<span data-ttu-id="3e6dc-150">Указывает тип ссылки, связанный с именем.</span><span class="sxs-lookup"><span data-stu-id="3e6dc-150">Indicates what type of reference is associated with the name.</span></span> <span data-ttu-id="3e6dc-151">Допустимые значения: `String`, `Integer`, `Double`, `Boolean`, `Range`.</span><span class="sxs-lookup"><span data-stu-id="3e6dc-151">The possible values are: `String`, `Integer`, `Double`, `Boolean`, `Range`.</span></span> <span data-ttu-id="3e6dc-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e6dc-152">Read-only.</span></span>|
|<span data-ttu-id="3e6dc-153">value</span><span class="sxs-lookup"><span data-stu-id="3e6dc-153">value</span></span>|<span data-ttu-id="3e6dc-154">Json</span><span class="sxs-lookup"><span data-stu-id="3e6dc-154">Json</span></span>|<span data-ttu-id="3e6dc-p107">Представляет формулу, на которую ссылается имя. Например, =Sheet14!$B$2:$H$12, =4,75 и т. д. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e6dc-p107">Represents the formula that the name is defined to refer to. E.g. =Sheet14!$B$2:$H$12, =4.75, etc. Read-only.</span></span>|
|<span data-ttu-id="3e6dc-158">visible</span><span class="sxs-lookup"><span data-stu-id="3e6dc-158">visible</span></span>|<span data-ttu-id="3e6dc-159">boolean</span><span class="sxs-lookup"><span data-stu-id="3e6dc-159">boolean</span></span>|<span data-ttu-id="3e6dc-160">Определяет, является ли объект видимым.</span><span class="sxs-lookup"><span data-stu-id="3e6dc-160">Specifies whether the object is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e6dc-161">Отношения</span><span class="sxs-lookup"><span data-stu-id="3e6dc-161">Relationships</span></span>
| <span data-ttu-id="3e6dc-162">Связь</span><span class="sxs-lookup"><span data-stu-id="3e6dc-162">Relationship</span></span>     | <span data-ttu-id="3e6dc-163">Тип</span><span class="sxs-lookup"><span data-stu-id="3e6dc-163">Type</span></span>   |<span data-ttu-id="3e6dc-164">Описание</span><span class="sxs-lookup"><span data-stu-id="3e6dc-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e6dc-165">worksheet</span><span class="sxs-lookup"><span data-stu-id="3e6dc-165">worksheet</span></span>|[<span data-ttu-id="3e6dc-166">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="3e6dc-166">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="3e6dc-p108">Возвращает лист, к которому относится именованный элемент. Доступно, только если элемент относится к листу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e6dc-p108">Returns the worksheet on which the named item is scoped to. Available only if the item is scoped to the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3e6dc-170">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3e6dc-170">JSON representation</span></span>

<span data-ttu-id="3e6dc-171">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e6dc-171">Here is a JSON representation of the resource.</span></span>

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
