---
title: Тип ресурса RangeBorder
description: Представляет границу объекта.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 8b5a12c05bed39363d8a8a01eef749f2e88b929e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034932"
---
# <a name="rangeborder-resource-type"></a><span data-ttu-id="470f3-103">Тип ресурса RangeBorder</span><span class="sxs-lookup"><span data-stu-id="470f3-103">RangeBorder resource type</span></span>

<span data-ttu-id="470f3-104">Представляет границу объекта.</span><span class="sxs-lookup"><span data-stu-id="470f3-104">Represents the border of an object.</span></span>


## <a name="methods"></a><span data-ttu-id="470f3-105">Методы</span><span class="sxs-lookup"><span data-stu-id="470f3-105">Methods</span></span>

| <span data-ttu-id="470f3-106">Метод</span><span class="sxs-lookup"><span data-stu-id="470f3-106">Method</span></span>           | <span data-ttu-id="470f3-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="470f3-107">Return Type</span></span>    |<span data-ttu-id="470f3-108">Описание</span><span class="sxs-lookup"><span data-stu-id="470f3-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="470f3-109">Получение объекта RangeBorder</span><span class="sxs-lookup"><span data-stu-id="470f3-109">Get RangeBorder</span></span>](../api/rangeborder-get.md) | [<span data-ttu-id="470f3-110">Воркбукранжебордер</span><span class="sxs-lookup"><span data-stu-id="470f3-110">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="470f3-111">Чтение свойств и связей объекта rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="470f3-111">Read properties and relationships of rangeBorder object.</span></span>|
|[<span data-ttu-id="470f3-112">Обновление</span><span class="sxs-lookup"><span data-stu-id="470f3-112">Update</span></span>](../api/rangeborder-update.md) | [<span data-ttu-id="470f3-113">Воркбукранжебордер</span><span class="sxs-lookup"><span data-stu-id="470f3-113">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="470f3-114">Обновление объекта RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="470f3-114">Update RangeBorder object.</span></span> |
|[<span data-ttu-id="470f3-115">Список</span><span class="sxs-lookup"><span data-stu-id="470f3-115">List</span></span>](../api/rangeborder-list.md) | <span data-ttu-id="470f3-116">Коллекция [воркбукранжебордер](rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="470f3-116">[WorkbookRangeBorder](rangeborder.md) collection</span></span> |<span data-ttu-id="470f3-117">Получение коллекции объектов rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="470f3-117">Get rangeBorder object collection.</span></span> |
|[<span data-ttu-id="470f3-118">Itemat</span><span class="sxs-lookup"><span data-stu-id="470f3-118">Itemat</span></span>](../api/rangebordercollection-itemat.md)|[<span data-ttu-id="470f3-119">Воркбукранжебордер</span><span class="sxs-lookup"><span data-stu-id="470f3-119">WorkbookRangeBorder</span></span>](rangeborder.md)|<span data-ttu-id="470f3-120">Получает объект границы по индексу.</span><span class="sxs-lookup"><span data-stu-id="470f3-120">Gets a border object using its index</span></span>|

## <a name="properties"></a><span data-ttu-id="470f3-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="470f3-121">Properties</span></span>
| <span data-ttu-id="470f3-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="470f3-122">Property</span></span>     | <span data-ttu-id="470f3-123">Тип</span><span class="sxs-lookup"><span data-stu-id="470f3-123">Type</span></span>   |<span data-ttu-id="470f3-124">Описание</span><span class="sxs-lookup"><span data-stu-id="470f3-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="470f3-125">color</span><span class="sxs-lookup"><span data-stu-id="470f3-125">color</span></span>|<span data-ttu-id="470f3-126">строка</span><span class="sxs-lookup"><span data-stu-id="470f3-126">string</span></span>|<span data-ttu-id="470f3-127">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова (например, orange).</span><span class="sxs-lookup"><span data-stu-id="470f3-127">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="470f3-128">id</span><span class="sxs-lookup"><span data-stu-id="470f3-128">id</span></span>|<span data-ttu-id="470f3-129">string</span><span class="sxs-lookup"><span data-stu-id="470f3-129">string</span></span>|<span data-ttu-id="470f3-130">Представляет идентификатор границы.</span><span class="sxs-lookup"><span data-stu-id="470f3-130">Represents border identifier.</span></span> <span data-ttu-id="470f3-131">Возможные `EdgeTop`значения:, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`,. `DiagonalUp`</span><span class="sxs-lookup"><span data-stu-id="470f3-131">The possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span></span> <span data-ttu-id="470f3-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="470f3-132">Read-only.</span></span>|
|<span data-ttu-id="470f3-133">Сидеиндекс</span><span class="sxs-lookup"><span data-stu-id="470f3-133">sideIndex</span></span>|<span data-ttu-id="470f3-134">string</span><span class="sxs-lookup"><span data-stu-id="470f3-134">string</span></span>|<span data-ttu-id="470f3-135">Постоянное значение, указывающее определенную сторону границы.</span><span class="sxs-lookup"><span data-stu-id="470f3-135">Constant value that indicates the specific side of the border.</span></span> <span data-ttu-id="470f3-136">Возможные `EdgeTop`значения:, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`,. `DiagonalUp`</span><span class="sxs-lookup"><span data-stu-id="470f3-136">The possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span></span> <span data-ttu-id="470f3-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="470f3-137">Read-only.</span></span>|
|<span data-ttu-id="470f3-138">style</span><span class="sxs-lookup"><span data-stu-id="470f3-138">style</span></span>|<span data-ttu-id="470f3-139">string</span><span class="sxs-lookup"><span data-stu-id="470f3-139">string</span></span>|<span data-ttu-id="470f3-140">Одна из констант стиля линии, определяющая стиль линии границы.</span><span class="sxs-lookup"><span data-stu-id="470f3-140">One of the constants of line style specifying the line style for the border.</span></span> <span data-ttu-id="470f3-141">Возможные `None`значения:, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`,. `SlantDashDot`</span><span class="sxs-lookup"><span data-stu-id="470f3-141">The possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="470f3-142">weight</span><span class="sxs-lookup"><span data-stu-id="470f3-142">weight</span></span>|<span data-ttu-id="470f3-143">string</span><span class="sxs-lookup"><span data-stu-id="470f3-143">string</span></span>|<span data-ttu-id="470f3-144">Определяет толщину границы вокруг диапазона.</span><span class="sxs-lookup"><span data-stu-id="470f3-144">Specifies the weight of the border around a range.</span></span> <span data-ttu-id="470f3-145">Допустимые значения: `Hairline`, `Thin`, `Medium`, `Thick`.</span><span class="sxs-lookup"><span data-stu-id="470f3-145">The possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="470f3-146">Отношения</span><span class="sxs-lookup"><span data-stu-id="470f3-146">Relationships</span></span>
<span data-ttu-id="470f3-147">Нет</span><span class="sxs-lookup"><span data-stu-id="470f3-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="470f3-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="470f3-148">JSON representation</span></span>

<span data-ttu-id="470f3-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="470f3-149">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeBorder"
}-->

```json
{
  "color": "string",
  "id": "string",
  "sideIndex": "string",
  "style": "string",
  "weight": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
