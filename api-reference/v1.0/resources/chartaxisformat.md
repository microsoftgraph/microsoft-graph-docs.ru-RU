---
title: Тип ресурса ChartAxisFormat
description: Инкапсулирует свойства формата для оси диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 92258887c9646890ee63d14aebcd32ada7a8aaa6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569251"
---
# <a name="chartaxisformat-resource-type"></a><span data-ttu-id="424cb-103">Тип ресурса ChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="424cb-103">ChartAxisFormat resource type</span></span>

<span data-ttu-id="424cb-104">Инкапсулирует свойства формата для оси диаграммы.</span><span class="sxs-lookup"><span data-stu-id="424cb-104">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="424cb-105">Методы</span><span class="sxs-lookup"><span data-stu-id="424cb-105">Methods</span></span>
<span data-ttu-id="424cb-106">Нет</span><span class="sxs-lookup"><span data-stu-id="424cb-106">None</span></span>
## <a name="properties"></a><span data-ttu-id="424cb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="424cb-107">Properties</span></span>
<span data-ttu-id="424cb-108">Нет</span><span class="sxs-lookup"><span data-stu-id="424cb-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="424cb-109">Связи</span><span class="sxs-lookup"><span data-stu-id="424cb-109">Relationships</span></span>
| <span data-ttu-id="424cb-110">Отношение</span><span class="sxs-lookup"><span data-stu-id="424cb-110">Relationship</span></span> | <span data-ttu-id="424cb-111">Тип</span><span class="sxs-lookup"><span data-stu-id="424cb-111">Type</span></span>   |<span data-ttu-id="424cb-112">Описание</span><span class="sxs-lookup"><span data-stu-id="424cb-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="424cb-113">font</span><span class="sxs-lookup"><span data-stu-id="424cb-113">font</span></span>|[<span data-ttu-id="424cb-114">Воркбукчартфонт</span><span class="sxs-lookup"><span data-stu-id="424cb-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="424cb-p101">Представляет атрибуты шрифта (имя, размер, цвет и т. д.) для элемента оси диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="424cb-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="424cb-117">line</span><span class="sxs-lookup"><span data-stu-id="424cb-117">line</span></span>|[<span data-ttu-id="424cb-118">Воркбукчартлинеформат</span><span class="sxs-lookup"><span data-stu-id="424cb-118">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="424cb-119">Представляет форматирование линий диаграммы.</span><span class="sxs-lookup"><span data-stu-id="424cb-119">Represents chart line formatting.</span></span> <span data-ttu-id="424cb-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="424cb-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="424cb-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="424cb-121">JSON representation</span></span>

<span data-ttu-id="424cb-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="424cb-122">Here is a JSON representation of the resource.</span></span>

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
