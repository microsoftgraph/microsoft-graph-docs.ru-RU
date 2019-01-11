---
title: Тип ресурса ChartLegend
description: Представляет легенду в диаграмме.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: db5c4531143df52c86e310c1d3670ab72b6e938c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853776"
---
# <a name="chartlegend-resource-type"></a><span data-ttu-id="dfc3a-103">Тип ресурса ChartLegend</span><span class="sxs-lookup"><span data-stu-id="dfc3a-103">ChartLegend resource type</span></span>

> <span data-ttu-id="dfc3a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dfc3a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dfc3a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfc3a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dfc3a-106">Представляет легенду в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="dfc3a-106">Represents the legend in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="dfc3a-107">Методы</span><span class="sxs-lookup"><span data-stu-id="dfc3a-107">Methods</span></span>

| <span data-ttu-id="dfc3a-108">Метод</span><span class="sxs-lookup"><span data-stu-id="dfc3a-108">Method</span></span>           | <span data-ttu-id="dfc3a-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="dfc3a-109">Return Type</span></span>    |<span data-ttu-id="dfc3a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dfc3a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dfc3a-111">Получение объекта ChartLegend</span><span class="sxs-lookup"><span data-stu-id="dfc3a-111">Get ChartLegend</span></span>](../api/chartlegend-get.md) | [<span data-ttu-id="dfc3a-112">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="dfc3a-112">ChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="dfc3a-113">Чтение свойств и связей объекта chartLegend.</span><span class="sxs-lookup"><span data-stu-id="dfc3a-113">Read properties and relationships of chartLegend object.</span></span>|
|<span data-ttu-id="dfc3a-114">[обновление](../api/chartlegend-update.md).</span><span class="sxs-lookup"><span data-stu-id="dfc3a-114">[Update](../api/chartlegend-update.md)</span></span> | [<span data-ttu-id="dfc3a-115">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="dfc3a-115">ChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="dfc3a-116">Обновление объекта ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="dfc3a-116">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="dfc3a-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="dfc3a-117">Properties</span></span>
| <span data-ttu-id="dfc3a-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="dfc3a-118">Property</span></span>     | <span data-ttu-id="dfc3a-119">Тип</span><span class="sxs-lookup"><span data-stu-id="dfc3a-119">Type</span></span>   |<span data-ttu-id="dfc3a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="dfc3a-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dfc3a-121">overlay</span><span class="sxs-lookup"><span data-stu-id="dfc3a-121">overlay</span></span>|<span data-ttu-id="dfc3a-122">boolean</span><span class="sxs-lookup"><span data-stu-id="dfc3a-122">boolean</span></span>|<span data-ttu-id="dfc3a-123">Логическое значение, определяющее, должна ли легенда диаграммы пересекаться с основной частью диаграммы.</span><span class="sxs-lookup"><span data-stu-id="dfc3a-123">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="dfc3a-124">position</span><span class="sxs-lookup"><span data-stu-id="dfc3a-124">position</span></span>|<span data-ttu-id="dfc3a-125">string</span><span class="sxs-lookup"><span data-stu-id="dfc3a-125">string</span></span>|<span data-ttu-id="dfc3a-p102">Представляет расположение легенды на диаграмме. Возможные значения: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span><span class="sxs-lookup"><span data-stu-id="dfc3a-p102">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="dfc3a-128">visible</span><span class="sxs-lookup"><span data-stu-id="dfc3a-128">visible</span></span>|<span data-ttu-id="dfc3a-129">boolean</span><span class="sxs-lookup"><span data-stu-id="dfc3a-129">boolean</span></span>|<span data-ttu-id="dfc3a-130">Логическое значение, представляющее видимость объекта ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="dfc3a-130">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dfc3a-131">Связи</span><span class="sxs-lookup"><span data-stu-id="dfc3a-131">Relationships</span></span>
| <span data-ttu-id="dfc3a-132">Связь</span><span class="sxs-lookup"><span data-stu-id="dfc3a-132">Relationship</span></span> | <span data-ttu-id="dfc3a-133">Тип</span><span class="sxs-lookup"><span data-stu-id="dfc3a-133">Type</span></span>   |<span data-ttu-id="dfc3a-134">Описание</span><span class="sxs-lookup"><span data-stu-id="dfc3a-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dfc3a-135">format</span><span class="sxs-lookup"><span data-stu-id="dfc3a-135">format</span></span>|[<span data-ttu-id="dfc3a-136">ChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="dfc3a-136">ChartLegendFormat</span></span>](chartlegendformat.md)|<span data-ttu-id="dfc3a-p103">Представляет форматирование легенды диаграммы, включая заливку и шрифт. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dfc3a-p103">Represents the formatting of a chart legend, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dfc3a-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dfc3a-139">JSON representation</span></span>

<span data-ttu-id="dfc3a-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dfc3a-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartLegend"
}-->

```json
{
  "overlay": true,
  "position": "string",
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLegend resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
