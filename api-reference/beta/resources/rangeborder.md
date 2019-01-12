---
title: Тип ресурса RangeBorder
description: Представляет границу объекта.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 8404a45ea7c56bbbb318994daa55229706d700a2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960240"
---
# <a name="rangeborder-resource-type"></a><span data-ttu-id="e5d42-103">Тип ресурса RangeBorder</span><span class="sxs-lookup"><span data-stu-id="e5d42-103">RangeBorder resource type</span></span>

> <span data-ttu-id="e5d42-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e5d42-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5d42-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5d42-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e5d42-106">Представляет границу объекта.</span><span class="sxs-lookup"><span data-stu-id="e5d42-106">Represents the border of an object.</span></span>


## <a name="methods"></a><span data-ttu-id="e5d42-107">Методы</span><span class="sxs-lookup"><span data-stu-id="e5d42-107">Methods</span></span>

| <span data-ttu-id="e5d42-108">Метод</span><span class="sxs-lookup"><span data-stu-id="e5d42-108">Method</span></span>           | <span data-ttu-id="e5d42-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e5d42-109">Return Type</span></span>    |<span data-ttu-id="e5d42-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e5d42-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e5d42-111">Получение объекта RangeBorder</span><span class="sxs-lookup"><span data-stu-id="e5d42-111">Get RangeBorder</span></span>](../api/rangeborder-get.md) | [<span data-ttu-id="e5d42-112">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="e5d42-112">RangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="e5d42-113">Чтение свойств и связей объекта rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="e5d42-113">Read properties and relationships of rangeBorder object.</span></span>|
|<span data-ttu-id="e5d42-114">[обновление](../api/rangeborder-update.md).</span><span class="sxs-lookup"><span data-stu-id="e5d42-114">[Update](../api/rangeborder-update.md)</span></span> | [<span data-ttu-id="e5d42-115">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="e5d42-115">RangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="e5d42-116">Обновление объекта RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="e5d42-116">Update RangeBorder object.</span></span> |
|[<span data-ttu-id="e5d42-117">List</span><span class="sxs-lookup"><span data-stu-id="e5d42-117">List</span></span>](../api/rangeborder-list.md) | <span data-ttu-id="e5d42-118">Коллекция объектов [RangeBorder](rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="e5d42-118">[RangeBorder](rangeborder.md) collection</span></span> |<span data-ttu-id="e5d42-119">Получение коллекции объектов rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="e5d42-119">Get rangeBorder object collection.</span></span> |
|[<span data-ttu-id="e5d42-120">Itemat</span><span class="sxs-lookup"><span data-stu-id="e5d42-120">Itemat</span></span>](../api/rangebordercollection-itemat.md)|[<span data-ttu-id="e5d42-121">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="e5d42-121">RangeBorder</span></span>](rangeborder.md)|<span data-ttu-id="e5d42-122">Возвращает объект границы по его индексу.</span><span class="sxs-lookup"><span data-stu-id="e5d42-122">Gets a border object using its index</span></span>|

## <a name="properties"></a><span data-ttu-id="e5d42-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="e5d42-123">Properties</span></span>
| <span data-ttu-id="e5d42-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5d42-124">Property</span></span>     | <span data-ttu-id="e5d42-125">Тип</span><span class="sxs-lookup"><span data-stu-id="e5d42-125">Type</span></span>   |<span data-ttu-id="e5d42-126">Описание</span><span class="sxs-lookup"><span data-stu-id="e5d42-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5d42-127">color</span><span class="sxs-lookup"><span data-stu-id="e5d42-127">color</span></span>|<span data-ttu-id="e5d42-128">строка</span><span class="sxs-lookup"><span data-stu-id="e5d42-128">string</span></span>|<span data-ttu-id="e5d42-129">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова (например, orange).</span><span class="sxs-lookup"><span data-stu-id="e5d42-129">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="e5d42-130">id</span><span class="sxs-lookup"><span data-stu-id="e5d42-130">id</span></span>|<span data-ttu-id="e5d42-131">строка</span><span class="sxs-lookup"><span data-stu-id="e5d42-131">string</span></span>|<span data-ttu-id="e5d42-p102">Представляет идентификатор границы. Возможные значения: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e5d42-p102">Represents border identifier. Possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Read-only.</span></span>|
|<span data-ttu-id="e5d42-135">sideIndex</span><span class="sxs-lookup"><span data-stu-id="e5d42-135">sideIndex</span></span>|<span data-ttu-id="e5d42-136">string</span><span class="sxs-lookup"><span data-stu-id="e5d42-136">string</span></span>|<span data-ttu-id="e5d42-p103">Постоянное значение, указывающее определенную сторону границы. Возможные значения: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e5d42-p103">Constant value that indicates the specific side of the border. Possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Read-only.</span></span>|
|<span data-ttu-id="e5d42-140">style</span><span class="sxs-lookup"><span data-stu-id="e5d42-140">style</span></span>|<span data-ttu-id="e5d42-141">строка</span><span class="sxs-lookup"><span data-stu-id="e5d42-141">string</span></span>|<span data-ttu-id="e5d42-p104">Одна из констант типа линии, определяющая тип линии границы. Возможные значения: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="e5d42-p104">One of the constants of line style specifying the line style for the border. Possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="e5d42-144">weight</span><span class="sxs-lookup"><span data-stu-id="e5d42-144">weight</span></span>|<span data-ttu-id="e5d42-145">string</span><span class="sxs-lookup"><span data-stu-id="e5d42-145">string</span></span>|<span data-ttu-id="e5d42-p105">Определяет толщину границы вокруг диапазона. Возможные значения: `Hairline`, `Thin`, `Medium`, `Thick`.</span><span class="sxs-lookup"><span data-stu-id="e5d42-p105">Specifies the weight of the border around a range. Possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5d42-148">Связи</span><span class="sxs-lookup"><span data-stu-id="e5d42-148">Relationships</span></span>
<span data-ttu-id="e5d42-149">Нет</span><span class="sxs-lookup"><span data-stu-id="e5d42-149">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e5d42-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e5d42-150">JSON representation</span></span>

<span data-ttu-id="e5d42-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5d42-151">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeBorder"
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
