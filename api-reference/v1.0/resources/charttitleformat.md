---
title: Тип ресурса ChartTitleFormat
description: Инкапсулирует свойства формата для заголовка диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 632b3a165a5f2f3a4216868bf440099610cdc800
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059217"
---
# <a name="charttitleformat-resource-type"></a><span data-ttu-id="7c806-103">Тип ресурса ChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="7c806-103">ChartTitleFormat resource type</span></span>

<span data-ttu-id="7c806-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c806-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7c806-105">Инкапсулирует свойства формата для заголовка диаграммы.</span><span class="sxs-lookup"><span data-stu-id="7c806-105">Encapsulates the format properties for the chart title.</span></span>


## <a name="methods"></a><span data-ttu-id="7c806-106">Методы</span><span class="sxs-lookup"><span data-stu-id="7c806-106">Methods</span></span>
<span data-ttu-id="7c806-107">Нет</span><span class="sxs-lookup"><span data-stu-id="7c806-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="7c806-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7c806-108">Properties</span></span>
<span data-ttu-id="7c806-109">Нет</span><span class="sxs-lookup"><span data-stu-id="7c806-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="7c806-110">Связи</span><span class="sxs-lookup"><span data-stu-id="7c806-110">Relationships</span></span>
| <span data-ttu-id="7c806-111">Связь</span><span class="sxs-lookup"><span data-stu-id="7c806-111">Relationship</span></span> | <span data-ttu-id="7c806-112">Тип</span><span class="sxs-lookup"><span data-stu-id="7c806-112">Type</span></span>   |<span data-ttu-id="7c806-113">Описание</span><span class="sxs-lookup"><span data-stu-id="7c806-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c806-114">fill</span><span class="sxs-lookup"><span data-stu-id="7c806-114">fill</span></span>|[<span data-ttu-id="7c806-115">воркбукчартфилл</span><span class="sxs-lookup"><span data-stu-id="7c806-115">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="7c806-p101">Представляет формат заливки объекта, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c806-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="7c806-118">font</span><span class="sxs-lookup"><span data-stu-id="7c806-118">font</span></span>|[<span data-ttu-id="7c806-119">воркбукчартфонт</span><span class="sxs-lookup"><span data-stu-id="7c806-119">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="7c806-120">Представляет атрибуты шрифта (имя, размер шрифта, цвет и т. д.) для текущего объекта.</span><span class="sxs-lookup"><span data-stu-id="7c806-120">Represents the font attributes (font name, font size, color, etc.) for the current object.</span></span> <span data-ttu-id="7c806-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c806-121">Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="7c806-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7c806-122">JSON representation</span></span>

<span data-ttu-id="7c806-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c806-123">Here is a JSON representation of the resource.</span></span>

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

