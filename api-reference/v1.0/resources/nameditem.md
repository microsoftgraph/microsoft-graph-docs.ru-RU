---
title: Тип ресурса NamedItem
description: Представляет определенное имя для диапазона ячеек или значения. Имена могут быть простыми именованными объектами (как показано ниже в столбце "Тип"), объектом диапазона и ссылкой на диапазон. Этот объект может использоваться для получения объекта диапазона, связанного с именами.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0aece739f4a65db35271e4fe6f2c87db3a2c56a5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534206"
---
# <a name="nameditem-resource-type"></a><span data-ttu-id="70aa5-105">Тип ресурса NamedItem</span><span class="sxs-lookup"><span data-stu-id="70aa5-105">NamedItem resource type</span></span>

<span data-ttu-id="70aa5-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70aa5-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="70aa5-p102">Представляет определенное имя для диапазона ячеек или значения. Имена могут быть простыми именованными объектами (как показано ниже в столбце "Тип"), объектом диапазона и ссылкой на диапазон. Этот объект может использоваться для получения объекта диапазона, связанного с именами.</span><span class="sxs-lookup"><span data-stu-id="70aa5-p102">Represents a defined name for a range of cells or value. Names can be primitive named objects (as seen in the type below), range object, reference to a range. This object can be used to obtain range object associated with names.</span></span>


## <a name="methods"></a><span data-ttu-id="70aa5-110">Методы</span><span class="sxs-lookup"><span data-stu-id="70aa5-110">Methods</span></span>

