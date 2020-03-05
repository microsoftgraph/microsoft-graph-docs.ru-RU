---
title: Тип ресурса Воркбукнамедитем
description: Представляет определенное имя для диапазона ячеек или значения. Имена могут быть простыми именованными объектами (как показано ниже в столбце "Тип"), объектом диапазона и ссылкой на диапазон. Этот объект может использоваться для получения объекта диапазона, связанного с именами.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: ''
ms.openlocfilehash: 17b9e7a04a2524febcb949829b626bc6efe6b779
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519213"
---
# <a name="workbooknameditem-resource-type"></a><span data-ttu-id="72d12-105">Тип ресурса Воркбукнамедитем</span><span class="sxs-lookup"><span data-stu-id="72d12-105">workbookNamedItem resource type</span></span>

<span data-ttu-id="72d12-106">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="72d12-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72d12-p102">Представляет определенное имя для диапазона ячеек или значения. Имена могут быть простыми именованными объектами (как показано ниже в столбце "Тип"), объектом диапазона и ссылкой на диапазон. Этот объект может использоваться для получения объекта диапазона, связанного с именами.</span><span class="sxs-lookup"><span data-stu-id="72d12-p102">Represents a defined name for a range of cells or value. Names can be primitive named objects (as seen in the type below), range object, reference to a range. This object can be used to obtain range object associated with names.</span></span>


## <a name="methods"></a><span data-ttu-id="72d12-110">Методы</span><span class="sxs-lookup"><span data-stu-id="72d12-110">Methods</span></span>

