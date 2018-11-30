---
title: Тип ресурса ChartSeriesFormat
description: Инкапсулирует свойства формата для ряда диаграммы.
ms.openlocfilehash: 81b79331580c2d7edbc52f19d1c4c9cfd57db0cf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025794"
---
# <a name="chartseriesformat-resource-type"></a><span data-ttu-id="c3fc4-103">Тип ресурса ChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="c3fc4-103">ChartSeriesFormat resource type</span></span>

<span data-ttu-id="c3fc4-104">Инкапсулирует свойства формата для ряда диаграммы.</span><span class="sxs-lookup"><span data-stu-id="c3fc4-104">encapsulates the format properties for the chart series</span></span>


## <a name="methods"></a><span data-ttu-id="c3fc4-105">Методы</span><span class="sxs-lookup"><span data-stu-id="c3fc4-105">Methods</span></span>
<span data-ttu-id="c3fc4-106">Нет</span><span class="sxs-lookup"><span data-stu-id="c3fc4-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="c3fc4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c3fc4-107">Properties</span></span>
<span data-ttu-id="c3fc4-108">Нет</span><span class="sxs-lookup"><span data-stu-id="c3fc4-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="c3fc4-109">Связи</span><span class="sxs-lookup"><span data-stu-id="c3fc4-109">Relationships</span></span>
| <span data-ttu-id="c3fc4-110">Связь</span><span class="sxs-lookup"><span data-stu-id="c3fc4-110">Relationship</span></span> | <span data-ttu-id="c3fc4-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c3fc4-111">Type</span></span>   |<span data-ttu-id="c3fc4-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c3fc4-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3fc4-113">fill</span><span class="sxs-lookup"><span data-stu-id="c3fc4-113">fill</span></span>|[<span data-ttu-id="c3fc4-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="c3fc4-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="c3fc4-p101">Представляет формат заливки ряда диаграммы, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c3fc4-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="c3fc4-117">line</span><span class="sxs-lookup"><span data-stu-id="c3fc4-117">line</span></span>|[<span data-ttu-id="c3fc4-118">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="c3fc4-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="c3fc4-p102">Представляет форматирование линий. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c3fc4-p102">Represents line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="c3fc4-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c3fc4-121">JSON representation</span></span>

<span data-ttu-id="c3fc4-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3fc4-122">Here is a JSON representation of the resource.</span></span>

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