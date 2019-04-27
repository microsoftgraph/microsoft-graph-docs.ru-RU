---
title: Тип ресурса Воркбукчартаксисформат
description: Инкапсулирует свойства формата для оси диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 8c152971dde5efb188cfde30c30b54a1266b44fb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348944"
---
# <a name="workbookchartaxisformat-resource-type"></a><span data-ttu-id="72961-103">Тип ресурса Воркбукчартаксисформат</span><span class="sxs-lookup"><span data-stu-id="72961-103">workbookChartAxisFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72961-104">Инкапсулирует свойства формата для оси диаграммы.</span><span class="sxs-lookup"><span data-stu-id="72961-104">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="72961-105">Методы</span><span class="sxs-lookup"><span data-stu-id="72961-105">Methods</span></span>
<span data-ttu-id="72961-106">Отсутствует</span><span class="sxs-lookup"><span data-stu-id="72961-106">None</span></span>
## <a name="properties"></a><span data-ttu-id="72961-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="72961-107">Properties</span></span>
<span data-ttu-id="72961-108">Нет</span><span class="sxs-lookup"><span data-stu-id="72961-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="72961-109">Отношения</span><span class="sxs-lookup"><span data-stu-id="72961-109">Relationships</span></span>
| <span data-ttu-id="72961-110">Отношение</span><span class="sxs-lookup"><span data-stu-id="72961-110">Relationship</span></span> | <span data-ttu-id="72961-111">Тип</span><span class="sxs-lookup"><span data-stu-id="72961-111">Type</span></span>   |<span data-ttu-id="72961-112">Описание</span><span class="sxs-lookup"><span data-stu-id="72961-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72961-113">font</span><span class="sxs-lookup"><span data-stu-id="72961-113">font</span></span>|[<span data-ttu-id="72961-114">Воркбукчартфонт</span><span class="sxs-lookup"><span data-stu-id="72961-114">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="72961-p101">Представляет атрибуты шрифта (имя, размер, цвет и т. д.) для элемента оси диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72961-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="72961-117">line</span><span class="sxs-lookup"><span data-stu-id="72961-117">line</span></span>|[<span data-ttu-id="72961-118">Воркбукчартлинеформат</span><span class="sxs-lookup"><span data-stu-id="72961-118">workbookChartLineFormat</span></span>](workbookchartlineformat.md)|<span data-ttu-id="72961-119">Представляет форматирование линий диаграммы.</span><span class="sxs-lookup"><span data-stu-id="72961-119">Represents chart line formatting.</span></span> <span data-ttu-id="72961-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72961-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="72961-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="72961-121">JSON representation</span></span>

<span data-ttu-id="72961-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72961-122">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxisFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
