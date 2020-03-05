---
title: Тип ресурса Воркбукчартсериесформат
description: Инкапсулирует свойства формата для ряда диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 2558d242e18fa8bf7d220ba5bc4dd8aef6cd2865
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519269"
---
# <a name="workbookchartseriesformat-resource-type"></a><span data-ttu-id="a1bad-103">Тип ресурса Воркбукчартсериесформат</span><span class="sxs-lookup"><span data-stu-id="a1bad-103">workbookChartSeriesFormat resource type</span></span>

<span data-ttu-id="a1bad-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a1bad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1bad-105">Инкапсулирует свойства формата для ряда диаграммы.</span><span class="sxs-lookup"><span data-stu-id="a1bad-105">Encapsulates the format properties for the chart series.</span></span>


## <a name="methods"></a><span data-ttu-id="a1bad-106">Методы</span><span class="sxs-lookup"><span data-stu-id="a1bad-106">Methods</span></span>
<span data-ttu-id="a1bad-107">Нет</span><span class="sxs-lookup"><span data-stu-id="a1bad-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="a1bad-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a1bad-108">Properties</span></span>
<span data-ttu-id="a1bad-109">Нет</span><span class="sxs-lookup"><span data-stu-id="a1bad-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="a1bad-110">Связи</span><span class="sxs-lookup"><span data-stu-id="a1bad-110">Relationships</span></span>
| <span data-ttu-id="a1bad-111">Связь</span><span class="sxs-lookup"><span data-stu-id="a1bad-111">Relationship</span></span> | <span data-ttu-id="a1bad-112">Тип</span><span class="sxs-lookup"><span data-stu-id="a1bad-112">Type</span></span>   |<span data-ttu-id="a1bad-113">Описание</span><span class="sxs-lookup"><span data-stu-id="a1bad-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1bad-114">fill</span><span class="sxs-lookup"><span data-stu-id="a1bad-114">fill</span></span>|[<span data-ttu-id="a1bad-115">воркбукчартфилл</span><span class="sxs-lookup"><span data-stu-id="a1bad-115">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="a1bad-p101">Представляет формат заливки ряда диаграммы, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a1bad-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="a1bad-118">line</span><span class="sxs-lookup"><span data-stu-id="a1bad-118">line</span></span>|[<span data-ttu-id="a1bad-119">воркбукчартлинеформат</span><span class="sxs-lookup"><span data-stu-id="a1bad-119">workbookChartLineFormat</span></span>](workbookchartlineformat.md)|<span data-ttu-id="a1bad-120">Представляет форматирование линий.</span><span class="sxs-lookup"><span data-stu-id="a1bad-120">Represents line formatting.</span></span> <span data-ttu-id="a1bad-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a1bad-121">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="a1bad-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a1bad-122">JSON representation</span></span>

<span data-ttu-id="a1bad-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a1bad-123">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartSeriesFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
