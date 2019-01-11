---
title: Тип ресурса Icon
description: Представляет значок ячейки.
localization_priority: Normal
ms.openlocfilehash: e1b31632884c757d40be4a7c9639933439028382
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861693"
---
# <a name="icon-resource-type"></a><span data-ttu-id="b2165-103">Тип ресурса Icon</span><span class="sxs-lookup"><span data-stu-id="b2165-103">Icon resource type</span></span>

> <span data-ttu-id="b2165-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b2165-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2165-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2165-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b2165-106">Представляет значок ячейки.</span><span class="sxs-lookup"><span data-stu-id="b2165-106">Represents a cell icon.</span></span>


## <a name="methods"></a><span data-ttu-id="b2165-107">Методы</span><span class="sxs-lookup"><span data-stu-id="b2165-107">Methods</span></span>

| <span data-ttu-id="b2165-108">Метод</span><span class="sxs-lookup"><span data-stu-id="b2165-108">Method</span></span>           | <span data-ttu-id="b2165-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b2165-109">Return Type</span></span>    |<span data-ttu-id="b2165-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b2165-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b2165-111">Получение объекта Icon</span><span class="sxs-lookup"><span data-stu-id="b2165-111">Get Icon</span></span>](../api/icon-get.md) | [<span data-ttu-id="b2165-112">Icon</span><span class="sxs-lookup"><span data-stu-id="b2165-112">Icon</span></span>](icon.md) |<span data-ttu-id="b2165-113">Чтение свойств и связей объекта значка.</span><span class="sxs-lookup"><span data-stu-id="b2165-113">Read properties and relationships of icon object.</span></span>|
|<span data-ttu-id="b2165-114">[обновление](../api/icon-update.md).</span><span class="sxs-lookup"><span data-stu-id="b2165-114">[Update](../api/icon-update.md)</span></span> | [<span data-ttu-id="b2165-115">Icon</span><span class="sxs-lookup"><span data-stu-id="b2165-115">Icon</span></span>](icon.md)  |<span data-ttu-id="b2165-116">Обновление объекта значка.</span><span class="sxs-lookup"><span data-stu-id="b2165-116">Update Icon object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b2165-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2165-117">Properties</span></span>
| <span data-ttu-id="b2165-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2165-118">Property</span></span>     | <span data-ttu-id="b2165-119">Тип</span><span class="sxs-lookup"><span data-stu-id="b2165-119">Type</span></span>   |<span data-ttu-id="b2165-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b2165-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2165-121">index</span><span class="sxs-lookup"><span data-stu-id="b2165-121">index</span></span>|<span data-ttu-id="b2165-122">int</span><span class="sxs-lookup"><span data-stu-id="b2165-122">int</span></span>|<span data-ttu-id="b2165-123">Представляет собой индекс значка данного набора.</span><span class="sxs-lookup"><span data-stu-id="b2165-123">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="b2165-124">set</span><span class="sxs-lookup"><span data-stu-id="b2165-124">set</span></span>|<span data-ttu-id="b2165-125">string</span><span class="sxs-lookup"><span data-stu-id="b2165-125">string</span></span>|<span data-ttu-id="b2165-p102">Представляет набор, в который входит значок. Возможные значения: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span><span class="sxs-lookup"><span data-stu-id="b2165-p102">Represents the set that the icon is part of. Possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2165-128">Связи</span><span class="sxs-lookup"><span data-stu-id="b2165-128">Relationships</span></span>
<span data-ttu-id="b2165-129">Нет</span><span class="sxs-lookup"><span data-stu-id="b2165-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b2165-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b2165-130">JSON representation</span></span>

<span data-ttu-id="b2165-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2165-131">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Icon resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
