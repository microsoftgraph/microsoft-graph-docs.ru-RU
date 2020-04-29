---
title: Тип ресурса ChartTitleFormat
description: Инкапсулирует свойства формата для заголовка диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: da702a7718765af464525c3ae2fafc8376296d25
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533083"
---
# <a name="charttitleformat-resource-type"></a><span data-ttu-id="a8dfd-103">Тип ресурса ChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="a8dfd-103">ChartTitleFormat resource type</span></span>

<span data-ttu-id="a8dfd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8dfd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a8dfd-105">Инкапсулирует свойства формата для заголовка диаграммы.</span><span class="sxs-lookup"><span data-stu-id="a8dfd-105">Encapsulates the format properties for the chart title.</span></span>


## <a name="methods"></a><span data-ttu-id="a8dfd-106">Methods</span><span class="sxs-lookup"><span data-stu-id="a8dfd-106">Methods</span></span>
<span data-ttu-id="a8dfd-107">Нет</span><span class="sxs-lookup"><span data-stu-id="a8dfd-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="a8dfd-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a8dfd-108">Properties</span></span>
<span data-ttu-id="a8dfd-109">Нет</span><span class="sxs-lookup"><span data-stu-id="a8dfd-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="a8dfd-110">Связи</span><span class="sxs-lookup"><span data-stu-id="a8dfd-110">Relationships</span></span>
| <span data-ttu-id="a8dfd-111">Связь</span><span class="sxs-lookup"><span data-stu-id="a8dfd-111">Relationship</span></span> | <span data-ttu-id="a8dfd-112">Тип</span><span class="sxs-lookup"><span data-stu-id="a8dfd-112">Type</span></span>   |<span data-ttu-id="a8dfd-113">Описание</span><span class="sxs-lookup"><span data-stu-id="a8dfd-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8dfd-114">fill</span><span class="sxs-lookup"><span data-stu-id="a8dfd-114">fill</span></span>|[<span data-ttu-id="a8dfd-115">воркбукчартфилл</span><span class="sxs-lookup"><span data-stu-id="a8dfd-115">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="a8dfd-p101">Представляет формат заливки объекта, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a8dfd-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="a8dfd-118">font</span><span class="sxs-lookup"><span data-stu-id="a8dfd-118">font</span></span>|[<span data-ttu-id="a8dfd-119">воркбукчартфонт</span><span class="sxs-lookup"><span data-stu-id="a8dfd-119">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="a8dfd-120">Представляет атрибуты шрифта (имя, размер шрифта, цвет и т. д.) для текущего объекта.</span><span class="sxs-lookup"><span data-stu-id="a8dfd-120">Represents the font attributes (font name, font size, color, etc.) for the current object.</span></span> <span data-ttu-id="a8dfd-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a8dfd-121">Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="a8dfd-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a8dfd-122">JSON representation</span></span>

<span data-ttu-id="a8dfd-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8dfd-123">Here is a JSON representation of the resource.</span></span>

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
