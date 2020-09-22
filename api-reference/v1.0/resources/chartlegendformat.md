---
title: Тип ресурса ChartLegendFormat
description: Инкапсулирует свойства формата легенды диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: f4d018fd01a9ad9899eefcb663b0860096567c84
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988395"
---
# <a name="chartlegendformat-resource-type"></a><span data-ttu-id="3f185-103">Тип ресурса ChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="3f185-103">ChartLegendFormat resource type</span></span>

<span data-ttu-id="3f185-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f185-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3f185-105">Инкапсулирует свойства формата легенды диаграммы.</span><span class="sxs-lookup"><span data-stu-id="3f185-105">Encapsulates the format properties of a chart legend.</span></span>


## <a name="methods"></a><span data-ttu-id="3f185-106">Методы</span><span class="sxs-lookup"><span data-stu-id="3f185-106">Methods</span></span>
<span data-ttu-id="3f185-107">Нет</span><span class="sxs-lookup"><span data-stu-id="3f185-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="3f185-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3f185-108">Properties</span></span>
<span data-ttu-id="3f185-109">Нет</span><span class="sxs-lookup"><span data-stu-id="3f185-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="3f185-110">Связи</span><span class="sxs-lookup"><span data-stu-id="3f185-110">Relationships</span></span>
| <span data-ttu-id="3f185-111">Связь</span><span class="sxs-lookup"><span data-stu-id="3f185-111">Relationship</span></span> | <span data-ttu-id="3f185-112">Тип</span><span class="sxs-lookup"><span data-stu-id="3f185-112">Type</span></span>   |<span data-ttu-id="3f185-113">Описание</span><span class="sxs-lookup"><span data-stu-id="3f185-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f185-114">fill</span><span class="sxs-lookup"><span data-stu-id="3f185-114">fill</span></span>|[<span data-ttu-id="3f185-115">воркбукчартфилл</span><span class="sxs-lookup"><span data-stu-id="3f185-115">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="3f185-p101">Представляет формат заливки объекта, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3f185-p101">Represents the fill format of an object, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="3f185-118">шрифт</span><span class="sxs-lookup"><span data-stu-id="3f185-118">font</span></span>|[<span data-ttu-id="3f185-119">воркбукчартфонт</span><span class="sxs-lookup"><span data-stu-id="3f185-119">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="3f185-120">Представляет атрибуты шрифта, такие как имя шрифта, размер шрифта, цвет и т. д., в условных обозначениях диаграммы.</span><span class="sxs-lookup"><span data-stu-id="3f185-120">Represents the font attributes such as font name, font size, color, etc. of a chart legend.</span></span> <span data-ttu-id="3f185-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3f185-121">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="3f185-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3f185-122">JSON representation</span></span>

<span data-ttu-id="3f185-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f185-123">Here is a JSON representation of the resource.</span></span>

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

