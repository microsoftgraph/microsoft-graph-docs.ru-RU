---
title: Тип ресурса Воркбукнамедитем
description: Представляет определенное имя для диапазона ячеек или значения. Имена могут быть простыми именованными объектами (как показано ниже в столбце "Тип"), объектом диапазона и ссылкой на диапазон. Этот объект может использоваться для получения объекта диапазона, связанного с именами.
localization_priority: Normal
ms.openlocfilehash: 49267379385a13b94e8639e4c129c05192b2ae6f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348991"
---
# <a name="workbooknameditem-resource-type"></a><span data-ttu-id="308be-105">Тип ресурса Воркбукнамедитем</span><span class="sxs-lookup"><span data-stu-id="308be-105">workbookNamedItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="308be-p102">Представляет определенное имя для диапазона ячеек или значения. Имена могут быть простыми именованными объектами (как показано ниже в столбце "Тип"), объектом диапазона и ссылкой на диапазон. Этот объект может использоваться для получения объекта диапазона, связанного с именами.</span><span class="sxs-lookup"><span data-stu-id="308be-p102">Represents a defined name for a range of cells or value. Names can be primitive named objects (as seen in the type below), range object, reference to a range. This object can be used to obtain range object associated with names.</span></span>


## <a name="methods"></a><span data-ttu-id="308be-109">Методы</span><span class="sxs-lookup"><span data-stu-id="308be-109">Methods</span></span>

