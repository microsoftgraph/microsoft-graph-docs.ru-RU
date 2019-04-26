---
title: Тип ресурса ChartLegendFormat
description: Инкапсулирует свойства формата легенды диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f35f7a3cf152024bd89f03daf8be98ec1d8066b0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569097"
---
# <a name="chartlegendformat-resource-type"></a><span data-ttu-id="7cf43-103">Тип ресурса ChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="7cf43-103">ChartLegendFormat resource type</span></span>

<span data-ttu-id="7cf43-104">Инкапсулирует свойства формата легенды диаграммы.</span><span class="sxs-lookup"><span data-stu-id="7cf43-104">Encapsulates the format properties of a chart legend.</span></span>


## <a name="methods"></a><span data-ttu-id="7cf43-105">Методы</span><span class="sxs-lookup"><span data-stu-id="7cf43-105">Methods</span></span>
<span data-ttu-id="7cf43-106">Нет</span><span class="sxs-lookup"><span data-stu-id="7cf43-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="7cf43-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7cf43-107">Properties</span></span>
<span data-ttu-id="7cf43-108">Нет</span><span class="sxs-lookup"><span data-stu-id="7cf43-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="7cf43-109">Связи</span><span class="sxs-lookup"><span data-stu-id="7cf43-109">Relationships</span></span>
| <span data-ttu-id="7cf43-110">Отношение</span><span class="sxs-lookup"><span data-stu-id="7cf43-110">Relationship</span></span> | <span data-ttu-id="7cf43-111">Тип</span><span class="sxs-lookup"><span data-stu-id="7cf43-111">Type</span></span>   |<span data-ttu-id="7cf43-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7cf43-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7cf43-113">fill</span><span class="sxs-lookup"><span data-stu-id="7cf43-113">fill</span></span>|[<span data-ttu-id="7cf43-114">Воркбукчартфилл</span><span class="sxs-lookup"><span data-stu-id="7cf43-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="7cf43-p101">Представляет формат заливки объекта, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7cf43-p101">Represents the fill format of an object, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="7cf43-117">шрифт</span><span class="sxs-lookup"><span data-stu-id="7cf43-117">font</span></span>|[<span data-ttu-id="7cf43-118">Воркбукчартфонт</span><span class="sxs-lookup"><span data-stu-id="7cf43-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="7cf43-119">Представляет атрибуты шрифта, такие как имя шрифта, размер шрифта, цвет и т. д., в условных обозначениях диаграммы.</span><span class="sxs-lookup"><span data-stu-id="7cf43-119">Represents the font attributes such as font name, font size, color, etc. of a chart legend.</span></span> <span data-ttu-id="7cf43-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7cf43-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="7cf43-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7cf43-121">JSON representation</span></span>

<span data-ttu-id="7cf43-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7cf43-122">Here is a JSON representation of the resource.</span></span>

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
