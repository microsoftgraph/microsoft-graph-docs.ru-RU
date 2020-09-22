---
title: Тип ресурса ChartDataLabelFormat
description: Инкапсулирует свойства формата для меток данных диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: a1fbb911a546f1ee8fb48f3337d99e3ebe0fcd8d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988452"
---
# <a name="chartdatalabelformat-resource-type"></a><span data-ttu-id="6b40d-103">Тип ресурса ChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="6b40d-103">ChartDataLabelFormat resource type</span></span>

<span data-ttu-id="6b40d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b40d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6b40d-105">Инкапсулирует свойства формата для меток данных диаграммы.</span><span class="sxs-lookup"><span data-stu-id="6b40d-105">Encapsulates the format properties for the chart data labels.</span></span>


## <a name="methods"></a><span data-ttu-id="6b40d-106">Методы</span><span class="sxs-lookup"><span data-stu-id="6b40d-106">Methods</span></span>
<span data-ttu-id="6b40d-107">Нет</span><span class="sxs-lookup"><span data-stu-id="6b40d-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="6b40d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b40d-108">Properties</span></span>
<span data-ttu-id="6b40d-109">Нет</span><span class="sxs-lookup"><span data-stu-id="6b40d-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="6b40d-110">Связи</span><span class="sxs-lookup"><span data-stu-id="6b40d-110">Relationships</span></span>
| <span data-ttu-id="6b40d-111">Связь</span><span class="sxs-lookup"><span data-stu-id="6b40d-111">Relationship</span></span> | <span data-ttu-id="6b40d-112">Тип</span><span class="sxs-lookup"><span data-stu-id="6b40d-112">Type</span></span>   |<span data-ttu-id="6b40d-113">Описание</span><span class="sxs-lookup"><span data-stu-id="6b40d-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b40d-114">fill</span><span class="sxs-lookup"><span data-stu-id="6b40d-114">fill</span></span>|[<span data-ttu-id="6b40d-115">воркбукчартфилл</span><span class="sxs-lookup"><span data-stu-id="6b40d-115">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="6b40d-p101">Представляет формат заливки для текущей метки данных диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6b40d-p101">Represents the fill format of the current chart data label. Read-only.</span></span>|
|<span data-ttu-id="6b40d-118">font</span><span class="sxs-lookup"><span data-stu-id="6b40d-118">font</span></span>|[<span data-ttu-id="6b40d-119">воркбукчартфонт</span><span class="sxs-lookup"><span data-stu-id="6b40d-119">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="6b40d-120">Представляет атрибуты шрифта (имя, размер шрифта, цвет и т. д.) для подписи данных диаграммы.</span><span class="sxs-lookup"><span data-stu-id="6b40d-120">Represents the font attributes (font name, font size, color, etc.) for a chart data label.</span></span> <span data-ttu-id="6b40d-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6b40d-121">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="6b40d-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6b40d-122">JSON representation</span></span>

<span data-ttu-id="6b40d-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b40d-123">Here is a JSON representation of the resource.</span></span>

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

