---
title: Тип ресурса ChartLegendFormat
description: Инкапсулирует свойства формата легенды диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: d3d7d9a0a74a56a6e0ae99aa7431779dc7164265
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531846"
---
# <a name="chartlegendformat-resource-type"></a><span data-ttu-id="893c9-103">Тип ресурса ChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="893c9-103">ChartLegendFormat resource type</span></span>

<span data-ttu-id="893c9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="893c9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="893c9-105">Инкапсулирует свойства формата легенды диаграммы.</span><span class="sxs-lookup"><span data-stu-id="893c9-105">Encapsulates the format properties of a chart legend.</span></span>


## <a name="methods"></a><span data-ttu-id="893c9-106">Methods</span><span class="sxs-lookup"><span data-stu-id="893c9-106">Methods</span></span>
<span data-ttu-id="893c9-107">Нет</span><span class="sxs-lookup"><span data-stu-id="893c9-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="893c9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="893c9-108">Properties</span></span>
<span data-ttu-id="893c9-109">Нет</span><span class="sxs-lookup"><span data-stu-id="893c9-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="893c9-110">Связи</span><span class="sxs-lookup"><span data-stu-id="893c9-110">Relationships</span></span>
| <span data-ttu-id="893c9-111">Связь</span><span class="sxs-lookup"><span data-stu-id="893c9-111">Relationship</span></span> | <span data-ttu-id="893c9-112">Тип</span><span class="sxs-lookup"><span data-stu-id="893c9-112">Type</span></span>   |<span data-ttu-id="893c9-113">Описание</span><span class="sxs-lookup"><span data-stu-id="893c9-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="893c9-114">fill</span><span class="sxs-lookup"><span data-stu-id="893c9-114">fill</span></span>|[<span data-ttu-id="893c9-115">воркбукчартфилл</span><span class="sxs-lookup"><span data-stu-id="893c9-115">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="893c9-p101">Представляет формат заливки объекта, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="893c9-p101">Represents the fill format of an object, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="893c9-118">шрифт</span><span class="sxs-lookup"><span data-stu-id="893c9-118">font</span></span>|[<span data-ttu-id="893c9-119">воркбукчартфонт</span><span class="sxs-lookup"><span data-stu-id="893c9-119">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="893c9-120">Представляет атрибуты шрифта, такие как имя шрифта, размер шрифта, цвет и т. д., в условных обозначениях диаграммы.</span><span class="sxs-lookup"><span data-stu-id="893c9-120">Represents the font attributes such as font name, font size, color, etc. of a chart legend.</span></span> <span data-ttu-id="893c9-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="893c9-121">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="893c9-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="893c9-122">JSON representation</span></span>

<span data-ttu-id="893c9-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="893c9-123">Here is a JSON representation of the resource.</span></span>

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
