---
title: Тип ресурса ChartSeriesFormat
description: Инкапсулирует свойства формата для ряда диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ce9a777936b25ed77b130dc2b2219eba0f72c183
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029752"
---
# <a name="chartseriesformat-resource-type"></a><span data-ttu-id="04a05-103">Тип ресурса ChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="04a05-103">ChartSeriesFormat resource type</span></span>

<span data-ttu-id="04a05-104">Инкапсулирует свойства формата для ряда диаграммы.</span><span class="sxs-lookup"><span data-stu-id="04a05-104">encapsulates the format properties for the chart series</span></span>


## <a name="methods"></a><span data-ttu-id="04a05-105">Методы</span><span class="sxs-lookup"><span data-stu-id="04a05-105">Methods</span></span>
<span data-ttu-id="04a05-106">Нет</span><span class="sxs-lookup"><span data-stu-id="04a05-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="04a05-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="04a05-107">Properties</span></span>
<span data-ttu-id="04a05-108">Нет</span><span class="sxs-lookup"><span data-stu-id="04a05-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="04a05-109">Отношения</span><span class="sxs-lookup"><span data-stu-id="04a05-109">Relationships</span></span>
| <span data-ttu-id="04a05-110">Отношение</span><span class="sxs-lookup"><span data-stu-id="04a05-110">Relationship</span></span> | <span data-ttu-id="04a05-111">Тип</span><span class="sxs-lookup"><span data-stu-id="04a05-111">Type</span></span>   |<span data-ttu-id="04a05-112">Описание</span><span class="sxs-lookup"><span data-stu-id="04a05-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04a05-113">fill</span><span class="sxs-lookup"><span data-stu-id="04a05-113">fill</span></span>|[<span data-ttu-id="04a05-114">Воркбукчартфилл</span><span class="sxs-lookup"><span data-stu-id="04a05-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="04a05-p101">Представляет формат заливки ряда диаграммы, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="04a05-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="04a05-117">line</span><span class="sxs-lookup"><span data-stu-id="04a05-117">line</span></span>|[<span data-ttu-id="04a05-118">Воркбукчартлинеформат</span><span class="sxs-lookup"><span data-stu-id="04a05-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="04a05-119">Представляет форматирование линий.</span><span class="sxs-lookup"><span data-stu-id="04a05-119">Represents line formatting.</span></span> <span data-ttu-id="04a05-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="04a05-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="04a05-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="04a05-121">JSON representation</span></span>

<span data-ttu-id="04a05-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04a05-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartSeriesFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeriesFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
