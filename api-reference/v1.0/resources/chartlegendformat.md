---
title: Тип ресурса ChartLegendFormat
description: Инкапсулирует свойства формата для легенды диаграммы.
author: lumine2008
ms.openlocfilehash: 6ef6f2d26ade1d8d93489fbc560d4e0eb511bc86
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334379"
---
# <a name="chartlegendformat-resource-type"></a><span data-ttu-id="d9998-103">Тип ресурса ChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="d9998-103">ChartLegendFormat resource type</span></span>

<span data-ttu-id="d9998-104">Инкапсулирует свойства формата для легенды диаграммы.</span><span class="sxs-lookup"><span data-stu-id="d9998-104">Encapsulates the format properties of a chart legend.</span></span>


## <a name="methods"></a><span data-ttu-id="d9998-105">Методы</span><span class="sxs-lookup"><span data-stu-id="d9998-105">Methods</span></span>
<span data-ttu-id="d9998-106">Нет</span><span class="sxs-lookup"><span data-stu-id="d9998-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="d9998-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d9998-107">Properties</span></span>
<span data-ttu-id="d9998-108">Нет</span><span class="sxs-lookup"><span data-stu-id="d9998-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="d9998-109">Связи</span><span class="sxs-lookup"><span data-stu-id="d9998-109">Relationships</span></span>
| <span data-ttu-id="d9998-110">Связь</span><span class="sxs-lookup"><span data-stu-id="d9998-110">Relationship</span></span> | <span data-ttu-id="d9998-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d9998-111">Type</span></span>   |<span data-ttu-id="d9998-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d9998-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d9998-113">fill</span><span class="sxs-lookup"><span data-stu-id="d9998-113">fill</span></span>|[<span data-ttu-id="d9998-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="d9998-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="d9998-p101">Представляет формат заливки объекта, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d9998-p101">Represents the fill format of an object, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="d9998-117">шрифт</span><span class="sxs-lookup"><span data-stu-id="d9998-117">font</span></span>|[<span data-ttu-id="d9998-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="d9998-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="d9998-p102">Представляет атрибуты шрифта (название, размер, цвет и т. д.) легенды диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d9998-p102">Represents the font attributes such as font name, font size, color, etc. of a chart legend. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="d9998-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d9998-121">JSON representation</span></span>

<span data-ttu-id="d9998-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9998-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartLegendFormat"
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
  "description": "ChartLegendFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->