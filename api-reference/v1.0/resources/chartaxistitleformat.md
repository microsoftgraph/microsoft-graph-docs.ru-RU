---
title: Тип ресурса ChartAxisTitleFormat
description: Представляет форматирование для названий осей диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 26d305d8bd4a0059123f77bd86cbbf5fd01dcea7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959484"
---
# <a name="chartaxistitleformat-resource-type"></a><span data-ttu-id="cd398-103">Тип ресурса ChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="cd398-103">ChartAxisTitleFormat resource type</span></span>

<span data-ttu-id="cd398-104">Представляет форматирование для названий осей диаграммы.</span><span class="sxs-lookup"><span data-stu-id="cd398-104">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="cd398-105">Методы</span><span class="sxs-lookup"><span data-stu-id="cd398-105">Methods</span></span>
<span data-ttu-id="cd398-106">Нет</span><span class="sxs-lookup"><span data-stu-id="cd398-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="cd398-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="cd398-107">Properties</span></span>
<span data-ttu-id="cd398-108">Нет</span><span class="sxs-lookup"><span data-stu-id="cd398-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="cd398-109">Связи</span><span class="sxs-lookup"><span data-stu-id="cd398-109">Relationships</span></span>
| <span data-ttu-id="cd398-110">Связь</span><span class="sxs-lookup"><span data-stu-id="cd398-110">Relationship</span></span> | <span data-ttu-id="cd398-111">Тип</span><span class="sxs-lookup"><span data-stu-id="cd398-111">Type</span></span>   |<span data-ttu-id="cd398-112">Описание</span><span class="sxs-lookup"><span data-stu-id="cd398-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd398-113">font</span><span class="sxs-lookup"><span data-stu-id="cd398-113">font</span></span>|[<span data-ttu-id="cd398-114">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="cd398-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="cd398-p101">Представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта названия оси диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cd398-p101">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cd398-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cd398-117">JSON representation</span></span>

<span data-ttu-id="cd398-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd398-118">Here is a JSON representation of the resource.</span></span>

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
