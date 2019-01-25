---
title: Тип ресурса RangeBorder
description: Представляет границу объекта.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5b3b814da53013d1daca686d549596a7ab656027
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515386"
---
# <a name="rangeborder-resource-type"></a><span data-ttu-id="d4292-103">Тип ресурса RangeBorder</span><span class="sxs-lookup"><span data-stu-id="d4292-103">RangeBorder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4292-104">Представляет границу объекта.</span><span class="sxs-lookup"><span data-stu-id="d4292-104">Represents the border of an object.</span></span>


## <a name="methods"></a><span data-ttu-id="d4292-105">Методы</span><span class="sxs-lookup"><span data-stu-id="d4292-105">Methods</span></span>

| <span data-ttu-id="d4292-106">Метод</span><span class="sxs-lookup"><span data-stu-id="d4292-106">Method</span></span>           | <span data-ttu-id="d4292-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d4292-107">Return Type</span></span>    |<span data-ttu-id="d4292-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d4292-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4292-109">Получение объекта RangeBorder</span><span class="sxs-lookup"><span data-stu-id="d4292-109">[Get RangeBorder](../api/rangeborder-get.md)</span></span> | <span data-ttu-id="d4292-110">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="d4292-110">[RangeBorder](rangeborder.md)</span></span> |<span data-ttu-id="d4292-111">Чтение свойств и связей объекта rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="d4292-111">Read properties and relationships of rangeBorder object.</span></span>|
|[<span data-ttu-id="d4292-112">Update</span><span class="sxs-lookup"><span data-stu-id="d4292-112">Update</span></span>](../api/rangeborder-update.md) | <span data-ttu-id="d4292-113">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="d4292-113">[RangeBorder](rangeborder.md)</span></span> |<span data-ttu-id="d4292-114">Обновление объекта RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="d4292-114">Update RangeBorder object.</span></span> |
|[<span data-ttu-id="d4292-115">List</span><span class="sxs-lookup"><span data-stu-id="d4292-115">List</span></span>](../api/rangeborder-list.md) | <span data-ttu-id="d4292-116">Коллекция объектов RangeBorder</span><span class="sxs-lookup"><span data-stu-id="d4292-116">[RangeBorder](rangeborder.md) collection</span></span> |<span data-ttu-id="d4292-117">Получение коллекции объектов rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="d4292-117">Get rangeBorder object collection.</span></span> |
|[<span data-ttu-id="d4292-118">Itemat</span><span class="sxs-lookup"><span data-stu-id="d4292-118">Itemat</span></span>](../api/rangebordercollection-itemat.md)|<span data-ttu-id="d4292-119">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="d4292-119">[RangeBorder](rangeborder.md)</span></span>|<span data-ttu-id="d4292-120">Возвращает объект границы по его индексу.</span><span class="sxs-lookup"><span data-stu-id="d4292-120">Gets a border object using its index</span></span>|

## <a name="properties"></a><span data-ttu-id="d4292-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="d4292-121">Properties</span></span>
| <span data-ttu-id="d4292-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4292-122">Property</span></span>     | <span data-ttu-id="d4292-123">Тип</span><span class="sxs-lookup"><span data-stu-id="d4292-123">Type</span></span>   |<span data-ttu-id="d4292-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d4292-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4292-125">color</span><span class="sxs-lookup"><span data-stu-id="d4292-125">color</span></span>|<span data-ttu-id="d4292-126">строка</span><span class="sxs-lookup"><span data-stu-id="d4292-126">string</span></span>|<span data-ttu-id="d4292-127">HTML-код, представляющий цвет линии границы в виде #RRGGBB (например, FFA500) или в виде ключевого слова (например, orange).</span><span class="sxs-lookup"><span data-stu-id="d4292-127">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="d4292-128">id</span><span class="sxs-lookup"><span data-stu-id="d4292-128">id</span></span>|<span data-ttu-id="d4292-129">string</span><span class="sxs-lookup"><span data-stu-id="d4292-129">string</span></span>|<span data-ttu-id="d4292-p101">Представляет идентификатор границы. Возможные значения: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d4292-p101">Represents border identifier. Possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Read-only.</span></span>|
|<span data-ttu-id="d4292-133">sideIndex</span><span class="sxs-lookup"><span data-stu-id="d4292-133">sideIndex</span></span>|<span data-ttu-id="d4292-134">string</span><span class="sxs-lookup"><span data-stu-id="d4292-134">string</span></span>|<span data-ttu-id="d4292-p102">Постоянное значение, указывающее определенную сторону границы. Возможные значения: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d4292-p102">Constant value that indicates the specific side of the border. Possible values are: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Read-only.</span></span>|
|<span data-ttu-id="d4292-138">style</span><span class="sxs-lookup"><span data-stu-id="d4292-138">style</span></span>|<span data-ttu-id="d4292-139">строка</span><span class="sxs-lookup"><span data-stu-id="d4292-139">string</span></span>|<span data-ttu-id="d4292-p103">Одна из констант типа линии, определяющая тип линии границы. Возможные значения: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="d4292-p103">One of the constants of line style specifying the line style for the border. Possible values are: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span></span>|
|<span data-ttu-id="d4292-142">weight</span><span class="sxs-lookup"><span data-stu-id="d4292-142">weight</span></span>|<span data-ttu-id="d4292-143">string</span><span class="sxs-lookup"><span data-stu-id="d4292-143">string</span></span>|<span data-ttu-id="d4292-p104">Определяет толщину границы вокруг диапазона. Возможные значения: `Hairline`, `Thin`, `Medium`, `Thick`.</span><span class="sxs-lookup"><span data-stu-id="d4292-p104">Specifies the weight of the border around a range. Possible values are: `Hairline`, `Thin`, `Medium`, `Thick`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4292-146">Отношения</span><span class="sxs-lookup"><span data-stu-id="d4292-146">Relationships</span></span>
<span data-ttu-id="d4292-147">Нет</span><span class="sxs-lookup"><span data-stu-id="d4292-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d4292-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d4292-148">JSON representation</span></span>

<span data-ttu-id="d4292-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4292-149">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "RangeBorder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/rangeborder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
