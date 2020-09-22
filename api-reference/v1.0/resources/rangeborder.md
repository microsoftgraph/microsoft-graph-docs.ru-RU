---
title: Тип ресурса RangeBorder
description: Представляет границу объекта.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: a4536607c4723a9e16d77e045e17bd151da50d36
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090930"
---
# <a name="rangeborder-resource-type"></a><span data-ttu-id="40100-103">Тип ресурса RangeBorder</span><span class="sxs-lookup"><span data-stu-id="40100-103">RangeBorder resource type</span></span>

<span data-ttu-id="40100-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40100-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="40100-105">Представляет границу объекта.</span><span class="sxs-lookup"><span data-stu-id="40100-105">Represents the border of an object.</span></span>


## <a name="methods"></a><span data-ttu-id="40100-106">Методы</span><span class="sxs-lookup"><span data-stu-id="40100-106">Methods</span></span>

| <span data-ttu-id="40100-107">Метод</span><span class="sxs-lookup"><span data-stu-id="40100-107">Method</span></span>           | <span data-ttu-id="40100-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="40100-108">Return Type</span></span>    |<span data-ttu-id="40100-109">Описание</span><span class="sxs-lookup"><span data-stu-id="40100-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="40100-110">Получение объекта RangeBorder</span><span class="sxs-lookup"><span data-stu-id="40100-110">Get RangeBorder</span></span>](../api/rangeborder-get.md) | [<span data-ttu-id="40100-111">воркбукранжебордер</span><span class="sxs-lookup"><span data-stu-id="40100-111">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="40100-112">Чтение свойств и связей объекта rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="40100-112">Read properties and relationships of rangeBorder object.</span></span>|
|[<span data-ttu-id="40100-113">Обновление</span><span class="sxs-lookup"><span data-stu-id="40100-113">Update</span></span>](../api/rangeborder-update.md) | [<span data-ttu-id="40100-114">воркбукранжебордер</span><span class="sxs-lookup"><span data-stu-id="40100-114">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="40100-115">Обновление объекта RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="40100-115">Update RangeBorder object.</span></span> |
|[<span data-ttu-id="40100-116">Список</span><span class="sxs-lookup"><span data-stu-id="40100-116">List</span></span>](../api/rangeborder-list.md) | <span data-ttu-id="40100-117">Коллекция [воркбукранжебордер](rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="40100-117">[WorkbookRangeBorder](rangeborder.md) collection</span></span> |<span data-ttu-id="40100-118">Получение коллекции объектов rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="40100-118">Get rangeBorder object collection.</span></span> |
|[<span data-ttu-id="40100-119">Itemat</span><span class="sxs-lookup"><span data-stu-id="40100-119">Itemat</span></span>](../api/rangebordercollection-itemat.md)|[<span data-ttu-id="40100-120">воркбукранжебордер</span><span class="sxs-lookup"><span data-stu-id="40100-120">WorkbookRangeBorder</span></span>](rangeborder.md)|<span data-ttu-id="40100-121">Получает объект границы по индексу.</span><span class="sxs-lookup"><span data-stu-id="40100-121">Gets a border object using its index</span></span>|

## <a name="properties"></a><span data-ttu-id="40100-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="40100-122">Properties</span></span>
| <span data-ttu-id="40100-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="40100-123">Property</span></span>     | <span data-ttu-id="40100-124">Тип</span><span class="sxs-lookup"><span data-stu-id="40100-124">Type</span></span>   |<span data-ttu-id="40100-125">Описание</span><span class="sxs-lookup"><span data-stu-id="40100-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40100-126">color</span><span class="sxs-lookup"><span data-stu-id="40100-126">color</span></span>|<span data-ttu-id="40100-127">string</span><span class="sxs-lookup"><span data-stu-id="40100-127">string</span></span>|<span data-ttu-id="40100-128">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова (например, orange).</span><span class="sxs-lookup"><span data-stu-id="40100-128">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="40100-129">id</span><span class="sxs-lookup"><span data-stu-id="40100-129">id</span></span>|<span data-ttu-id="40100-130">string</span><span class="sxs-lookup"><span data-stu-id="40100-130">string</span></span>|<span data-ttu-id="40100-131">Представляет идентификатор границы.</span><span class="sxs-lookup"><span data-stu-id="40100-131">Represents border identifier.</span></span> <span data-ttu-id="40100-132">Возможные значения:,, `EdgeTop` `EdgeBottom` ,, `EdgeLeft` `EdgeRight` `InsideVertical` , `InsideHorizontal` , `DiagonalDown` , `DiagonalUp` .</span><span class="sxs-lookup"><span data-stu-id="40100-132">The possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span></span> <span data-ttu-id="40100-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="40100-133">Read-only.</span></span>|
|<span data-ttu-id="40100-134">сидеиндекс</span><span class="sxs-lookup"><span data-stu-id="40100-134">sideIndex</span></span>|<span data-ttu-id="40100-135">string</span><span class="sxs-lookup"><span data-stu-id="40100-135">string</span></span>|<span data-ttu-id="40100-136">Постоянное значение, указывающее определенную сторону границы.</span><span class="sxs-lookup"><span data-stu-id="40100-136">Constant value that indicates the specific side of the border.</span></span> <span data-ttu-id="40100-137">Возможные значения:,, `EdgeTop` `EdgeBottom` ,, `EdgeLeft` `EdgeRight` `InsideVertical` , `InsideHorizontal` , `DiagonalDown` , `DiagonalUp` .</span><span class="sxs-lookup"><span data-stu-id="40100-137">The possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span></span> <span data-ttu-id="40100-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="40100-138">Read-only.</span></span>|
|<span data-ttu-id="40100-139">style</span><span class="sxs-lookup"><span data-stu-id="40100-139">style</span></span>|<span data-ttu-id="40100-140">string</span><span class="sxs-lookup"><span data-stu-id="40100-140">string</span></span>|<span data-ttu-id="40100-141">Одна из констант стиля линии, определяющая стиль линии границы.</span><span class="sxs-lookup"><span data-stu-id="40100-141">One of the constants of line style specifying the line style for the border.</span></span> <span data-ttu-id="40100-142">Возможные значения:,, `None` `Continuous` ,, `Dash` `DashDot` `DashDotDot` , `Dot` , `Double` , `SlantDashDot` .</span><span class="sxs-lookup"><span data-stu-id="40100-142">The possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="40100-143">weight</span><span class="sxs-lookup"><span data-stu-id="40100-143">weight</span></span>|<span data-ttu-id="40100-144">string</span><span class="sxs-lookup"><span data-stu-id="40100-144">string</span></span>|<span data-ttu-id="40100-145">Определяет толщину границы вокруг диапазона.</span><span class="sxs-lookup"><span data-stu-id="40100-145">Specifies the weight of the border around a range.</span></span> <span data-ttu-id="40100-146">Допустимые значения: `Hairline`, `Thin`, `Medium`, `Thick`.</span><span class="sxs-lookup"><span data-stu-id="40100-146">The possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="40100-147">Связи</span><span class="sxs-lookup"><span data-stu-id="40100-147">Relationships</span></span>
<span data-ttu-id="40100-148">Нет</span><span class="sxs-lookup"><span data-stu-id="40100-148">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="40100-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="40100-149">JSON representation</span></span>

<span data-ttu-id="40100-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40100-150">Here is a JSON representation of the resource.</span></span>

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

