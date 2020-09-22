---
title: Тип ресурса Воркбукикон
description: Представляет значок ячейки.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: ruoyingl
ms.openlocfilehash: bc2145da07a649f06de49bfb9af97567173fe746
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079650"
---
# <a name="workbookicon-resource-type"></a><span data-ttu-id="35752-103">Тип ресурса Воркбукикон</span><span class="sxs-lookup"><span data-stu-id="35752-103">workbookIcon resource type</span></span>

<span data-ttu-id="35752-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35752-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35752-105">Представляет значок ячейки.</span><span class="sxs-lookup"><span data-stu-id="35752-105">Represents a cell icon.</span></span>


## <a name="methods"></a><span data-ttu-id="35752-106">Методы</span><span class="sxs-lookup"><span data-stu-id="35752-106">Methods</span></span>

| <span data-ttu-id="35752-107">Метод</span><span class="sxs-lookup"><span data-stu-id="35752-107">Method</span></span>           | <span data-ttu-id="35752-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="35752-108">Return Type</span></span>    |<span data-ttu-id="35752-109">Описание</span><span class="sxs-lookup"><span data-stu-id="35752-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="35752-110">Получение объекта Icon</span><span class="sxs-lookup"><span data-stu-id="35752-110">Get Icon</span></span>](../api/icon-get.md) | [<span data-ttu-id="35752-111">воркбукикон</span><span class="sxs-lookup"><span data-stu-id="35752-111">workbookIcon</span></span>](workbookicon.md) |<span data-ttu-id="35752-112">Чтение свойств и связей объекта значка.</span><span class="sxs-lookup"><span data-stu-id="35752-112">Read properties and relationships of icon object.</span></span>|
|[<span data-ttu-id="35752-113">Обновление</span><span class="sxs-lookup"><span data-stu-id="35752-113">Update</span></span>](../api/icon-update.md) | [<span data-ttu-id="35752-114">воркбукикон</span><span class="sxs-lookup"><span data-stu-id="35752-114">workbookIcon</span></span>](workbookicon.md)  |<span data-ttu-id="35752-115">Обновление объекта значка.</span><span class="sxs-lookup"><span data-stu-id="35752-115">Update Icon object.</span></span> |

## <a name="properties"></a><span data-ttu-id="35752-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="35752-116">Properties</span></span>
| <span data-ttu-id="35752-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="35752-117">Property</span></span>     | <span data-ttu-id="35752-118">Тип</span><span class="sxs-lookup"><span data-stu-id="35752-118">Type</span></span>   |<span data-ttu-id="35752-119">Описание</span><span class="sxs-lookup"><span data-stu-id="35752-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35752-120">index</span><span class="sxs-lookup"><span data-stu-id="35752-120">index</span></span>|<span data-ttu-id="35752-121">int</span><span class="sxs-lookup"><span data-stu-id="35752-121">int</span></span>|<span data-ttu-id="35752-122">Представляет собой индекс значка данного набора.</span><span class="sxs-lookup"><span data-stu-id="35752-122">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="35752-123">set</span><span class="sxs-lookup"><span data-stu-id="35752-123">set</span></span>|<span data-ttu-id="35752-124">string</span><span class="sxs-lookup"><span data-stu-id="35752-124">string</span></span>|<span data-ttu-id="35752-p101">Представляет набор, в который входит значок. Возможные значения: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span><span class="sxs-lookup"><span data-stu-id="35752-p101">Represents the set that the icon is part of. Possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35752-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="35752-127">Relationships</span></span>
<span data-ttu-id="35752-128">Нет</span><span class="sxs-lookup"><span data-stu-id="35752-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="35752-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35752-129">JSON representation</span></span>

<span data-ttu-id="35752-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35752-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookIcon"
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
  "suppressions": []
}
-->


