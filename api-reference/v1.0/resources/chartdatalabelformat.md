---
title: Тип ресурса ChartDataLabelFormat
description: Инкапсулирует свойства формата для меток данных диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 72f9841948a87c0e22f9943f6c66a60c856adfa7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029836"
---
# <a name="chartdatalabelformat-resource-type"></a><span data-ttu-id="f77c6-103">Тип ресурса ChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="f77c6-103">ChartDataLabelFormat resource type</span></span>

<span data-ttu-id="f77c6-104">Инкапсулирует свойства формата для меток данных диаграммы.</span><span class="sxs-lookup"><span data-stu-id="f77c6-104">Encapsulates the format properties for the chart data labels.</span></span>


## <a name="methods"></a><span data-ttu-id="f77c6-105">Методы</span><span class="sxs-lookup"><span data-stu-id="f77c6-105">Methods</span></span>
<span data-ttu-id="f77c6-106">Нет</span><span class="sxs-lookup"><span data-stu-id="f77c6-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="f77c6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f77c6-107">Properties</span></span>
<span data-ttu-id="f77c6-108">Нет</span><span class="sxs-lookup"><span data-stu-id="f77c6-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="f77c6-109">Отношения</span><span class="sxs-lookup"><span data-stu-id="f77c6-109">Relationships</span></span>
| <span data-ttu-id="f77c6-110">Отношение</span><span class="sxs-lookup"><span data-stu-id="f77c6-110">Relationship</span></span> | <span data-ttu-id="f77c6-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f77c6-111">Type</span></span>   |<span data-ttu-id="f77c6-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f77c6-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f77c6-113">fill</span><span class="sxs-lookup"><span data-stu-id="f77c6-113">fill</span></span>|[<span data-ttu-id="f77c6-114">Воркбукчартфилл</span><span class="sxs-lookup"><span data-stu-id="f77c6-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="f77c6-p101">Представляет формат заливки для текущей метки данных диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f77c6-p101">Represents the fill format of the current chart data label. Read-only.</span></span>|
|<span data-ttu-id="f77c6-117">font</span><span class="sxs-lookup"><span data-stu-id="f77c6-117">font</span></span>|[<span data-ttu-id="f77c6-118">Воркбукчартфонт</span><span class="sxs-lookup"><span data-stu-id="f77c6-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="f77c6-119">Представляет атрибуты шрифта (имя, размер шрифта, цвет и т. д.) для подписи данных диаграммы.</span><span class="sxs-lookup"><span data-stu-id="f77c6-119">Represents the font attributes (font name, font size, color, etc.) for a chart data label.</span></span> <span data-ttu-id="f77c6-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f77c6-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f77c6-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f77c6-121">JSON representation</span></span>

<span data-ttu-id="f77c6-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f77c6-122">Here is a JSON representation of the resource.</span></span>

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
