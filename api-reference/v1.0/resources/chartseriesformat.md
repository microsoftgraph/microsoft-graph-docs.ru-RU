---
title: Тип ресурса ChartSeriesFormat
description: Инкапсулирует свойства формата для ряда диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: fd342e55524d51b6a0382df8ca9310ea162308d2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584998"
---
# <a name="chartseriesformat-resource-type"></a><span data-ttu-id="1df56-103">Тип ресурса ChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="1df56-103">ChartSeriesFormat resource type</span></span>

<span data-ttu-id="1df56-104">Инкапсулирует свойства формата для ряда диаграммы.</span><span class="sxs-lookup"><span data-stu-id="1df56-104">encapsulates the format properties for the chart series</span></span>


## <a name="methods"></a><span data-ttu-id="1df56-105">Методы</span><span class="sxs-lookup"><span data-stu-id="1df56-105">Methods</span></span>
<span data-ttu-id="1df56-106">Нет</span><span class="sxs-lookup"><span data-stu-id="1df56-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="1df56-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1df56-107">Properties</span></span>
<span data-ttu-id="1df56-108">Нет</span><span class="sxs-lookup"><span data-stu-id="1df56-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="1df56-109">Связи</span><span class="sxs-lookup"><span data-stu-id="1df56-109">Relationships</span></span>
| <span data-ttu-id="1df56-110">Отношение</span><span class="sxs-lookup"><span data-stu-id="1df56-110">Relationship</span></span> | <span data-ttu-id="1df56-111">Тип</span><span class="sxs-lookup"><span data-stu-id="1df56-111">Type</span></span>   |<span data-ttu-id="1df56-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1df56-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1df56-113">fill</span><span class="sxs-lookup"><span data-stu-id="1df56-113">fill</span></span>|[<span data-ttu-id="1df56-114">Воркбукчартфилл</span><span class="sxs-lookup"><span data-stu-id="1df56-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="1df56-p101">Представляет формат заливки ряда диаграммы, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1df56-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="1df56-117">line</span><span class="sxs-lookup"><span data-stu-id="1df56-117">line</span></span>|[<span data-ttu-id="1df56-118">Воркбукчартлинеформат</span><span class="sxs-lookup"><span data-stu-id="1df56-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="1df56-119">Представляет форматирование линий.</span><span class="sxs-lookup"><span data-stu-id="1df56-119">Represents line formatting.</span></span> <span data-ttu-id="1df56-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1df56-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="1df56-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1df56-121">JSON representation</span></span>

<span data-ttu-id="1df56-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1df56-122">Here is a JSON representation of the resource.</span></span>

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
