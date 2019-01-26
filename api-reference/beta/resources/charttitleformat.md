---
title: Тип ресурса ChartTitleFormat
description: Инкапсулирует свойства формата для заголовка диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7dd9400873234fd73ebe506a49caf6583d05b75b
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574014"
---
# <a name="charttitleformat-resource-type"></a><span data-ttu-id="a4a6c-103">Тип ресурса ChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="a4a6c-103">ChartTitleFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="methods"></a><span data-ttu-id="a4a6c-104">Методы</span><span class="sxs-lookup"><span data-stu-id="a4a6c-104">Methods</span></span>
<span data-ttu-id="a4a6c-105">Нет</span><span class="sxs-lookup"><span data-stu-id="a4a6c-105">None</span></span>

## <a name="properties"></a><span data-ttu-id="a4a6c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a4a6c-106">Properties</span></span>
<span data-ttu-id="a4a6c-107">Нет</span><span class="sxs-lookup"><span data-stu-id="a4a6c-107">None</span></span>

## <a name="relationships"></a><span data-ttu-id="a4a6c-108">Связи</span><span class="sxs-lookup"><span data-stu-id="a4a6c-108">Relationships</span></span>
| <span data-ttu-id="a4a6c-109">Связь</span><span class="sxs-lookup"><span data-stu-id="a4a6c-109">Relationship</span></span> | <span data-ttu-id="a4a6c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a4a6c-110">Type</span></span>   |<span data-ttu-id="a4a6c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a4a6c-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4a6c-112">fill</span><span class="sxs-lookup"><span data-stu-id="a4a6c-112">fill</span></span>|[<span data-ttu-id="a4a6c-113">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="a4a6c-113">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="a4a6c-p101">Представляет формат заливки объекта, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4a6c-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="a4a6c-116">font</span><span class="sxs-lookup"><span data-stu-id="a4a6c-116">font</span></span>|[<span data-ttu-id="a4a6c-117">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="a4a6c-117">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="a4a6c-p102">Представляет атрибуты шрифта (имя, размер, цвет и т. д.) для текущего объекта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4a6c-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="a4a6c-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a4a6c-120">JSON representation</span></span>

<span data-ttu-id="a4a6c-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4a6c-121">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartAreaFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/charttitleformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
