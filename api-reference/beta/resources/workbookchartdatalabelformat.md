---
title: Тип ресурса Воркбукчартдаталабелформат
description: Инкапсулирует свойства формата для меток данных диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 883f2ff1ce1c0b89f1525ea39e0adb558a1870cc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979296"
---
# <a name="workbookchartdatalabelformat-resource-type"></a><span data-ttu-id="ad21b-103">Тип ресурса Воркбукчартдаталабелформат</span><span class="sxs-lookup"><span data-stu-id="ad21b-103">workbookChartDataLabelFormat resource type</span></span>

<span data-ttu-id="ad21b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad21b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad21b-105">Инкапсулирует свойства формата для меток данных диаграммы.</span><span class="sxs-lookup"><span data-stu-id="ad21b-105">Encapsulates the format properties for the chart data labels.</span></span>


## <a name="methods"></a><span data-ttu-id="ad21b-106">Методы</span><span class="sxs-lookup"><span data-stu-id="ad21b-106">Methods</span></span>
<span data-ttu-id="ad21b-107">Нет</span><span class="sxs-lookup"><span data-stu-id="ad21b-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="ad21b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ad21b-108">Properties</span></span>
<span data-ttu-id="ad21b-109">Нет</span><span class="sxs-lookup"><span data-stu-id="ad21b-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="ad21b-110">Связи</span><span class="sxs-lookup"><span data-stu-id="ad21b-110">Relationships</span></span>
| <span data-ttu-id="ad21b-111">Связь</span><span class="sxs-lookup"><span data-stu-id="ad21b-111">Relationship</span></span> | <span data-ttu-id="ad21b-112">Тип</span><span class="sxs-lookup"><span data-stu-id="ad21b-112">Type</span></span>   |<span data-ttu-id="ad21b-113">Описание</span><span class="sxs-lookup"><span data-stu-id="ad21b-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad21b-114">fill</span><span class="sxs-lookup"><span data-stu-id="ad21b-114">fill</span></span>|[<span data-ttu-id="ad21b-115">воркбукчартфилл</span><span class="sxs-lookup"><span data-stu-id="ad21b-115">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="ad21b-p101">Представляет формат заливки для текущей метки данных диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ad21b-p101">Represents the fill format of the current chart data label. Read-only.</span></span>|
|<span data-ttu-id="ad21b-118">font</span><span class="sxs-lookup"><span data-stu-id="ad21b-118">font</span></span>|[<span data-ttu-id="ad21b-119">воркбукчартфонт</span><span class="sxs-lookup"><span data-stu-id="ad21b-119">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="ad21b-120">Представляет атрибуты шрифта (имя, размер шрифта, цвет и т. д.) для подписи данных диаграммы.</span><span class="sxs-lookup"><span data-stu-id="ad21b-120">Represents the font attributes (font name, font size, color, etc.) for a chart data label.</span></span> <span data-ttu-id="ad21b-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ad21b-121">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="ad21b-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ad21b-122">JSON representation</span></span>

<span data-ttu-id="ad21b-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad21b-123">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "fill",
    "font"
    ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartDataLabelFormat"
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
  "description": "ChartDataLabelFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


