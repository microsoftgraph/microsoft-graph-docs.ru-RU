---
title: Тип ресурса ChartLegend
description: Представляет легенду в диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c76fd21700616ec6c353644de93bddd0a47ac7dd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980883"
---
# <a name="chartlegend-resource-type"></a><span data-ttu-id="9ab65-103">Тип ресурса ChartLegend</span><span class="sxs-lookup"><span data-stu-id="9ab65-103">ChartLegend resource type</span></span>

> <span data-ttu-id="9ab65-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9ab65-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ab65-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ab65-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9ab65-106">Представляет легенду в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="9ab65-106">Represents the legend in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="9ab65-107">Методы</span><span class="sxs-lookup"><span data-stu-id="9ab65-107">Methods</span></span>

| <span data-ttu-id="9ab65-108">Метод</span><span class="sxs-lookup"><span data-stu-id="9ab65-108">Method</span></span>           | <span data-ttu-id="9ab65-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9ab65-109">Return Type</span></span>    |<span data-ttu-id="9ab65-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9ab65-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9ab65-111">Получение объекта ChartLegend</span><span class="sxs-lookup"><span data-stu-id="9ab65-111">Get ChartLegend</span></span>](../api/chartlegend-get.md) | [<span data-ttu-id="9ab65-112">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="9ab65-112">ChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="9ab65-113">Чтение свойств и связей объекта chartLegend.</span><span class="sxs-lookup"><span data-stu-id="9ab65-113">Read properties and relationships of chartLegend object.</span></span>|
|<span data-ttu-id="9ab65-114">[обновление](../api/chartlegend-update.md).</span><span class="sxs-lookup"><span data-stu-id="9ab65-114">[Update](../api/chartlegend-update.md)</span></span> | [<span data-ttu-id="9ab65-115">ChartLegend</span><span class="sxs-lookup"><span data-stu-id="9ab65-115">ChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="9ab65-116">Обновление объекта ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="9ab65-116">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9ab65-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="9ab65-117">Properties</span></span>
| <span data-ttu-id="9ab65-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ab65-118">Property</span></span>     | <span data-ttu-id="9ab65-119">Тип</span><span class="sxs-lookup"><span data-stu-id="9ab65-119">Type</span></span>   |<span data-ttu-id="9ab65-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9ab65-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ab65-121">overlay</span><span class="sxs-lookup"><span data-stu-id="9ab65-121">overlay</span></span>|<span data-ttu-id="9ab65-122">boolean</span><span class="sxs-lookup"><span data-stu-id="9ab65-122">boolean</span></span>|<span data-ttu-id="9ab65-123">Логическое значение, определяющее, должна ли легенда диаграммы пересекаться с основной частью диаграммы.</span><span class="sxs-lookup"><span data-stu-id="9ab65-123">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="9ab65-124">position</span><span class="sxs-lookup"><span data-stu-id="9ab65-124">position</span></span>|<span data-ttu-id="9ab65-125">string</span><span class="sxs-lookup"><span data-stu-id="9ab65-125">string</span></span>|<span data-ttu-id="9ab65-p102">Представляет расположение легенды на диаграмме. Возможные значения: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span><span class="sxs-lookup"><span data-stu-id="9ab65-p102">Represents the position of the legend on the chart. Possible values are: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span></span>|
|<span data-ttu-id="9ab65-128">visible</span><span class="sxs-lookup"><span data-stu-id="9ab65-128">visible</span></span>|<span data-ttu-id="9ab65-129">boolean</span><span class="sxs-lookup"><span data-stu-id="9ab65-129">boolean</span></span>|<span data-ttu-id="9ab65-130">Логическое значение, представляющее видимость объекта ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="9ab65-130">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ab65-131">Связи</span><span class="sxs-lookup"><span data-stu-id="9ab65-131">Relationships</span></span>
| <span data-ttu-id="9ab65-132">Связь</span><span class="sxs-lookup"><span data-stu-id="9ab65-132">Relationship</span></span> | <span data-ttu-id="9ab65-133">Тип</span><span class="sxs-lookup"><span data-stu-id="9ab65-133">Type</span></span>   |<span data-ttu-id="9ab65-134">Описание</span><span class="sxs-lookup"><span data-stu-id="9ab65-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ab65-135">format</span><span class="sxs-lookup"><span data-stu-id="9ab65-135">format</span></span>|[<span data-ttu-id="9ab65-136">ChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="9ab65-136">ChartLegendFormat</span></span>](chartlegendformat.md)|<span data-ttu-id="9ab65-p103">Представляет форматирование легенды диаграммы, включая заливку и шрифт. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9ab65-p103">Represents the formatting of a chart legend, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9ab65-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9ab65-139">JSON representation</span></span>

<span data-ttu-id="9ab65-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9ab65-140">Here is a JSON representation of the resource.</span></span>

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
