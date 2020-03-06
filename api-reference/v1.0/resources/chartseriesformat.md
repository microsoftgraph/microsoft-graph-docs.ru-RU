---
title: Тип ресурса ChartSeriesFormat
description: Инкапсулирует свойства формата для ряда диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: a44392eb718c157f6422228405f7bb2a4b411733
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533099"
---
# <a name="chartseriesformat-resource-type"></a><span data-ttu-id="a2243-103">Тип ресурса ChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="a2243-103">ChartSeriesFormat resource type</span></span>

<span data-ttu-id="a2243-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2243-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a2243-105">Инкапсулирует свойства формата для ряда диаграммы.</span><span class="sxs-lookup"><span data-stu-id="a2243-105">encapsulates the format properties for the chart series</span></span>


## <a name="methods"></a><span data-ttu-id="a2243-106">Методы</span><span class="sxs-lookup"><span data-stu-id="a2243-106">Methods</span></span>
<span data-ttu-id="a2243-107">Нет</span><span class="sxs-lookup"><span data-stu-id="a2243-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="a2243-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a2243-108">Properties</span></span>
<span data-ttu-id="a2243-109">Нет</span><span class="sxs-lookup"><span data-stu-id="a2243-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="a2243-110">Связи</span><span class="sxs-lookup"><span data-stu-id="a2243-110">Relationships</span></span>
| <span data-ttu-id="a2243-111">Связь</span><span class="sxs-lookup"><span data-stu-id="a2243-111">Relationship</span></span> | <span data-ttu-id="a2243-112">Тип</span><span class="sxs-lookup"><span data-stu-id="a2243-112">Type</span></span>   |<span data-ttu-id="a2243-113">Описание</span><span class="sxs-lookup"><span data-stu-id="a2243-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2243-114">fill</span><span class="sxs-lookup"><span data-stu-id="a2243-114">fill</span></span>|[<span data-ttu-id="a2243-115">воркбукчартфилл</span><span class="sxs-lookup"><span data-stu-id="a2243-115">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="a2243-p101">Представляет формат заливки ряда диаграммы, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a2243-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="a2243-118">line</span><span class="sxs-lookup"><span data-stu-id="a2243-118">line</span></span>|[<span data-ttu-id="a2243-119">воркбукчартлинеформат</span><span class="sxs-lookup"><span data-stu-id="a2243-119">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="a2243-120">Представляет форматирование линий.</span><span class="sxs-lookup"><span data-stu-id="a2243-120">Represents line formatting.</span></span> <span data-ttu-id="a2243-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a2243-121">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="a2243-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a2243-122">JSON representation</span></span>

<span data-ttu-id="a2243-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2243-123">Here is a JSON representation of the resource.</span></span>

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
