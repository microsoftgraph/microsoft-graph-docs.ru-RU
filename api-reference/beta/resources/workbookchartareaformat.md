---
title: Тип ресурса Воркбукчартареаформат
description: Инкапсулирует свойства формата для всей области диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6554604e2bb4c49d7e14546f1c5079690f99637f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348939"
---
# <a name="workbookchartareaformat-resource-type"></a><span data-ttu-id="66339-103">Тип ресурса Воркбукчартареаформат</span><span class="sxs-lookup"><span data-stu-id="66339-103">workbookChartAreaFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66339-104">Инкапсулирует свойства формата для всей области диаграммы.</span><span class="sxs-lookup"><span data-stu-id="66339-104">Encapsulates the format properties for the overall chart area.</span></span>


## <a name="methods"></a><span data-ttu-id="66339-105">Методы</span><span class="sxs-lookup"><span data-stu-id="66339-105">Methods</span></span>
<span data-ttu-id="66339-106">Отсутствует</span><span class="sxs-lookup"><span data-stu-id="66339-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="66339-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="66339-107">Properties</span></span>
<span data-ttu-id="66339-108">Нет</span><span class="sxs-lookup"><span data-stu-id="66339-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="66339-109">Отношения</span><span class="sxs-lookup"><span data-stu-id="66339-109">Relationships</span></span>
| <span data-ttu-id="66339-110">Отношение</span><span class="sxs-lookup"><span data-stu-id="66339-110">Relationship</span></span> | <span data-ttu-id="66339-111">Тип</span><span class="sxs-lookup"><span data-stu-id="66339-111">Type</span></span>   |<span data-ttu-id="66339-112">Описание</span><span class="sxs-lookup"><span data-stu-id="66339-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66339-113">fill</span><span class="sxs-lookup"><span data-stu-id="66339-113">fill</span></span>|[<span data-ttu-id="66339-114">Воркбукчартфилл</span><span class="sxs-lookup"><span data-stu-id="66339-114">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="66339-p101">Представляет формат заливки объекта, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="66339-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="66339-117">font</span><span class="sxs-lookup"><span data-stu-id="66339-117">font</span></span>|[<span data-ttu-id="66339-118">Воркбукчартфонт</span><span class="sxs-lookup"><span data-stu-id="66339-118">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="66339-119">Представляет атрибуты шрифта (имя, размер шрифта, цвет и т. д.) для текущего объекта.</span><span class="sxs-lookup"><span data-stu-id="66339-119">Represents the font attributes (font name, font size, color, etc.) for the current object.</span></span> <span data-ttu-id="66339-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="66339-120">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="66339-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="66339-121">JSON representation</span></span>

<span data-ttu-id="66339-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66339-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "fill",
    "font"
    ],
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartAreaFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
