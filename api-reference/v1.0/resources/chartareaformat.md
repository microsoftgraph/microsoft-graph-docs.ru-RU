---
title: Тип ресурса ChartAreaFormat
description: Инкапсулирует свойства формата для всей области диаграммы.
author: lumine2008
ms.openlocfilehash: d9db44fefeff00ae6f7363126de35d4028964d14
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310005"
---
# <a name="chartareaformat-resource-type"></a><span data-ttu-id="60a5e-103">Тип ресурса ChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="60a5e-103">ChartAreaFormat resource type</span></span>

<span data-ttu-id="60a5e-104">Инкапсулирует свойства формата для всей области диаграммы.</span><span class="sxs-lookup"><span data-stu-id="60a5e-104">Encapsulates the format properties for the overall chart area.</span></span>


## <a name="methods"></a><span data-ttu-id="60a5e-105">Методы</span><span class="sxs-lookup"><span data-stu-id="60a5e-105">Methods</span></span>
<span data-ttu-id="60a5e-106">Нет</span><span class="sxs-lookup"><span data-stu-id="60a5e-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="60a5e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="60a5e-107">Properties</span></span>
<span data-ttu-id="60a5e-108">Нет</span><span class="sxs-lookup"><span data-stu-id="60a5e-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="60a5e-109">Связи</span><span class="sxs-lookup"><span data-stu-id="60a5e-109">Relationships</span></span>
| <span data-ttu-id="60a5e-110">Связь</span><span class="sxs-lookup"><span data-stu-id="60a5e-110">Relationship</span></span> | <span data-ttu-id="60a5e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="60a5e-111">Type</span></span>   |<span data-ttu-id="60a5e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="60a5e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60a5e-113">fill</span><span class="sxs-lookup"><span data-stu-id="60a5e-113">fill</span></span>|[<span data-ttu-id="60a5e-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="60a5e-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="60a5e-p101">Представляет формат заливки объекта, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="60a5e-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="60a5e-117">font</span><span class="sxs-lookup"><span data-stu-id="60a5e-117">font</span></span>|[<span data-ttu-id="60a5e-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="60a5e-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="60a5e-p102">Представляет атрибуты шрифта (имя, размер, цвет и т. д.) для текущего объекта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="60a5e-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="60a5e-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="60a5e-121">JSON representation</span></span>

<span data-ttu-id="60a5e-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60a5e-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAreaFormat"
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