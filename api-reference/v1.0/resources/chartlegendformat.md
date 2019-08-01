---
title: Тип ресурса ChartLegendFormat
description: Инкапсулирует свойства формата легенды диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 2148b6b5baf8bb680f85954d000da097bcf8f0b9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032958"
---
# <a name="chartlegendformat-resource-type"></a><span data-ttu-id="e9e03-103">Тип ресурса ChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="e9e03-103">ChartLegendFormat resource type</span></span>

<span data-ttu-id="e9e03-104">Инкапсулирует свойства формата легенды диаграммы.</span><span class="sxs-lookup"><span data-stu-id="e9e03-104">Encapsulates the format properties of a chart legend.</span></span>


## <a name="methods"></a><span data-ttu-id="e9e03-105">Методы</span><span class="sxs-lookup"><span data-stu-id="e9e03-105">Methods</span></span>
<span data-ttu-id="e9e03-106">Нет</span><span class="sxs-lookup"><span data-stu-id="e9e03-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="e9e03-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e9e03-107">Properties</span></span>
<span data-ttu-id="e9e03-108">Нет</span><span class="sxs-lookup"><span data-stu-id="e9e03-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="e9e03-109">Отношения</span><span class="sxs-lookup"><span data-stu-id="e9e03-109">Relationships</span></span>
| <span data-ttu-id="e9e03-110">Отношение</span><span class="sxs-lookup"><span data-stu-id="e9e03-110">Relationship</span></span> | <span data-ttu-id="e9e03-111">Тип</span><span class="sxs-lookup"><span data-stu-id="e9e03-111">Type</span></span>   |<span data-ttu-id="e9e03-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e9e03-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9e03-113">fill</span><span class="sxs-lookup"><span data-stu-id="e9e03-113">fill</span></span>|[<span data-ttu-id="e9e03-114">Воркбукчартфилл</span><span class="sxs-lookup"><span data-stu-id="e9e03-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="e9e03-p101">Представляет формат заливки объекта, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e9e03-p101">Represents the fill format of an object, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="e9e03-117">шрифт</span><span class="sxs-lookup"><span data-stu-id="e9e03-117">font</span></span>|[<span data-ttu-id="e9e03-118">Воркбукчартфонт</span><span class="sxs-lookup"><span data-stu-id="e9e03-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="e9e03-119">Представляет атрибуты шрифта, такие как имя шрифта, размер шрифта, цвет и т. д., в условных обозначениях диаграммы.</span><span class="sxs-lookup"><span data-stu-id="e9e03-119">Represents the font attributes such as font name, font size, color, etc. of a chart legend.</span></span> <span data-ttu-id="e9e03-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e9e03-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e9e03-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e9e03-121">JSON representation</span></span>

<span data-ttu-id="e9e03-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9e03-122">Here is a JSON representation of the resource.</span></span>

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
