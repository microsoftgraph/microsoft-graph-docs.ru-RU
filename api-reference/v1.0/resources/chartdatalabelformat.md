---
title: Тип ресурса ChartDataLabelFormat
description: Инкапсулирует свойства формата для меток данных диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 645267fd595a4b8e83090d9d6b2179e8c6112a78
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951994"
---
# <a name="chartdatalabelformat-resource-type"></a><span data-ttu-id="0edb3-103">Тип ресурса ChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="0edb3-103">ChartDataLabelFormat resource type</span></span>

<span data-ttu-id="0edb3-104">Инкапсулирует свойства формата для меток данных диаграммы.</span><span class="sxs-lookup"><span data-stu-id="0edb3-104">Encapsulates the format properties for the chart data labels.</span></span>


## <a name="methods"></a><span data-ttu-id="0edb3-105">Методы</span><span class="sxs-lookup"><span data-stu-id="0edb3-105">Methods</span></span>
<span data-ttu-id="0edb3-106">Нет</span><span class="sxs-lookup"><span data-stu-id="0edb3-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="0edb3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0edb3-107">Properties</span></span>
<span data-ttu-id="0edb3-108">Нет</span><span class="sxs-lookup"><span data-stu-id="0edb3-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="0edb3-109">Связи</span><span class="sxs-lookup"><span data-stu-id="0edb3-109">Relationships</span></span>
| <span data-ttu-id="0edb3-110">Связь</span><span class="sxs-lookup"><span data-stu-id="0edb3-110">Relationship</span></span> | <span data-ttu-id="0edb3-111">Тип</span><span class="sxs-lookup"><span data-stu-id="0edb3-111">Type</span></span>   |<span data-ttu-id="0edb3-112">Описание</span><span class="sxs-lookup"><span data-stu-id="0edb3-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0edb3-113">fill</span><span class="sxs-lookup"><span data-stu-id="0edb3-113">fill</span></span>|[<span data-ttu-id="0edb3-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="0edb3-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="0edb3-p101">Представляет формат заливки для текущей метки данных диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0edb3-p101">Represents the fill format of the current chart data label. Read-only.</span></span>|
|<span data-ttu-id="0edb3-117">font</span><span class="sxs-lookup"><span data-stu-id="0edb3-117">font</span></span>|[<span data-ttu-id="0edb3-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="0edb3-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="0edb3-p102">Представляет атрибуты шрифта (имя, размер, цвет и т. д.) для метки данных диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0edb3-p102">Represents the font attributes (font name, font size, color, etc.) for a chart data label. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="0edb3-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0edb3-121">JSON representation</span></span>

<span data-ttu-id="0edb3-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0edb3-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartDataLabelFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartDataLabelFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
