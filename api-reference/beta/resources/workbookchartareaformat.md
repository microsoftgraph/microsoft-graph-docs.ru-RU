---
title: Тип ресурса Воркбукчартареаформат
description: Инкапсулирует свойства формата для всей области диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 02e176887053654c103bf2aedaf86f48831d9d08
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039141"
---
# <a name="workbookchartareaformat-resource-type"></a><span data-ttu-id="9b4a0-103">Тип ресурса Воркбукчартареаформат</span><span class="sxs-lookup"><span data-stu-id="9b4a0-103">workbookChartAreaFormat resource type</span></span>

<span data-ttu-id="9b4a0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b4a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b4a0-105">Инкапсулирует свойства формата для всей области диаграммы.</span><span class="sxs-lookup"><span data-stu-id="9b4a0-105">Encapsulates the format properties for the overall chart area.</span></span>


## <a name="methods"></a><span data-ttu-id="9b4a0-106">Методы</span><span class="sxs-lookup"><span data-stu-id="9b4a0-106">Methods</span></span>
<span data-ttu-id="9b4a0-107">Нет</span><span class="sxs-lookup"><span data-stu-id="9b4a0-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="9b4a0-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9b4a0-108">Properties</span></span>
<span data-ttu-id="9b4a0-109">Нет</span><span class="sxs-lookup"><span data-stu-id="9b4a0-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="9b4a0-110">Отношения</span><span class="sxs-lookup"><span data-stu-id="9b4a0-110">Relationships</span></span>
| <span data-ttu-id="9b4a0-111">Связь</span><span class="sxs-lookup"><span data-stu-id="9b4a0-111">Relationship</span></span> | <span data-ttu-id="9b4a0-112">Тип</span><span class="sxs-lookup"><span data-stu-id="9b4a0-112">Type</span></span>   |<span data-ttu-id="9b4a0-113">Описание</span><span class="sxs-lookup"><span data-stu-id="9b4a0-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b4a0-114">fill</span><span class="sxs-lookup"><span data-stu-id="9b4a0-114">fill</span></span>|[<span data-ttu-id="9b4a0-115">воркбукчартфилл</span><span class="sxs-lookup"><span data-stu-id="9b4a0-115">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="9b4a0-p101">Представляет формат заливки объекта, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b4a0-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="9b4a0-118">font</span><span class="sxs-lookup"><span data-stu-id="9b4a0-118">font</span></span>|[<span data-ttu-id="9b4a0-119">воркбукчартфонт</span><span class="sxs-lookup"><span data-stu-id="9b4a0-119">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="9b4a0-120">Представляет атрибуты шрифта (имя, размер шрифта, цвет и т. д.) для текущего объекта.</span><span class="sxs-lookup"><span data-stu-id="9b4a0-120">Represents the font attributes (font name, font size, color, etc.) for the current object.</span></span> <span data-ttu-id="9b4a0-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b4a0-121">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9b4a0-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9b4a0-122">JSON representation</span></span>

<span data-ttu-id="9b4a0-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b4a0-123">Here is a JSON representation of the resource.</span></span>

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