| <span data-ttu-id="72d12-111">Метод</span><span class="sxs-lookup"><span data-stu-id="72d12-111">Method</span></span>           | <span data-ttu-id="72d12-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="72d12-112">Return Type</span></span>    |<span data-ttu-id="72d12-113">Описание</span><span class="sxs-lookup"><span data-stu-id="72d12-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="72d12-114">Add</span><span class="sxs-lookup"><span data-stu-id="72d12-114">Add</span></span>](../api/nameditem-add.md)|[<span data-ttu-id="72d12-115">воркбукнамедитем</span><span class="sxs-lookup"><span data-stu-id="72d12-115">workbookNamedItem</span></span>](workbooknameditem.md)|<span data-ttu-id="72d12-116">Добавляет новое имя в определенную коллекцию.</span><span class="sxs-lookup"><span data-stu-id="72d12-116">Adds a new name to the collection of the given scope.</span></span>|
|[<span data-ttu-id="72d12-117">AddFormulaLocal</span><span class="sxs-lookup"><span data-stu-id="72d12-117">AddFormulaLocal</span></span>](../api/nameditem-addformulalocal.md)|[<span data-ttu-id="72d12-118">воркбукнамедитем</span><span class="sxs-lookup"><span data-stu-id="72d12-118">workbookNamedItem</span></span>](workbooknameditem.md)|<span data-ttu-id="72d12-119">Добавляет новое имя в определенную коллекцию, используя языковой стандарт пользователя для формулы.</span><span class="sxs-lookup"><span data-stu-id="72d12-119">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>|
|[<span data-ttu-id="72d12-120">Get NamedItem</span><span class="sxs-lookup"><span data-stu-id="72d12-120">Get NamedItem</span></span>](../api/nameditem-get.md) | [<span data-ttu-id="72d12-121">воркбукнамедитем</span><span class="sxs-lookup"><span data-stu-id="72d12-121">workbookNamedItem</span></span>](workbooknameditem.md) |<span data-ttu-id="72d12-122">Чтение свойств и связей объекта namedItem.</span><span class="sxs-lookup"><span data-stu-id="72d12-122">Read properties and relationships of namedItem object.</span></span>|
|[<span data-ttu-id="72d12-123">Обновление</span><span class="sxs-lookup"><span data-stu-id="72d12-123">Update</span></span>](../api/nameditem-update.md) | [<span data-ttu-id="72d12-124">воркбукнамедитем</span><span class="sxs-lookup"><span data-stu-id="72d12-124">workbookNamedItem</span></span>](workbooknameditem.md)   |<span data-ttu-id="72d12-125">Обновление объекта NamedItem.</span><span class="sxs-lookup"><span data-stu-id="72d12-125">Update NamedItem object.</span></span> |
|[<span data-ttu-id="72d12-126">Range</span><span class="sxs-lookup"><span data-stu-id="72d12-126">Range</span></span>](../api/nameditem-range.md)|[<span data-ttu-id="72d12-127">workbookRange</span><span class="sxs-lookup"><span data-stu-id="72d12-127">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="72d12-p103">Возвращает объект Range, сопоставленный с именем. Вызывает исключение, если тип именованного элемента не является диапазоном.</span><span class="sxs-lookup"><span data-stu-id="72d12-p103">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>|
|[<span data-ttu-id="72d12-130">Список</span><span class="sxs-lookup"><span data-stu-id="72d12-130">List</span></span>](../api/nameditem-list.md) | <span data-ttu-id="72d12-131">Коллекция [воркбукнамедитем](workbooknameditem.md)</span><span class="sxs-lookup"><span data-stu-id="72d12-131">[workbookNamedItem](workbooknameditem.md) collection</span></span> |<span data-ttu-id="72d12-132">Получение коллекции объектов namedItem.</span><span class="sxs-lookup"><span data-stu-id="72d12-132">Get namedItem object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="72d12-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="72d12-133">Properties</span></span>
| <span data-ttu-id="72d12-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="72d12-134">Property</span></span>     | <span data-ttu-id="72d12-135">Тип</span><span class="sxs-lookup"><span data-stu-id="72d12-135">Type</span></span>   |<span data-ttu-id="72d12-136">Описание</span><span class="sxs-lookup"><span data-stu-id="72d12-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72d12-137">name</span><span class="sxs-lookup"><span data-stu-id="72d12-137">name</span></span>|<span data-ttu-id="72d12-138">string</span><span class="sxs-lookup"><span data-stu-id="72d12-138">string</span></span>|<span data-ttu-id="72d12-p104">Имя объекта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72d12-p104">The name of the object. Read-only.</span></span>|
|<span data-ttu-id="72d12-141">comment</span><span class="sxs-lookup"><span data-stu-id="72d12-141">comment</span></span>|<span data-ttu-id="72d12-142">строка</span><span class="sxs-lookup"><span data-stu-id="72d12-142">string</span></span>|<span data-ttu-id="72d12-143">Представляет примечание, связанное с этим именем.</span><span class="sxs-lookup"><span data-stu-id="72d12-143">Represents the comment associated with this name.</span></span>|
|<span data-ttu-id="72d12-144">scope</span><span class="sxs-lookup"><span data-stu-id="72d12-144">scope</span></span>|<span data-ttu-id="72d12-145">string</span><span class="sxs-lookup"><span data-stu-id="72d12-145">string</span></span>|<span data-ttu-id="72d12-p105">Указывает, относится ли имя к книге или определенному листу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72d12-p105">Indicates whether the name is scoped to the workbook or to a specific worksheet. Read-only.</span></span>|
|<span data-ttu-id="72d12-148">type</span><span class="sxs-lookup"><span data-stu-id="72d12-148">type</span></span>|<span data-ttu-id="72d12-149">string</span><span class="sxs-lookup"><span data-stu-id="72d12-149">string</span></span>|<span data-ttu-id="72d12-p106">Указывает тип ссылки, связанный с именем. Возможные значения: `String`, `Integer`, `Double`, `Boolean`, `Range`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72d12-p106">Indicates what type of reference is associated with the name. Possible values are: `String`, `Integer`, `Double`, `Boolean`, `Range`. Read-only.</span></span>|
|<span data-ttu-id="72d12-153">value</span><span class="sxs-lookup"><span data-stu-id="72d12-153">value</span></span>|<span data-ttu-id="72d12-154">строка</span><span class="sxs-lookup"><span data-stu-id="72d12-154">string</span></span>|<span data-ttu-id="72d12-p107">Представляет формулу, на которую ссылается имя. Например, =Sheet14!$B$2:$H$12, =4.75 и т. д. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72d12-p107">Represents the formula that the name is defined to refer to. E.g. =Sheet14!$B$2:$H$12, =4.75, etc. Read-only.</span></span>|
|<span data-ttu-id="72d12-158">visible</span><span class="sxs-lookup"><span data-stu-id="72d12-158">visible</span></span>|<span data-ttu-id="72d12-159">boolean</span><span class="sxs-lookup"><span data-stu-id="72d12-159">boolean</span></span>|<span data-ttu-id="72d12-160">Определяет, является ли объект видимым.</span><span class="sxs-lookup"><span data-stu-id="72d12-160">Specifies whether the object is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="72d12-161">Связи</span><span class="sxs-lookup"><span data-stu-id="72d12-161">Relationships</span></span>
| <span data-ttu-id="72d12-162">Связь</span><span class="sxs-lookup"><span data-stu-id="72d12-162">Relationship</span></span>     | <span data-ttu-id="72d12-163">Тип</span><span class="sxs-lookup"><span data-stu-id="72d12-163">Type</span></span>   |<span data-ttu-id="72d12-164">Описание</span><span class="sxs-lookup"><span data-stu-id="72d12-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72d12-165">worksheet</span><span class="sxs-lookup"><span data-stu-id="72d12-165">worksheet</span></span>|[<span data-ttu-id="72d12-166">воркбукворкшит</span><span class="sxs-lookup"><span data-stu-id="72d12-166">workbookWorksheet</span></span>](workbookworksheet.md)|<span data-ttu-id="72d12-p108">Возвращает лист, к которому относится именованный элемент. Доступно, только если элемент относится к листу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72d12-p108">Returns the worksheet on which the named item is scoped to. Available only if the item is scoped to the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="72d12-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="72d12-170">JSON representation</span></span>

<span data-ttu-id="72d12-171">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72d12-171">Here is a JSON representation of the resource.</span></span>

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
