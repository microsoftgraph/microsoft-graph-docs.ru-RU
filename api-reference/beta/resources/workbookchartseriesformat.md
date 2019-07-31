---
title: Тип ресурса Воркбукчартсериесформат
description: Инкапсулирует свойства формата для ряда диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 739a874545047c2ed6927cb4e31d2e006f4e6ba4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007167"
---
# <a name="workbookchartseriesformat-resource-type"></a><span data-ttu-id="81a66-103">Тип ресурса Воркбукчартсериесформат</span><span class="sxs-lookup"><span data-stu-id="81a66-103">workbookChartSeriesFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81a66-104">Инкапсулирует свойства формата для ряда диаграммы.</span><span class="sxs-lookup"><span data-stu-id="81a66-104">Encapsulates the format properties for the chart series.</span></span>


## <a name="methods"></a><span data-ttu-id="81a66-105">Методы</span><span class="sxs-lookup"><span data-stu-id="81a66-105">Methods</span></span>
<span data-ttu-id="81a66-106">Нет</span><span class="sxs-lookup"><span data-stu-id="81a66-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="81a66-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="81a66-107">Properties</span></span>
<span data-ttu-id="81a66-108">Нет</span><span class="sxs-lookup"><span data-stu-id="81a66-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="81a66-109">Отношения</span><span class="sxs-lookup"><span data-stu-id="81a66-109">Relationships</span></span>
| <span data-ttu-id="81a66-110">Отношение</span><span class="sxs-lookup"><span data-stu-id="81a66-110">Relationship</span></span> | <span data-ttu-id="81a66-111">Тип</span><span class="sxs-lookup"><span data-stu-id="81a66-111">Type</span></span>   |<span data-ttu-id="81a66-112">Описание</span><span class="sxs-lookup"><span data-stu-id="81a66-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81a66-113">fill</span><span class="sxs-lookup"><span data-stu-id="81a66-113">fill</span></span>|[<span data-ttu-id="81a66-114">Воркбукчартфилл</span><span class="sxs-lookup"><span data-stu-id="81a66-114">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="81a66-p101">Представляет формат заливки ряда диаграммы, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81a66-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="81a66-117">line</span><span class="sxs-lookup"><span data-stu-id="81a66-117">line</span></span>|[<span data-ttu-id="81a66-118">Воркбукчартлинеформат</span><span class="sxs-lookup"><span data-stu-id="81a66-118">workbookChartLineFormat</span></span>](workbookchartlineformat.md)|<span data-ttu-id="81a66-119">Представляет форматирование линий.</span><span class="sxs-lookup"><span data-stu-id="81a66-119">Represents line formatting.</span></span> <span data-ttu-id="81a66-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="81a66-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="81a66-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="81a66-121">JSON representation</span></span>

<span data-ttu-id="81a66-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="81a66-122">Here is a JSON representation of the resource.</span></span>

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
