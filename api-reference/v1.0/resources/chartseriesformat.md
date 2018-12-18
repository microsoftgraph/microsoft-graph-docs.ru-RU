---
title: Тип ресурса ChartSeriesFormat
description: Инкапсулирует свойства формата для ряда диаграммы.
author: lumine2008
ms.openlocfilehash: 9c27a20c6be6987c31579ca88d546ee80c86d3ea
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354063"
---
# <a name="chartseriesformat-resource-type"></a><span data-ttu-id="5dd2a-103">Тип ресурса ChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="5dd2a-103">ChartSeriesFormat resource type</span></span>

<span data-ttu-id="5dd2a-104">Инкапсулирует свойства формата для ряда диаграммы.</span><span class="sxs-lookup"><span data-stu-id="5dd2a-104">encapsulates the format properties for the chart series</span></span>


## <a name="methods"></a><span data-ttu-id="5dd2a-105">Методы</span><span class="sxs-lookup"><span data-stu-id="5dd2a-105">Methods</span></span>
<span data-ttu-id="5dd2a-106">Нет</span><span class="sxs-lookup"><span data-stu-id="5dd2a-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="5dd2a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5dd2a-107">Properties</span></span>
<span data-ttu-id="5dd2a-108">Нет</span><span class="sxs-lookup"><span data-stu-id="5dd2a-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="5dd2a-109">Связи</span><span class="sxs-lookup"><span data-stu-id="5dd2a-109">Relationships</span></span>
| <span data-ttu-id="5dd2a-110">Связь</span><span class="sxs-lookup"><span data-stu-id="5dd2a-110">Relationship</span></span> | <span data-ttu-id="5dd2a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="5dd2a-111">Type</span></span>   |<span data-ttu-id="5dd2a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5dd2a-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5dd2a-113">fill</span><span class="sxs-lookup"><span data-stu-id="5dd2a-113">fill</span></span>|[<span data-ttu-id="5dd2a-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="5dd2a-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="5dd2a-p101">Представляет формат заливки ряда диаграммы, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5dd2a-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="5dd2a-117">line</span><span class="sxs-lookup"><span data-stu-id="5dd2a-117">line</span></span>|[<span data-ttu-id="5dd2a-118">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="5dd2a-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="5dd2a-p102">Представляет форматирование линий. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5dd2a-p102">Represents line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="5dd2a-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5dd2a-121">JSON representation</span></span>

<span data-ttu-id="5dd2a-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5dd2a-122">Here is a JSON representation of the resource.</span></span>

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