---
title: Тип ресурса Воркбукчартаксисформат
description: Инкапсулирует свойства формата для оси диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: d04f885f135eadf2a8404b7e17b3b2ed32554e14
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039066"
---
# <a name="workbookchartaxisformat-resource-type"></a><span data-ttu-id="a7720-103">Тип ресурса Воркбукчартаксисформат</span><span class="sxs-lookup"><span data-stu-id="a7720-103">workbookChartAxisFormat resource type</span></span>

<span data-ttu-id="a7720-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7720-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7720-105">Инкапсулирует свойства формата для оси диаграммы.</span><span class="sxs-lookup"><span data-stu-id="a7720-105">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="a7720-106">Методы</span><span class="sxs-lookup"><span data-stu-id="a7720-106">Methods</span></span>
<span data-ttu-id="a7720-107">Нет</span><span class="sxs-lookup"><span data-stu-id="a7720-107">None</span></span>
## <a name="properties"></a><span data-ttu-id="a7720-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a7720-108">Properties</span></span>
<span data-ttu-id="a7720-109">Нет</span><span class="sxs-lookup"><span data-stu-id="a7720-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="a7720-110">Отношения</span><span class="sxs-lookup"><span data-stu-id="a7720-110">Relationships</span></span>
| <span data-ttu-id="a7720-111">Связь</span><span class="sxs-lookup"><span data-stu-id="a7720-111">Relationship</span></span> | <span data-ttu-id="a7720-112">Тип</span><span class="sxs-lookup"><span data-stu-id="a7720-112">Type</span></span>   |<span data-ttu-id="a7720-113">Описание</span><span class="sxs-lookup"><span data-stu-id="a7720-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a7720-114">font</span><span class="sxs-lookup"><span data-stu-id="a7720-114">font</span></span>|[<span data-ttu-id="a7720-115">воркбукчартфонт</span><span class="sxs-lookup"><span data-stu-id="a7720-115">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="a7720-p101">Представляет атрибуты шрифта (имя, размер, цвет и т. д.) для элемента оси диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a7720-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="a7720-118">line</span><span class="sxs-lookup"><span data-stu-id="a7720-118">line</span></span>|[<span data-ttu-id="a7720-119">воркбукчартлинеформат</span><span class="sxs-lookup"><span data-stu-id="a7720-119">workbookChartLineFormat</span></span>](workbookchartlineformat.md)|<span data-ttu-id="a7720-120">Представляет форматирование линий диаграммы.</span><span class="sxs-lookup"><span data-stu-id="a7720-120">Represents chart line formatting.</span></span> <span data-ttu-id="a7720-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a7720-121">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="a7720-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a7720-122">JSON representation</span></span>

<span data-ttu-id="a7720-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7720-123">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"},
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxisFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


