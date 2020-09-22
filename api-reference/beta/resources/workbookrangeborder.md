---
title: Тип ресурса Воркбукранжебордер
description: Представляет границу объекта.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 054b2db2b1292136c5044a158f3aaa6072d68e51
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046244"
---
# <a name="workbookrangeborder-resource-type"></a><span data-ttu-id="9d55c-103">Тип ресурса Воркбукранжебордер</span><span class="sxs-lookup"><span data-stu-id="9d55c-103">workbookRangeBorder resource type</span></span>

<span data-ttu-id="9d55c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d55c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d55c-105">Представляет границу объекта.</span><span class="sxs-lookup"><span data-stu-id="9d55c-105">Represents the border of an object.</span></span>


## <a name="methods"></a><span data-ttu-id="9d55c-106">Методы</span><span class="sxs-lookup"><span data-stu-id="9d55c-106">Methods</span></span>

| <span data-ttu-id="9d55c-107">Метод</span><span class="sxs-lookup"><span data-stu-id="9d55c-107">Method</span></span>           | <span data-ttu-id="9d55c-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9d55c-108">Return Type</span></span>    |<span data-ttu-id="9d55c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9d55c-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9d55c-110">Получение Воркбукранжебордер</span><span class="sxs-lookup"><span data-stu-id="9d55c-110">Get workbookRangeBorder</span></span>](../api/rangeborder-get.md) | [<span data-ttu-id="9d55c-111">воркбукранжебордер</span><span class="sxs-lookup"><span data-stu-id="9d55c-111">workbookRangeBorder</span></span>](workbookrangeborder.md) |<span data-ttu-id="9d55c-112">Чтение свойств и связей объекта rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="9d55c-112">Read properties and relationships of rangeBorder object.</span></span>|
|[<span data-ttu-id="9d55c-113">Обновление</span><span class="sxs-lookup"><span data-stu-id="9d55c-113">Update</span></span>](../api/rangeborder-update.md) | [<span data-ttu-id="9d55c-114">воркбукранжебордер</span><span class="sxs-lookup"><span data-stu-id="9d55c-114">workbookRangeBorder</span></span>](workbookrangeborder.md) |<span data-ttu-id="9d55c-115">Обновление объекта RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="9d55c-115">Update RangeBorder object.</span></span> |
|[<span data-ttu-id="9d55c-116">Список</span><span class="sxs-lookup"><span data-stu-id="9d55c-116">List</span></span>](../api/rangeborder-list.md) | <span data-ttu-id="9d55c-117">Коллекция [воркбукранжебордер](workbookrangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="9d55c-117">[workbookRangeBorder](workbookrangeborder.md) collection</span></span> |<span data-ttu-id="9d55c-118">Получение коллекции объектов rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="9d55c-118">Get rangeBorder object collection.</span></span> |
|[<span data-ttu-id="9d55c-119">Itemat</span><span class="sxs-lookup"><span data-stu-id="9d55c-119">Itemat</span></span>](../api/rangebordercollection-itemat.md)|[<span data-ttu-id="9d55c-120">воркбукранжебордер</span><span class="sxs-lookup"><span data-stu-id="9d55c-120">workbookRangeBorder</span></span>](workbookrangeborder.md)|<span data-ttu-id="9d55c-121">Получает объект границы по индексу.</span><span class="sxs-lookup"><span data-stu-id="9d55c-121">Gets a border object using its index</span></span>|

## <a name="properties"></a><span data-ttu-id="9d55c-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="9d55c-122">Properties</span></span>
| <span data-ttu-id="9d55c-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d55c-123">Property</span></span>     | <span data-ttu-id="9d55c-124">Тип</span><span class="sxs-lookup"><span data-stu-id="9d55c-124">Type</span></span>   |<span data-ttu-id="9d55c-125">Описание</span><span class="sxs-lookup"><span data-stu-id="9d55c-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d55c-126">color</span><span class="sxs-lookup"><span data-stu-id="9d55c-126">color</span></span>|<span data-ttu-id="9d55c-127">string</span><span class="sxs-lookup"><span data-stu-id="9d55c-127">string</span></span>|<span data-ttu-id="9d55c-128">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова (например, orange).</span><span class="sxs-lookup"><span data-stu-id="9d55c-128">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="9d55c-129">id</span><span class="sxs-lookup"><span data-stu-id="9d55c-129">id</span></span>|<span data-ttu-id="9d55c-130">string</span><span class="sxs-lookup"><span data-stu-id="9d55c-130">string</span></span>|<span data-ttu-id="9d55c-p101">Представляет идентификатор границы. Возможные значения: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9d55c-p101">Represents border identifier. Possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Read-only.</span></span>|
|<span data-ttu-id="9d55c-134">сидеиндекс</span><span class="sxs-lookup"><span data-stu-id="9d55c-134">sideIndex</span></span>|<span data-ttu-id="9d55c-135">string</span><span class="sxs-lookup"><span data-stu-id="9d55c-135">string</span></span>|<span data-ttu-id="9d55c-p102">Постоянное значение, указывающее определенную сторону границы. Возможные значения: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9d55c-p102">Constant value that indicates the specific side of the border. Possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Read-only.</span></span>|
|<span data-ttu-id="9d55c-139">style</span><span class="sxs-lookup"><span data-stu-id="9d55c-139">style</span></span>|<span data-ttu-id="9d55c-140">string</span><span class="sxs-lookup"><span data-stu-id="9d55c-140">string</span></span>|<span data-ttu-id="9d55c-p103">Одна из констант типа линии, определяющая тип линии границы. Возможные значения: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="9d55c-p103">One of the constants of line style specifying the line style for the border. Possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="9d55c-143">weight</span><span class="sxs-lookup"><span data-stu-id="9d55c-143">weight</span></span>|<span data-ttu-id="9d55c-144">string</span><span class="sxs-lookup"><span data-stu-id="9d55c-144">string</span></span>|<span data-ttu-id="9d55c-p104">Определяет толщину границы вокруг диапазона. Возможные значения: `Hairline`, `Thin`, `Medium`, `Thick`.</span><span class="sxs-lookup"><span data-stu-id="9d55c-p104">Specifies the weight of the border around a range. Possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d55c-147">Связи</span><span class="sxs-lookup"><span data-stu-id="9d55c-147">Relationships</span></span>
<span data-ttu-id="9d55c-148">Нет</span><span class="sxs-lookup"><span data-stu-id="9d55c-148">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9d55c-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9d55c-149">JSON representation</span></span>

<span data-ttu-id="9d55c-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d55c-150">Here is a JSON representation of the resource.</span></span>

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


