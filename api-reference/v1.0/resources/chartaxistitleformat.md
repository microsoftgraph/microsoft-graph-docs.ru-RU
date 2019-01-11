---
title: Тип ресурса ChartAxisTitleFormat
description: Представляет форматирование для названий осей диаграммы.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 4aa96f0a346d8b08832464097b258a92b1db44df
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840315"
---
# <a name="chartaxistitleformat-resource-type"></a><span data-ttu-id="4b6d9-103">Тип ресурса ChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="4b6d9-103">ChartAxisTitleFormat resource type</span></span>

<span data-ttu-id="4b6d9-104">Представляет форматирование для названий осей диаграммы.</span><span class="sxs-lookup"><span data-stu-id="4b6d9-104">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="4b6d9-105">Методы</span><span class="sxs-lookup"><span data-stu-id="4b6d9-105">Methods</span></span>
<span data-ttu-id="4b6d9-106">Нет</span><span class="sxs-lookup"><span data-stu-id="4b6d9-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="4b6d9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4b6d9-107">Properties</span></span>
<span data-ttu-id="4b6d9-108">Нет</span><span class="sxs-lookup"><span data-stu-id="4b6d9-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="4b6d9-109">Связи</span><span class="sxs-lookup"><span data-stu-id="4b6d9-109">Relationships</span></span>
| <span data-ttu-id="4b6d9-110">Связь</span><span class="sxs-lookup"><span data-stu-id="4b6d9-110">Relationship</span></span> | <span data-ttu-id="4b6d9-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4b6d9-111">Type</span></span>   |<span data-ttu-id="4b6d9-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4b6d9-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b6d9-113">font</span><span class="sxs-lookup"><span data-stu-id="4b6d9-113">font</span></span>|[<span data-ttu-id="4b6d9-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="4b6d9-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="4b6d9-p101">Представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта названия оси диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4b6d9-p101">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4b6d9-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4b6d9-117">JSON representation</span></span>

<span data-ttu-id="4b6d9-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b6d9-118">Here is a JSON representation of the resource.</span></span>

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
