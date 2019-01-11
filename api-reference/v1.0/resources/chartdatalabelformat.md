---
title: Тип ресурса ChartDataLabelFormat
description: Инкапсулирует свойства формата для меток данных диаграммы.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 586b201b0bcc70765fb68aa7736664f493f5539b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876925"
---
# <a name="chartdatalabelformat-resource-type"></a><span data-ttu-id="fb1ff-103">Тип ресурса ChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="fb1ff-103">ChartDataLabelFormat resource type</span></span>

<span data-ttu-id="fb1ff-104">Инкапсулирует свойства формата для меток данных диаграммы.</span><span class="sxs-lookup"><span data-stu-id="fb1ff-104">Encapsulates the format properties for the chart data labels.</span></span>


## <a name="methods"></a><span data-ttu-id="fb1ff-105">Методы</span><span class="sxs-lookup"><span data-stu-id="fb1ff-105">Methods</span></span>
<span data-ttu-id="fb1ff-106">Нет</span><span class="sxs-lookup"><span data-stu-id="fb1ff-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="fb1ff-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="fb1ff-107">Properties</span></span>
<span data-ttu-id="fb1ff-108">Нет</span><span class="sxs-lookup"><span data-stu-id="fb1ff-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="fb1ff-109">Связи</span><span class="sxs-lookup"><span data-stu-id="fb1ff-109">Relationships</span></span>
| <span data-ttu-id="fb1ff-110">Связь</span><span class="sxs-lookup"><span data-stu-id="fb1ff-110">Relationship</span></span> | <span data-ttu-id="fb1ff-111">Тип</span><span class="sxs-lookup"><span data-stu-id="fb1ff-111">Type</span></span>   |<span data-ttu-id="fb1ff-112">Описание</span><span class="sxs-lookup"><span data-stu-id="fb1ff-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb1ff-113">fill</span><span class="sxs-lookup"><span data-stu-id="fb1ff-113">fill</span></span>|[<span data-ttu-id="fb1ff-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="fb1ff-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="fb1ff-p101">Представляет формат заливки для текущей метки данных диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fb1ff-p101">Represents the fill format of the current chart data label. Read-only.</span></span>|
|<span data-ttu-id="fb1ff-117">font</span><span class="sxs-lookup"><span data-stu-id="fb1ff-117">font</span></span>|[<span data-ttu-id="fb1ff-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="fb1ff-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="fb1ff-p102">Представляет атрибуты шрифта (имя, размер, цвет и т. д.) для метки данных диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fb1ff-p102">Represents the font attributes (font name, font size, color, etc.) for a chart data label. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="fb1ff-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fb1ff-121">JSON representation</span></span>

<span data-ttu-id="fb1ff-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb1ff-122">Here is a JSON representation of the resource.</span></span>

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