| <span data-ttu-id="70aa5-111">Метод</span><span class="sxs-lookup"><span data-stu-id="70aa5-111">Method</span></span>           | <span data-ttu-id="70aa5-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="70aa5-112">Return Type</span></span>    |<span data-ttu-id="70aa5-113">Описание</span><span class="sxs-lookup"><span data-stu-id="70aa5-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="70aa5-114">Add</span><span class="sxs-lookup"><span data-stu-id="70aa5-114">Add</span></span>](../api/nameditem-add.md)|[<span data-ttu-id="70aa5-115">воркбукнамедитем</span><span class="sxs-lookup"><span data-stu-id="70aa5-115">WorkbookNamedItem</span></span>](nameditem.md)|<span data-ttu-id="70aa5-116">Добавляет новое имя в определенную коллекцию.</span><span class="sxs-lookup"><span data-stu-id="70aa5-116">Adds a new name to the collection of the given scope.</span></span>|
|[<span data-ttu-id="70aa5-117">AddFormulaLocal</span><span class="sxs-lookup"><span data-stu-id="70aa5-117">AddFormulaLocal</span></span>](../api/nameditem-addformulalocal.md)|[<span data-ttu-id="70aa5-118">воркбукнамедитем</span><span class="sxs-lookup"><span data-stu-id="70aa5-118">WorkbookNamedItem</span></span>](nameditem.md)|<span data-ttu-id="70aa5-119">Добавляет новое имя в определенную коллекцию, используя языковой стандарт пользователя для формулы.</span><span class="sxs-lookup"><span data-stu-id="70aa5-119">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>|
|[<span data-ttu-id="70aa5-120">Get NamedItem</span><span class="sxs-lookup"><span data-stu-id="70aa5-120">Get NamedItem</span></span>](../api/nameditem-get.md) | [<span data-ttu-id="70aa5-121">воркбукнамедитем</span><span class="sxs-lookup"><span data-stu-id="70aa5-121">WorkbookNamedItem</span></span>](nameditem.md) |<span data-ttu-id="70aa5-122">Чтение свойств и связей объекта namedItem.</span><span class="sxs-lookup"><span data-stu-id="70aa5-122">Read properties and relationships of namedItem object.</span></span>|
|[<span data-ttu-id="70aa5-123">Обновление</span><span class="sxs-lookup"><span data-stu-id="70aa5-123">Update</span></span>](../api/nameditem-update.md) | [<span data-ttu-id="70aa5-124">воркбукнамедитем</span><span class="sxs-lookup"><span data-stu-id="70aa5-124">WorkbookNamedItem</span></span>](nameditem.md)   |<span data-ttu-id="70aa5-125">Обновление объекта NamedItem.</span><span class="sxs-lookup"><span data-stu-id="70aa5-125">Update NamedItem object.</span></span> |
|[<span data-ttu-id="70aa5-126">Range</span><span class="sxs-lookup"><span data-stu-id="70aa5-126">Range</span></span>](../api/nameditem-range.md)|[<span data-ttu-id="70aa5-127">Range</span><span class="sxs-lookup"><span data-stu-id="70aa5-127">Range</span></span>](range.md)|<span data-ttu-id="70aa5-p103">Возвращает объект Range, сопоставленный с именем. Вызывает исключение, если тип именованного элемента не является диапазоном.</span><span class="sxs-lookup"><span data-stu-id="70aa5-p103">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>|
|[<span data-ttu-id="70aa5-130">Список</span><span class="sxs-lookup"><span data-stu-id="70aa5-130">List</span></span>](../api/nameditem-list.md) | <span data-ttu-id="70aa5-131">Коллекция [WorkbookNamedItem](nameditem.md)</span><span class="sxs-lookup"><span data-stu-id="70aa5-131">[WorkbookNamedItem](nameditem.md) collection</span></span> |<span data-ttu-id="70aa5-132">Получение коллекции объектов namedItem.</span><span class="sxs-lookup"><span data-stu-id="70aa5-132">Get namedItem object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="70aa5-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="70aa5-133">Properties</span></span>
| <span data-ttu-id="70aa5-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="70aa5-134">Property</span></span>     | <span data-ttu-id="70aa5-135">Тип</span><span class="sxs-lookup"><span data-stu-id="70aa5-135">Type</span></span>   |<span data-ttu-id="70aa5-136">Описание</span><span class="sxs-lookup"><span data-stu-id="70aa5-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70aa5-137">name</span><span class="sxs-lookup"><span data-stu-id="70aa5-137">name</span></span>|<span data-ttu-id="70aa5-138">string</span><span class="sxs-lookup"><span data-stu-id="70aa5-138">string</span></span>|<span data-ttu-id="70aa5-p104">Имя объекта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="70aa5-p104">The name of the object. Read-only.</span></span>|
|<span data-ttu-id="70aa5-141">comment</span><span class="sxs-lookup"><span data-stu-id="70aa5-141">comment</span></span>|<span data-ttu-id="70aa5-142">строка</span><span class="sxs-lookup"><span data-stu-id="70aa5-142">string</span></span>|<span data-ttu-id="70aa5-143">Представляет примечание, связанное с этим именем.</span><span class="sxs-lookup"><span data-stu-id="70aa5-143">Represents the comment associated with this name.</span></span>|
|<span data-ttu-id="70aa5-144">scope</span><span class="sxs-lookup"><span data-stu-id="70aa5-144">scope</span></span>|<span data-ttu-id="70aa5-145">string</span><span class="sxs-lookup"><span data-stu-id="70aa5-145">string</span></span>|<span data-ttu-id="70aa5-p105">Указывает, относится ли имя к книге или определенному листу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="70aa5-p105">Indicates whether the name is scoped to the workbook or to a specific worksheet. Read-only.</span></span>|
|<span data-ttu-id="70aa5-148">type</span><span class="sxs-lookup"><span data-stu-id="70aa5-148">type</span></span>|<span data-ttu-id="70aa5-149">string</span><span class="sxs-lookup"><span data-stu-id="70aa5-149">string</span></span>|<span data-ttu-id="70aa5-150">Указывает тип ссылки, связанный с именем.</span><span class="sxs-lookup"><span data-stu-id="70aa5-150">Indicates what type of reference is associated with the name.</span></span> <span data-ttu-id="70aa5-151">Допустимые значения: `String`, `Integer`, `Double`, `Boolean`, `Range`.</span><span class="sxs-lookup"><span data-stu-id="70aa5-151">The possible values are: `String`, `Integer`, `Double`, `Boolean`, `Range`.</span></span> <span data-ttu-id="70aa5-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="70aa5-152">Read-only.</span></span>|
|<span data-ttu-id="70aa5-153">value</span><span class="sxs-lookup"><span data-stu-id="70aa5-153">value</span></span>|<span data-ttu-id="70aa5-154">Json</span><span class="sxs-lookup"><span data-stu-id="70aa5-154">Json</span></span>|<span data-ttu-id="70aa5-p107">Представляет формулу, на которую ссылается имя. Например, =Sheet14!$B$2:$H$12, =4,75 и т. д. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="70aa5-p107">Represents the formula that the name is defined to refer to. E.g. =Sheet14!$B$2:$H$12, =4.75, etc. Read-only.</span></span>|
|<span data-ttu-id="70aa5-158">visible</span><span class="sxs-lookup"><span data-stu-id="70aa5-158">visible</span></span>|<span data-ttu-id="70aa5-159">boolean</span><span class="sxs-lookup"><span data-stu-id="70aa5-159">boolean</span></span>|<span data-ttu-id="70aa5-160">Определяет, является ли объект видимым.</span><span class="sxs-lookup"><span data-stu-id="70aa5-160">Specifies whether the object is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="70aa5-161">Связи</span><span class="sxs-lookup"><span data-stu-id="70aa5-161">Relationships</span></span>
| <span data-ttu-id="70aa5-162">Связь</span><span class="sxs-lookup"><span data-stu-id="70aa5-162">Relationship</span></span>     | <span data-ttu-id="70aa5-163">Тип</span><span class="sxs-lookup"><span data-stu-id="70aa5-163">Type</span></span>   |<span data-ttu-id="70aa5-164">Описание</span><span class="sxs-lookup"><span data-stu-id="70aa5-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70aa5-165">worksheet</span><span class="sxs-lookup"><span data-stu-id="70aa5-165">worksheet</span></span>|[<span data-ttu-id="70aa5-166">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="70aa5-166">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="70aa5-p108">Возвращает лист, к которому относится именованный элемент. Доступно, только если элемент относится к листу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="70aa5-p108">Returns the worksheet on which the named item is scoped to. Available only if the item is scoped to the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="70aa5-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="70aa5-170">JSON representation</span></span>

<span data-ttu-id="70aa5-171">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="70aa5-171">Here is a JSON representation of the resource.</span></span>

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
