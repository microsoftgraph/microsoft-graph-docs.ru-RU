---
title: Тип ресурса ChartTitleFormat
description: Инкапсулирует свойства формата для заголовка диаграммы.
ms.openlocfilehash: 7e84412adb46981a0a2b8570ed28c62d36936e36
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025263"
---
# <a name="charttitleformat-resource-type"></a><span data-ttu-id="ef283-103">Тип ресурса ChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="ef283-103">ChartTitleFormat resource type</span></span>

<span data-ttu-id="ef283-104">Инкапсулирует свойства формата для заголовка диаграммы.</span><span class="sxs-lookup"><span data-stu-id="ef283-104">Encapsulates the format properties for the chart title.</span></span>


## <a name="methods"></a><span data-ttu-id="ef283-105">Методы</span><span class="sxs-lookup"><span data-stu-id="ef283-105">Methods</span></span>
<span data-ttu-id="ef283-106">Нет</span><span class="sxs-lookup"><span data-stu-id="ef283-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="ef283-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ef283-107">Properties</span></span>
<span data-ttu-id="ef283-108">Нет</span><span class="sxs-lookup"><span data-stu-id="ef283-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="ef283-109">Связи</span><span class="sxs-lookup"><span data-stu-id="ef283-109">Relationships</span></span>
| <span data-ttu-id="ef283-110">Связь</span><span class="sxs-lookup"><span data-stu-id="ef283-110">Relationship</span></span> | <span data-ttu-id="ef283-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ef283-111">Type</span></span>   |<span data-ttu-id="ef283-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ef283-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef283-113">fill</span><span class="sxs-lookup"><span data-stu-id="ef283-113">fill</span></span>|[<span data-ttu-id="ef283-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="ef283-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="ef283-p101">Представляет формат заливки объекта, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef283-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="ef283-117">font</span><span class="sxs-lookup"><span data-stu-id="ef283-117">font</span></span>|[<span data-ttu-id="ef283-118">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="ef283-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="ef283-p102">Представляет атрибуты шрифта (имя, размер, цвет и т. д.) для текущего объекта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef283-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="ef283-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ef283-121">JSON representation</span></span>

<span data-ttu-id="ef283-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef283-122">Here is a JSON representation of the resource.</span></span>

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
