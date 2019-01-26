---
title: Тип ресурса ChartAxisTitleFormat
description: Представляет форматирование для названий осей диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: aeb39c46b349bda9f71385d13ef8e9ab17320823
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575921"
---
# <a name="chartaxistitleformat-resource-type"></a><span data-ttu-id="2834c-103">Тип ресурса ChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="2834c-103">ChartAxisTitleFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2834c-104">Представляет форматирование для названий осей диаграммы.</span><span class="sxs-lookup"><span data-stu-id="2834c-104">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="2834c-105">Методы</span><span class="sxs-lookup"><span data-stu-id="2834c-105">Methods</span></span>
<span data-ttu-id="2834c-106">Нет</span><span class="sxs-lookup"><span data-stu-id="2834c-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="2834c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2834c-107">Properties</span></span>
<span data-ttu-id="2834c-108">Нет</span><span class="sxs-lookup"><span data-stu-id="2834c-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="2834c-109">Связи</span><span class="sxs-lookup"><span data-stu-id="2834c-109">Relationships</span></span>
| <span data-ttu-id="2834c-110">Связь</span><span class="sxs-lookup"><span data-stu-id="2834c-110">Relationship</span></span> | <span data-ttu-id="2834c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="2834c-111">Type</span></span>   |<span data-ttu-id="2834c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2834c-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2834c-113">font</span><span class="sxs-lookup"><span data-stu-id="2834c-113">font</span></span>|[<span data-ttu-id="2834c-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="2834c-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="2834c-p101">Представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта названия оси диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2834c-p101">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2834c-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2834c-117">JSON representation</span></span>

<span data-ttu-id="2834c-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2834c-118">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxisTitleFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartaxistitleformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
