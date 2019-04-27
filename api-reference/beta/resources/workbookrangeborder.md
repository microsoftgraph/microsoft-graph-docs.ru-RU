---
title: Тип ресурса Воркбукранжебордер
description: Представляет границу объекта.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6b7bf53e74679a591c113f89c8744ff9c20a1211
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348978"
---
# <a name="workbookrangeborder-resource-type"></a><span data-ttu-id="5cddc-103">Тип ресурса Воркбукранжебордер</span><span class="sxs-lookup"><span data-stu-id="5cddc-103">workbookRangeBorder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cddc-104">Представляет границу объекта.</span><span class="sxs-lookup"><span data-stu-id="5cddc-104">Represents the border of an object.</span></span>


## <a name="methods"></a><span data-ttu-id="5cddc-105">Методы</span><span class="sxs-lookup"><span data-stu-id="5cddc-105">Methods</span></span>

| <span data-ttu-id="5cddc-106">Метод</span><span class="sxs-lookup"><span data-stu-id="5cddc-106">Method</span></span>           | <span data-ttu-id="5cddc-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5cddc-107">Return Type</span></span>    |<span data-ttu-id="5cddc-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5cddc-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5cddc-109">Получение Воркбукранжебордер</span><span class="sxs-lookup"><span data-stu-id="5cddc-109">Get workbookRangeBorder</span></span>](../api/rangeborder-get.md) | [<span data-ttu-id="5cddc-110">Воркбукранжебордер</span><span class="sxs-lookup"><span data-stu-id="5cddc-110">workbookRangeBorder</span></span>](workbookrangeborder.md) |<span data-ttu-id="5cddc-111">Чтение свойств и связей объекта rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="5cddc-111">Read properties and relationships of rangeBorder object.</span></span>|
|[<span data-ttu-id="5cddc-112">Обновление</span><span class="sxs-lookup"><span data-stu-id="5cddc-112">Update</span></span>](../api/rangeborder-update.md) | [<span data-ttu-id="5cddc-113">Воркбукранжебордер</span><span class="sxs-lookup"><span data-stu-id="5cddc-113">workbookRangeBorder</span></span>](workbookrangeborder.md) |<span data-ttu-id="5cddc-114">Обновление объекта RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="5cddc-114">Update RangeBorder object.</span></span> |
|[<span data-ttu-id="5cddc-115">Список</span><span class="sxs-lookup"><span data-stu-id="5cddc-115">List</span></span>](../api/rangeborder-list.md) | <span data-ttu-id="5cddc-116">Коллекция [воркбукранжебордер](workbookrangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="5cddc-116">[workbookRangeBorder](workbookrangeborder.md) collection</span></span> |<span data-ttu-id="5cddc-117">Получение коллекции объектов rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="5cddc-117">Get rangeBorder object collection.</span></span> |
|[<span data-ttu-id="5cddc-118">Itemat</span><span class="sxs-lookup"><span data-stu-id="5cddc-118">Itemat</span></span>](../api/rangebordercollection-itemat.md)|[<span data-ttu-id="5cddc-119">Воркбукранжебордер</span><span class="sxs-lookup"><span data-stu-id="5cddc-119">workbookRangeBorder</span></span>](workbookrangeborder.md)|<span data-ttu-id="5cddc-120">Получает объект границы по индексу.</span><span class="sxs-lookup"><span data-stu-id="5cddc-120">Gets a border object using its index</span></span>|

## <a name="properties"></a><span data-ttu-id="5cddc-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="5cddc-121">Properties</span></span>
| <span data-ttu-id="5cddc-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="5cddc-122">Property</span></span>     | <span data-ttu-id="5cddc-123">Тип</span><span class="sxs-lookup"><span data-stu-id="5cddc-123">Type</span></span>   |<span data-ttu-id="5cddc-124">Описание</span><span class="sxs-lookup"><span data-stu-id="5cddc-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5cddc-125">color</span><span class="sxs-lookup"><span data-stu-id="5cddc-125">color</span></span>|<span data-ttu-id="5cddc-126">строка</span><span class="sxs-lookup"><span data-stu-id="5cddc-126">string</span></span>|<span data-ttu-id="5cddc-127">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова (например, orange).</span><span class="sxs-lookup"><span data-stu-id="5cddc-127">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="5cddc-128">id</span><span class="sxs-lookup"><span data-stu-id="5cddc-128">id</span></span>|<span data-ttu-id="5cddc-129">string</span><span class="sxs-lookup"><span data-stu-id="5cddc-129">string</span></span>|<span data-ttu-id="5cddc-p101">Представляет идентификатор границы. Возможные значения: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5cddc-p101">Represents border identifier. Possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Read-only.</span></span>|
|<span data-ttu-id="5cddc-133">Сидеиндекс</span><span class="sxs-lookup"><span data-stu-id="5cddc-133">sideIndex</span></span>|<span data-ttu-id="5cddc-134">string</span><span class="sxs-lookup"><span data-stu-id="5cddc-134">string</span></span>|<span data-ttu-id="5cddc-p102">Постоянное значение, указывающее определенную сторону границы. Возможные значения: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5cddc-p102">Constant value that indicates the specific side of the border. Possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Read-only.</span></span>|
|<span data-ttu-id="5cddc-138">стиль</span><span class="sxs-lookup"><span data-stu-id="5cddc-138">style</span></span>|<span data-ttu-id="5cddc-139">string</span><span class="sxs-lookup"><span data-stu-id="5cddc-139">string</span></span>|<span data-ttu-id="5cddc-p103">Одна из констант типа линии, определяющая тип линии границы. Возможные значения: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="5cddc-p103">One of the constants of line style specifying the line style for the border. Possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="5cddc-142">weight</span><span class="sxs-lookup"><span data-stu-id="5cddc-142">weight</span></span>|<span data-ttu-id="5cddc-143">string</span><span class="sxs-lookup"><span data-stu-id="5cddc-143">string</span></span>|<span data-ttu-id="5cddc-p104">Определяет толщину границы вокруг диапазона. Возможные значения: `Hairline`, `Thin`, `Medium`, `Thick`.</span><span class="sxs-lookup"><span data-stu-id="5cddc-p104">Specifies the weight of the border around a range. Possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5cddc-146">Отношения</span><span class="sxs-lookup"><span data-stu-id="5cddc-146">Relationships</span></span>
<span data-ttu-id="5cddc-147">Нет</span><span class="sxs-lookup"><span data-stu-id="5cddc-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="5cddc-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5cddc-148">JSON representation</span></span>

<span data-ttu-id="5cddc-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5cddc-149">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "RangeBorder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
