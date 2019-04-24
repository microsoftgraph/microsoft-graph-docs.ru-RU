---
title: Тип ресурса Icon
description: Представляет значок ячейки.
localization_priority: Normal
ms.openlocfilehash: c15ee02d1c6830cbb5246826665d0353b7e999b9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506413"
---
# <a name="icon-resource-type"></a><span data-ttu-id="74624-103">Тип ресурса Icon</span><span class="sxs-lookup"><span data-stu-id="74624-103">Icon resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74624-104">Представляет значок ячейки.</span><span class="sxs-lookup"><span data-stu-id="74624-104">Represents a cell icon.</span></span>


## <a name="methods"></a><span data-ttu-id="74624-105">Методы</span><span class="sxs-lookup"><span data-stu-id="74624-105">Methods</span></span>

| <span data-ttu-id="74624-106">Метод</span><span class="sxs-lookup"><span data-stu-id="74624-106">Method</span></span>           | <span data-ttu-id="74624-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="74624-107">Return Type</span></span>    |<span data-ttu-id="74624-108">Описание</span><span class="sxs-lookup"><span data-stu-id="74624-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="74624-109">Получение объекта Icon</span><span class="sxs-lookup"><span data-stu-id="74624-109">Get Icon</span></span>](../api/icon-get.md) | [<span data-ttu-id="74624-110">Icon</span><span class="sxs-lookup"><span data-stu-id="74624-110">Icon</span></span>](icon.md) |<span data-ttu-id="74624-111">Чтение свойств и связей объекта значка.</span><span class="sxs-lookup"><span data-stu-id="74624-111">Read properties and relationships of icon object.</span></span>|
|[<span data-ttu-id="74624-112">Обновление</span><span class="sxs-lookup"><span data-stu-id="74624-112">Update</span></span>](../api/icon-update.md) | [<span data-ttu-id="74624-113">Icon</span><span class="sxs-lookup"><span data-stu-id="74624-113">Icon</span></span>](icon.md)  |<span data-ttu-id="74624-114">Обновление объекта значка.</span><span class="sxs-lookup"><span data-stu-id="74624-114">Update Icon object.</span></span> |

## <a name="properties"></a><span data-ttu-id="74624-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="74624-115">Properties</span></span>
| <span data-ttu-id="74624-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="74624-116">Property</span></span>     | <span data-ttu-id="74624-117">Тип</span><span class="sxs-lookup"><span data-stu-id="74624-117">Type</span></span>   |<span data-ttu-id="74624-118">Описание</span><span class="sxs-lookup"><span data-stu-id="74624-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74624-119">index</span><span class="sxs-lookup"><span data-stu-id="74624-119">index</span></span>|<span data-ttu-id="74624-120">int</span><span class="sxs-lookup"><span data-stu-id="74624-120">int</span></span>|<span data-ttu-id="74624-121">Представляет собой индекс значка данного набора.</span><span class="sxs-lookup"><span data-stu-id="74624-121">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="74624-122">set</span><span class="sxs-lookup"><span data-stu-id="74624-122">set</span></span>|<span data-ttu-id="74624-123">string</span><span class="sxs-lookup"><span data-stu-id="74624-123">string</span></span>|<span data-ttu-id="74624-p101">Представляет набор, в который входит значок. Возможные значения: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span><span class="sxs-lookup"><span data-stu-id="74624-p101">Represents the set that the icon is part of. Possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="74624-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="74624-126">Relationships</span></span>
<span data-ttu-id="74624-127">Нет</span><span class="sxs-lookup"><span data-stu-id="74624-127">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="74624-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="74624-128">JSON representation</span></span>

<span data-ttu-id="74624-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74624-129">Here is a JSON representation of the resource.</span></span>

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
