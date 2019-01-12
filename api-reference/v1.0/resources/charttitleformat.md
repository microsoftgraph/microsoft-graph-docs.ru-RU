---
title: Тип ресурса ChartTitleFormat
description: Инкапсулирует свойства формата для заголовка диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3a2c16d37d2ca86d7cafbb4047ee0bcea1ee4bde
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977117"
---
# <a name="charttitleformat-resource-type"></a><span data-ttu-id="245e1-103">Тип ресурса ChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="245e1-103">ChartTitleFormat resource type</span></span>

<span data-ttu-id="245e1-104">Инкапсулирует свойства формата для заголовка диаграммы.</span><span class="sxs-lookup"><span data-stu-id="245e1-104">Encapsulates the format properties for the chart title.</span></span>


## <a name="methods"></a><span data-ttu-id="245e1-105">Методы</span><span class="sxs-lookup"><span data-stu-id="245e1-105">Methods</span></span>
<span data-ttu-id="245e1-106">Нет</span><span class="sxs-lookup"><span data-stu-id="245e1-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="245e1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="245e1-107">Properties</span></span>
<span data-ttu-id="245e1-108">Нет</span><span class="sxs-lookup"><span data-stu-id="245e1-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="245e1-109">Связи</span><span class="sxs-lookup"><span data-stu-id="245e1-109">Relationships</span></span>
| <span data-ttu-id="245e1-110">Связь</span><span class="sxs-lookup"><span data-stu-id="245e1-110">Relationship</span></span> | <span data-ttu-id="245e1-111">Тип</span><span class="sxs-lookup"><span data-stu-id="245e1-111">Type</span></span>   |<span data-ttu-id="245e1-112">Описание</span><span class="sxs-lookup"><span data-stu-id="245e1-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="245e1-113">fill</span><span class="sxs-lookup"><span data-stu-id="245e1-113">fill</span></span>|[<span data-ttu-id="245e1-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="245e1-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="245e1-p101">Представляет формат заливки объекта, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="245e1-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="245e1-117">font</span><span class="sxs-lookup"><span data-stu-id="245e1-117">font</span></span>|[<span data-ttu-id="245e1-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="245e1-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="245e1-p102">Представляет атрибуты шрифта (имя, размер, цвет и т. д.) для текущего объекта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="245e1-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="245e1-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="245e1-121">JSON representation</span></span>

<span data-ttu-id="245e1-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="245e1-122">Here is a JSON representation of the resource.</span></span>

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
