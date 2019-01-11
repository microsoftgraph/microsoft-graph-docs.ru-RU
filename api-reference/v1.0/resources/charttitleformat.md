---
title: Тип ресурса ChartTitleFormat
description: Инкапсулирует свойства формата для заголовка диаграммы.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: ee70eb991f2981a41de3e401a420a7fc0515d7c2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885549"
---
# <a name="charttitleformat-resource-type"></a><span data-ttu-id="ca4d2-103">Тип ресурса ChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="ca4d2-103">ChartTitleFormat resource type</span></span>

<span data-ttu-id="ca4d2-104">Инкапсулирует свойства формата для заголовка диаграммы.</span><span class="sxs-lookup"><span data-stu-id="ca4d2-104">Encapsulates the format properties for the chart title.</span></span>


## <a name="methods"></a><span data-ttu-id="ca4d2-105">Методы</span><span class="sxs-lookup"><span data-stu-id="ca4d2-105">Methods</span></span>
<span data-ttu-id="ca4d2-106">Нет</span><span class="sxs-lookup"><span data-stu-id="ca4d2-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="ca4d2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ca4d2-107">Properties</span></span>
<span data-ttu-id="ca4d2-108">Нет</span><span class="sxs-lookup"><span data-stu-id="ca4d2-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="ca4d2-109">Связи</span><span class="sxs-lookup"><span data-stu-id="ca4d2-109">Relationships</span></span>
| <span data-ttu-id="ca4d2-110">Связь</span><span class="sxs-lookup"><span data-stu-id="ca4d2-110">Relationship</span></span> | <span data-ttu-id="ca4d2-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ca4d2-111">Type</span></span>   |<span data-ttu-id="ca4d2-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ca4d2-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ca4d2-113">fill</span><span class="sxs-lookup"><span data-stu-id="ca4d2-113">fill</span></span>|[<span data-ttu-id="ca4d2-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="ca4d2-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="ca4d2-p101">Представляет формат заливки объекта, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ca4d2-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="ca4d2-117">font</span><span class="sxs-lookup"><span data-stu-id="ca4d2-117">font</span></span>|[<span data-ttu-id="ca4d2-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="ca4d2-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="ca4d2-p102">Представляет атрибуты шрифта (имя, размер, цвет и т. д.) для текущего объекта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ca4d2-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="ca4d2-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ca4d2-121">JSON representation</span></span>

<span data-ttu-id="ca4d2-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca4d2-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartTitleFormat"
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
  "description": "ChartAreaFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
