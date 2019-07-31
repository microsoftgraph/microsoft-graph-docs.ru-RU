---
title: Тип ресурса Воркбукчарттитлеформат
description: Инкапсулирует свойства формата для заголовка диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ce00af7877b4602e76c390635478713835da2f2b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007139"
---
# <a name="workbookcharttitleformat-resource-type"></a><span data-ttu-id="5ba1f-103">Тип ресурса Воркбукчарттитлеформат</span><span class="sxs-lookup"><span data-stu-id="5ba1f-103">workbookChartTitleFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ba1f-104">Инкапсулирует свойства формата для заголовка диаграммы.</span><span class="sxs-lookup"><span data-stu-id="5ba1f-104">Encapsulates the format properties for the chart title.</span></span>


## <a name="methods"></a><span data-ttu-id="5ba1f-105">Методы</span><span class="sxs-lookup"><span data-stu-id="5ba1f-105">Methods</span></span>
<span data-ttu-id="5ba1f-106">Нет</span><span class="sxs-lookup"><span data-stu-id="5ba1f-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="5ba1f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5ba1f-107">Properties</span></span>
<span data-ttu-id="5ba1f-108">Нет</span><span class="sxs-lookup"><span data-stu-id="5ba1f-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="5ba1f-109">Отношения</span><span class="sxs-lookup"><span data-stu-id="5ba1f-109">Relationships</span></span>
| <span data-ttu-id="5ba1f-110">Отношение</span><span class="sxs-lookup"><span data-stu-id="5ba1f-110">Relationship</span></span> | <span data-ttu-id="5ba1f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="5ba1f-111">Type</span></span>   |<span data-ttu-id="5ba1f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5ba1f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ba1f-113">fill</span><span class="sxs-lookup"><span data-stu-id="5ba1f-113">fill</span></span>|[<span data-ttu-id="5ba1f-114">Воркбукчартфилл</span><span class="sxs-lookup"><span data-stu-id="5ba1f-114">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="5ba1f-p101">Представляет формат заливки объекта, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5ba1f-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="5ba1f-117">font</span><span class="sxs-lookup"><span data-stu-id="5ba1f-117">font</span></span>|[<span data-ttu-id="5ba1f-118">Воркбукчартфонт</span><span class="sxs-lookup"><span data-stu-id="5ba1f-118">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="5ba1f-119">Представляет атрибуты шрифта (имя, размер шрифта, цвет и т. д.) для текущего объекта.</span><span class="sxs-lookup"><span data-stu-id="5ba1f-119">Represents the font attributes (font name, font size, color, etc.) for the current object.</span></span> <span data-ttu-id="5ba1f-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5ba1f-120">Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="5ba1f-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5ba1f-121">JSON representation</span></span>

<span data-ttu-id="5ba1f-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5ba1f-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "fill",
    "font"
    ],
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
  "description": "workbookChartTitleFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
