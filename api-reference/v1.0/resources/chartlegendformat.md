---
title: Тип ресурса ChartLegendFormat
description: Инкапсулирует свойства формата для легенды диаграммы.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 7d57ad66da6e5f280684cf364ac7890bcc3ed259
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811069"
---
# <a name="chartlegendformat-resource-type"></a><span data-ttu-id="ae276-103">Тип ресурса ChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="ae276-103">ChartLegendFormat resource type</span></span>

<span data-ttu-id="ae276-104">Инкапсулирует свойства формата для легенды диаграммы.</span><span class="sxs-lookup"><span data-stu-id="ae276-104">Encapsulates the format properties of a chart legend.</span></span>


## <a name="methods"></a><span data-ttu-id="ae276-105">Методы</span><span class="sxs-lookup"><span data-stu-id="ae276-105">Methods</span></span>
<span data-ttu-id="ae276-106">Нет</span><span class="sxs-lookup"><span data-stu-id="ae276-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="ae276-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ae276-107">Properties</span></span>
<span data-ttu-id="ae276-108">Нет</span><span class="sxs-lookup"><span data-stu-id="ae276-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="ae276-109">Связи</span><span class="sxs-lookup"><span data-stu-id="ae276-109">Relationships</span></span>
| <span data-ttu-id="ae276-110">Связь</span><span class="sxs-lookup"><span data-stu-id="ae276-110">Relationship</span></span> | <span data-ttu-id="ae276-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ae276-111">Type</span></span>   |<span data-ttu-id="ae276-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ae276-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae276-113">fill</span><span class="sxs-lookup"><span data-stu-id="ae276-113">fill</span></span>|[<span data-ttu-id="ae276-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="ae276-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="ae276-p101">Представляет формат заливки объекта, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ae276-p101">Represents the fill format of an object, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="ae276-117">шрифт</span><span class="sxs-lookup"><span data-stu-id="ae276-117">font</span></span>|[<span data-ttu-id="ae276-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="ae276-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="ae276-p102">Представляет атрибуты шрифта (название, размер, цвет и т. д.) легенды диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ae276-p102">Represents the font attributes such as font name, font size, color, etc. of a chart legend. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="ae276-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ae276-121">JSON representation</span></span>

<span data-ttu-id="ae276-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae276-122">Here is a JSON representation of the resource.</span></span>

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
