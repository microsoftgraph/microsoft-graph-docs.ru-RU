---
title: Тип ресурса ChartAxisFormat
description: Инкапсулирует свойства формата для оси диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 1d52063e63e179540bcbd5c3b4ec0cd09fb620d7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029857"
---
# <a name="chartaxisformat-resource-type"></a><span data-ttu-id="2480a-103">Тип ресурса ChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="2480a-103">ChartAxisFormat resource type</span></span>

<span data-ttu-id="2480a-104">Инкапсулирует свойства формата для оси диаграммы.</span><span class="sxs-lookup"><span data-stu-id="2480a-104">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="2480a-105">Методы</span><span class="sxs-lookup"><span data-stu-id="2480a-105">Methods</span></span>
<span data-ttu-id="2480a-106">Нет</span><span class="sxs-lookup"><span data-stu-id="2480a-106">None</span></span>
## <a name="properties"></a><span data-ttu-id="2480a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2480a-107">Properties</span></span>
<span data-ttu-id="2480a-108">Нет</span><span class="sxs-lookup"><span data-stu-id="2480a-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="2480a-109">Отношения</span><span class="sxs-lookup"><span data-stu-id="2480a-109">Relationships</span></span>
| <span data-ttu-id="2480a-110">Отношение</span><span class="sxs-lookup"><span data-stu-id="2480a-110">Relationship</span></span> | <span data-ttu-id="2480a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="2480a-111">Type</span></span>   |<span data-ttu-id="2480a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2480a-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2480a-113">font</span><span class="sxs-lookup"><span data-stu-id="2480a-113">font</span></span>|[<span data-ttu-id="2480a-114">Воркбукчартфонт</span><span class="sxs-lookup"><span data-stu-id="2480a-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="2480a-p101">Представляет атрибуты шрифта (имя, размер, цвет и т. д.) для элемента оси диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2480a-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="2480a-117">line</span><span class="sxs-lookup"><span data-stu-id="2480a-117">line</span></span>|[<span data-ttu-id="2480a-118">Воркбукчартлинеформат</span><span class="sxs-lookup"><span data-stu-id="2480a-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="2480a-119">Представляет форматирование линий диаграммы.</span><span class="sxs-lookup"><span data-stu-id="2480a-119">Represents chart line formatting.</span></span> <span data-ttu-id="2480a-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2480a-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="2480a-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2480a-121">JSON representation</span></span>

<span data-ttu-id="2480a-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2480a-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"},
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