| <span data-ttu-id="308be-110">Метод</span><span class="sxs-lookup"><span data-stu-id="308be-110">Method</span></span>           | <span data-ttu-id="308be-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="308be-111">Return Type</span></span>    |<span data-ttu-id="308be-112">Описание</span><span class="sxs-lookup"><span data-stu-id="308be-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="308be-113">Add</span><span class="sxs-lookup"><span data-stu-id="308be-113">Add</span></span>](../api/nameditem-add.md)|[<span data-ttu-id="308be-114">Воркбукнамедитем</span><span class="sxs-lookup"><span data-stu-id="308be-114">workbookNamedItem</span></span>](workbooknameditem.md)|<span data-ttu-id="308be-115">Добавляет новое имя в определенную коллекцию.</span><span class="sxs-lookup"><span data-stu-id="308be-115">Adds a new name to the collection of the given scope.</span></span>|
|[<span data-ttu-id="308be-116">AddFormulaLocal</span><span class="sxs-lookup"><span data-stu-id="308be-116">AddFormulaLocal</span></span>](../api/nameditem-addformulalocal.md)|[<span data-ttu-id="308be-117">Воркбукнамедитем</span><span class="sxs-lookup"><span data-stu-id="308be-117">workbookNamedItem</span></span>](workbooknameditem.md)|<span data-ttu-id="308be-118">Добавляет новое имя в определенную коллекцию, используя языковой стандарт пользователя для формулы.</span><span class="sxs-lookup"><span data-stu-id="308be-118">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>|
|[<span data-ttu-id="308be-119">Get NamedItem</span><span class="sxs-lookup"><span data-stu-id="308be-119">Get NamedItem</span></span>](../api/nameditem-get.md) | [<span data-ttu-id="308be-120">Воркбукнамедитем</span><span class="sxs-lookup"><span data-stu-id="308be-120">workbookNamedItem</span></span>](workbooknameditem.md) |<span data-ttu-id="308be-121">Чтение свойств и связей объекта namedItem.</span><span class="sxs-lookup"><span data-stu-id="308be-121">Read properties and relationships of namedItem object.</span></span>|
|[<span data-ttu-id="308be-122">Обновление</span><span class="sxs-lookup"><span data-stu-id="308be-122">Update</span></span>](../api/nameditem-update.md) | [<span data-ttu-id="308be-123">Воркбукнамедитем</span><span class="sxs-lookup"><span data-stu-id="308be-123">workbookNamedItem</span></span>](workbooknameditem.md)   |<span data-ttu-id="308be-124">Обновление объекта NamedItem.</span><span class="sxs-lookup"><span data-stu-id="308be-124">Update NamedItem object.</span></span> |
|[<span data-ttu-id="308be-125">Range</span><span class="sxs-lookup"><span data-stu-id="308be-125">Range</span></span>](../api/nameditem-range.md)|[<span data-ttu-id="308be-126">workbookRange</span><span class="sxs-lookup"><span data-stu-id="308be-126">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="308be-p103">Возвращает объект Range, сопоставленный с именем. Вызывает исключение, если тип именованного элемента не является диапазоном.</span><span class="sxs-lookup"><span data-stu-id="308be-p103">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>|
|[<span data-ttu-id="308be-129">Список</span><span class="sxs-lookup"><span data-stu-id="308be-129">List</span></span>](../api/nameditem-list.md) | <span data-ttu-id="308be-130">Коллекция [воркбукнамедитем](workbooknameditem.md)</span><span class="sxs-lookup"><span data-stu-id="308be-130">[workbookNamedItem](workbooknameditem.md) collection</span></span> |<span data-ttu-id="308be-131">Получение коллекции объектов namedItem.</span><span class="sxs-lookup"><span data-stu-id="308be-131">Get namedItem object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="308be-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="308be-132">Properties</span></span>
| <span data-ttu-id="308be-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="308be-133">Property</span></span>     | <span data-ttu-id="308be-134">Тип</span><span class="sxs-lookup"><span data-stu-id="308be-134">Type</span></span>   |<span data-ttu-id="308be-135">Описание</span><span class="sxs-lookup"><span data-stu-id="308be-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="308be-136">name</span><span class="sxs-lookup"><span data-stu-id="308be-136">name</span></span>|<span data-ttu-id="308be-137">string</span><span class="sxs-lookup"><span data-stu-id="308be-137">string</span></span>|<span data-ttu-id="308be-p104">Имя объекта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="308be-p104">The name of the object. Read-only.</span></span>|
|<span data-ttu-id="308be-140">comment</span><span class="sxs-lookup"><span data-stu-id="308be-140">comment</span></span>|<span data-ttu-id="308be-141">string</span><span class="sxs-lookup"><span data-stu-id="308be-141">string</span></span>|<span data-ttu-id="308be-142">Представляет примечание, связанное с этим именем.</span><span class="sxs-lookup"><span data-stu-id="308be-142">Represents the comment associated with this name.</span></span>|
|<span data-ttu-id="308be-143">scope</span><span class="sxs-lookup"><span data-stu-id="308be-143">scope</span></span>|<span data-ttu-id="308be-144">string</span><span class="sxs-lookup"><span data-stu-id="308be-144">string</span></span>|<span data-ttu-id="308be-p105">Указывает, относится ли имя к книге или определенному листу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="308be-p105">Indicates whether the name is scoped to the workbook or to a specific worksheet. Read-only.</span></span>|
|<span data-ttu-id="308be-147">type</span><span class="sxs-lookup"><span data-stu-id="308be-147">type</span></span>|<span data-ttu-id="308be-148">string</span><span class="sxs-lookup"><span data-stu-id="308be-148">string</span></span>|<span data-ttu-id="308be-p106">Указывает тип ссылки, связанный с именем. Возможные значения: `String`, `Integer`, `Double`, `Boolean`, `Range`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="308be-p106">Indicates what type of reference is associated with the name. Possible values are: `String`, `Integer`, `Double`, `Boolean`, `Range`. Read-only.</span></span>|
|<span data-ttu-id="308be-152">value</span><span class="sxs-lookup"><span data-stu-id="308be-152">value</span></span>|<span data-ttu-id="308be-153">строка</span><span class="sxs-lookup"><span data-stu-id="308be-153">string</span></span>|<span data-ttu-id="308be-p107">Представляет формулу, на которую ссылается имя. Например, =Sheet14!$B$2:$H$12, =4.75 и т. д. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="308be-p107">Represents the formula that the name is defined to refer to. E.g. =Sheet14!$B$2:$H$12, =4.75, etc. Read-only.</span></span>|
|<span data-ttu-id="308be-157">visible</span><span class="sxs-lookup"><span data-stu-id="308be-157">visible</span></span>|<span data-ttu-id="308be-158">boolean</span><span class="sxs-lookup"><span data-stu-id="308be-158">boolean</span></span>|<span data-ttu-id="308be-159">Определяет, является ли объект видимым.</span><span class="sxs-lookup"><span data-stu-id="308be-159">Specifies whether the object is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="308be-160">Отношения</span><span class="sxs-lookup"><span data-stu-id="308be-160">Relationships</span></span>
| <span data-ttu-id="308be-161">Отношение</span><span class="sxs-lookup"><span data-stu-id="308be-161">Relationship</span></span>     | <span data-ttu-id="308be-162">Тип</span><span class="sxs-lookup"><span data-stu-id="308be-162">Type</span></span>   |<span data-ttu-id="308be-163">Описание</span><span class="sxs-lookup"><span data-stu-id="308be-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="308be-164">worksheet</span><span class="sxs-lookup"><span data-stu-id="308be-164">worksheet</span></span>|[<span data-ttu-id="308be-165">Воркбукворкшит</span><span class="sxs-lookup"><span data-stu-id="308be-165">workbookWorksheet</span></span>](workbookworksheet.md)|<span data-ttu-id="308be-p108">Возвращает лист, к которому относится именованный элемент. Доступно, только если элемент относится к листу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="308be-p108">Returns the worksheet on which the named item is scoped to. Available only if the item is scoped to the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="308be-169">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="308be-169">JSON representation</span></span>

<span data-ttu-id="308be-170">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="308be-170">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookNamedItem"
}-->

```json
{
  "name": "string",
  "comment": "string",
  "scope": "string",
  "type": "string",
  "value": "string",
  "visible": true
  
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "NamedItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
