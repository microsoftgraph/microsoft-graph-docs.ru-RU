---
title: Тип ресурса Воркбукчартсериесформат
description: Инкапсулирует свойства формата для ряда диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5d07dbaf17fd715b93dcd039fe3fb9e264bd7f63
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33349000"
---
# <a name="workbookchartseriesformat-resource-type"></a><span data-ttu-id="d2030-103">Тип ресурса Воркбукчартсериесформат</span><span class="sxs-lookup"><span data-stu-id="d2030-103">workbookChartSeriesFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2030-104">Инкапсулирует свойства формата для ряда диаграммы.</span><span class="sxs-lookup"><span data-stu-id="d2030-104">Encapsulates the format properties for the chart series.</span></span>


## <a name="methods"></a><span data-ttu-id="d2030-105">Методы</span><span class="sxs-lookup"><span data-stu-id="d2030-105">Methods</span></span>
<span data-ttu-id="d2030-106">Отсутствует</span><span class="sxs-lookup"><span data-stu-id="d2030-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="d2030-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d2030-107">Properties</span></span>
<span data-ttu-id="d2030-108">Нет</span><span class="sxs-lookup"><span data-stu-id="d2030-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="d2030-109">Отношения</span><span class="sxs-lookup"><span data-stu-id="d2030-109">Relationships</span></span>
| <span data-ttu-id="d2030-110">Отношение</span><span class="sxs-lookup"><span data-stu-id="d2030-110">Relationship</span></span> | <span data-ttu-id="d2030-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d2030-111">Type</span></span>   |<span data-ttu-id="d2030-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d2030-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2030-113">fill</span><span class="sxs-lookup"><span data-stu-id="d2030-113">fill</span></span>|[<span data-ttu-id="d2030-114">Воркбукчартфилл</span><span class="sxs-lookup"><span data-stu-id="d2030-114">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="d2030-p101">Представляет формат заливки ряда диаграммы, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d2030-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="d2030-117">line</span><span class="sxs-lookup"><span data-stu-id="d2030-117">line</span></span>|[<span data-ttu-id="d2030-118">Воркбукчартлинеформат</span><span class="sxs-lookup"><span data-stu-id="d2030-118">workbookChartLineFormat</span></span>](workbookchartlineformat.md)|<span data-ttu-id="d2030-119">Представляет форматирование линий.</span><span class="sxs-lookup"><span data-stu-id="d2030-119">Represents line formatting.</span></span> <span data-ttu-id="d2030-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d2030-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="d2030-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d2030-121">JSON representation</span></span>

<span data-ttu-id="d2030-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2030-122">Here is a JSON representation of the resource.</span></span>

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
