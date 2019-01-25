---
title: Тип ресурса Icon
description: Представляет значок ячейки.
localization_priority: Normal
ms.openlocfilehash: c15ee02d1c6830cbb5246826665d0353b7e999b9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516303"
---
# <a name="icon-resource-type"></a><span data-ttu-id="b8803-103">Тип ресурса Icon</span><span class="sxs-lookup"><span data-stu-id="b8803-103">Icon resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8803-104">Представляет значок ячейки.</span><span class="sxs-lookup"><span data-stu-id="b8803-104">Represents a cell icon.</span></span>


## <a name="methods"></a><span data-ttu-id="b8803-105">Методы</span><span class="sxs-lookup"><span data-stu-id="b8803-105">Methods</span></span>

| <span data-ttu-id="b8803-106">Метод</span><span class="sxs-lookup"><span data-stu-id="b8803-106">Method</span></span>           | <span data-ttu-id="b8803-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b8803-107">Return Type</span></span>    |<span data-ttu-id="b8803-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b8803-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8803-109">Получение объекта Icon</span><span class="sxs-lookup"><span data-stu-id="b8803-109">[Get Icon](../api/icon-get.md)</span></span> | [<span data-ttu-id="b8803-110">Icon</span><span class="sxs-lookup"><span data-stu-id="b8803-110">Icon</span></span>](icon.md) |<span data-ttu-id="b8803-111">Чтение свойств и связей объекта значка.</span><span class="sxs-lookup"><span data-stu-id="b8803-111">Read properties and relationships of icon object.</span></span>|
|[<span data-ttu-id="b8803-112">Update</span><span class="sxs-lookup"><span data-stu-id="b8803-112">Update</span></span>](../api/icon-update.md) | [<span data-ttu-id="b8803-113">Icon</span><span class="sxs-lookup"><span data-stu-id="b8803-113">Icon</span></span>](icon.md)  |<span data-ttu-id="b8803-114">Обновление объекта значка.</span><span class="sxs-lookup"><span data-stu-id="b8803-114">Update Icon object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b8803-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="b8803-115">Properties</span></span>
| <span data-ttu-id="b8803-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8803-116">Property</span></span>     | <span data-ttu-id="b8803-117">Тип</span><span class="sxs-lookup"><span data-stu-id="b8803-117">Type</span></span>   |<span data-ttu-id="b8803-118">Описание</span><span class="sxs-lookup"><span data-stu-id="b8803-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8803-119">index</span><span class="sxs-lookup"><span data-stu-id="b8803-119">index</span></span>|<span data-ttu-id="b8803-120">int</span><span class="sxs-lookup"><span data-stu-id="b8803-120">int</span></span>|<span data-ttu-id="b8803-121">Представляет собой индекс значка данного набора.</span><span class="sxs-lookup"><span data-stu-id="b8803-121">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="b8803-122">set</span><span class="sxs-lookup"><span data-stu-id="b8803-122">set</span></span>|<span data-ttu-id="b8803-123">string</span><span class="sxs-lookup"><span data-stu-id="b8803-123">string</span></span>|<span data-ttu-id="b8803-p101">Представляет набор, в который входит значок. Возможные значения: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span><span class="sxs-lookup"><span data-stu-id="b8803-p101">Represents the set that the icon is part of. Possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8803-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="b8803-126">Relationships</span></span>
<span data-ttu-id="b8803-127">Нет</span><span class="sxs-lookup"><span data-stu-id="b8803-127">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b8803-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b8803-128">JSON representation</span></span>

<span data-ttu-id="b8803-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8803-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.icon"
}-->

```json
{
  "index": 1024,
  "set": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Icon resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/icon.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
