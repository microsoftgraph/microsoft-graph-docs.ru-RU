---
title: Тип ресурса ChartPointFormat
description: Представляет объект форматирования для точек диаграммы.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 5923252a9fce47eedc58751def301b6515560ddd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883344"
---
# <a name="chartpointformat-resource-type"></a><span data-ttu-id="b655d-103">Тип ресурса ChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="b655d-103">ChartPointFormat resource type</span></span>

<span data-ttu-id="b655d-104">Представляет объект форматирования для точек диаграммы.</span><span class="sxs-lookup"><span data-stu-id="b655d-104">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="b655d-105">Методы</span><span class="sxs-lookup"><span data-stu-id="b655d-105">Methods</span></span>
<span data-ttu-id="b655d-106">Нет</span><span class="sxs-lookup"><span data-stu-id="b655d-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="b655d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b655d-107">Properties</span></span>
<span data-ttu-id="b655d-108">Нет</span><span class="sxs-lookup"><span data-stu-id="b655d-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="b655d-109">Связи</span><span class="sxs-lookup"><span data-stu-id="b655d-109">Relationships</span></span>
| <span data-ttu-id="b655d-110">Связь</span><span class="sxs-lookup"><span data-stu-id="b655d-110">Relationship</span></span> | <span data-ttu-id="b655d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="b655d-111">Type</span></span>   |<span data-ttu-id="b655d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b655d-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b655d-113">fill</span><span class="sxs-lookup"><span data-stu-id="b655d-113">fill</span></span>|[<span data-ttu-id="b655d-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="b655d-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="b655d-p101">Представляет формат заливки диаграммы, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b655d-p101">Represents the fill format of a chart, which includes background formating information. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b655d-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b655d-117">JSON representation</span></span>

<span data-ttu-id="b655d-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b655d-118">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPointFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPointFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
