---
title: Тип ресурса ChartAxisTitleFormat
description: Представляет форматирование для названий осей диаграммы.
author: lumine2008
ms.openlocfilehash: 7a160f02f06c74edeee09f91b2b117ea437291e8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343024"
---
# <a name="chartaxistitleformat-resource-type"></a><span data-ttu-id="86c8a-103">Тип ресурса ChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="86c8a-103">ChartAxisTitleFormat resource type</span></span>

<span data-ttu-id="86c8a-104">Представляет форматирование для названий осей диаграммы.</span><span class="sxs-lookup"><span data-stu-id="86c8a-104">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="86c8a-105">Методы</span><span class="sxs-lookup"><span data-stu-id="86c8a-105">Methods</span></span>
<span data-ttu-id="86c8a-106">Нет</span><span class="sxs-lookup"><span data-stu-id="86c8a-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="86c8a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="86c8a-107">Properties</span></span>
<span data-ttu-id="86c8a-108">Нет</span><span class="sxs-lookup"><span data-stu-id="86c8a-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="86c8a-109">Связи</span><span class="sxs-lookup"><span data-stu-id="86c8a-109">Relationships</span></span>
| <span data-ttu-id="86c8a-110">Связь</span><span class="sxs-lookup"><span data-stu-id="86c8a-110">Relationship</span></span> | <span data-ttu-id="86c8a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="86c8a-111">Type</span></span>   |<span data-ttu-id="86c8a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="86c8a-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86c8a-113">font</span><span class="sxs-lookup"><span data-stu-id="86c8a-113">font</span></span>|[<span data-ttu-id="86c8a-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="86c8a-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="86c8a-p101">Представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта названия оси диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="86c8a-p101">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="86c8a-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="86c8a-117">JSON representation</span></span>

<span data-ttu-id="86c8a-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="86c8a-118">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisTitleFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitleFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->