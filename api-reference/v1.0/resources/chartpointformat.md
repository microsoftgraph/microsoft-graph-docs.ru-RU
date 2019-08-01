---
title: Тип ресурса ChartPointFormat
description: Представляет объект форматирования для точек диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: b17eb84c3de5505a3dfea23ce3fef564dca9aa2b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029766"
---
# <a name="chartpointformat-resource-type"></a><span data-ttu-id="feb42-103">Тип ресурса ChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="feb42-103">ChartPointFormat resource type</span></span>

<span data-ttu-id="feb42-104">Представляет объект форматирования для точек диаграммы.</span><span class="sxs-lookup"><span data-stu-id="feb42-104">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="feb42-105">Методы</span><span class="sxs-lookup"><span data-stu-id="feb42-105">Methods</span></span>
<span data-ttu-id="feb42-106">Нет</span><span class="sxs-lookup"><span data-stu-id="feb42-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="feb42-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="feb42-107">Properties</span></span>
<span data-ttu-id="feb42-108">Нет</span><span class="sxs-lookup"><span data-stu-id="feb42-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="feb42-109">Отношения</span><span class="sxs-lookup"><span data-stu-id="feb42-109">Relationships</span></span>
| <span data-ttu-id="feb42-110">Отношение</span><span class="sxs-lookup"><span data-stu-id="feb42-110">Relationship</span></span> | <span data-ttu-id="feb42-111">Тип</span><span class="sxs-lookup"><span data-stu-id="feb42-111">Type</span></span>   |<span data-ttu-id="feb42-112">Описание</span><span class="sxs-lookup"><span data-stu-id="feb42-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="feb42-113">fill</span><span class="sxs-lookup"><span data-stu-id="feb42-113">fill</span></span>|[<span data-ttu-id="feb42-114">Воркбукчартфилл</span><span class="sxs-lookup"><span data-stu-id="feb42-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="feb42-115">Представляет формат заливки диаграммы, включая сведения о форматировании фона.</span><span class="sxs-lookup"><span data-stu-id="feb42-115">Represents the fill format of a chart, which includes background formating information.</span></span> <span data-ttu-id="feb42-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="feb42-116">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="feb42-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="feb42-117">JSON representation</span></span>

<span data-ttu-id="feb42-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="feb42-118">Here is a JSON representation of the resource.</span></span>

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
