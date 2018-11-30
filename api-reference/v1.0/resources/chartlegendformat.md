---
title: Тип ресурса ChartLegendFormat
description: Инкапсулирует свойства формата для легенды диаграммы.
ms.openlocfilehash: a29fd6e54e0976c7b4a391c450809868fe45939c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028018"
---
# <a name="chartlegendformat-resource-type"></a><span data-ttu-id="9130f-103">Тип ресурса ChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="9130f-103">ChartLegendFormat resource type</span></span>

<span data-ttu-id="9130f-104">Инкапсулирует свойства формата для легенды диаграммы.</span><span class="sxs-lookup"><span data-stu-id="9130f-104">Encapsulates the format properties of a chart legend.</span></span>


## <a name="methods"></a><span data-ttu-id="9130f-105">Методы</span><span class="sxs-lookup"><span data-stu-id="9130f-105">Methods</span></span>
<span data-ttu-id="9130f-106">Нет</span><span class="sxs-lookup"><span data-stu-id="9130f-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="9130f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9130f-107">Properties</span></span>
<span data-ttu-id="9130f-108">Нет</span><span class="sxs-lookup"><span data-stu-id="9130f-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="9130f-109">Связи</span><span class="sxs-lookup"><span data-stu-id="9130f-109">Relationships</span></span>
| <span data-ttu-id="9130f-110">Связь</span><span class="sxs-lookup"><span data-stu-id="9130f-110">Relationship</span></span> | <span data-ttu-id="9130f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="9130f-111">Type</span></span>   |<span data-ttu-id="9130f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="9130f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9130f-113">fill</span><span class="sxs-lookup"><span data-stu-id="9130f-113">fill</span></span>|[<span data-ttu-id="9130f-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="9130f-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="9130f-p101">Представляет формат заливки объекта, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9130f-p101">Represents the fill format of an object, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="9130f-117">шрифт</span><span class="sxs-lookup"><span data-stu-id="9130f-117">font</span></span>|[<span data-ttu-id="9130f-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="9130f-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="9130f-p102">Представляет атрибуты шрифта (название, размер, цвет и т. д.) легенды диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9130f-p102">Represents the font attributes such as font name, font size, color, etc. of a chart legend. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="9130f-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9130f-121">JSON representation</span></span>

<span data-ttu-id="9130f-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9130f-122">Here is a JSON representation of the resource.</span></span>

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