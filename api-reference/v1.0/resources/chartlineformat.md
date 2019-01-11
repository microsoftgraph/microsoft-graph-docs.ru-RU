---
title: Тип ресурса ChartLineFormat
description: Инкапсулирует параметры форматирования для элементов линий.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 70e4e3d5c88fccd2a34c3fa17d5fe4bf5dcf1e5b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805742"
---
# <a name="chartlineformat-resource-type"></a><span data-ttu-id="7c4ed-103">Тип ресурса ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="7c4ed-103">ChartLineFormat resource type</span></span>

<span data-ttu-id="7c4ed-104">Инкапсулирует параметры форматирования для элементов линий.</span><span class="sxs-lookup"><span data-stu-id="7c4ed-104">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="7c4ed-105">Методы</span><span class="sxs-lookup"><span data-stu-id="7c4ed-105">Methods</span></span>

| <span data-ttu-id="7c4ed-106">Метод</span><span class="sxs-lookup"><span data-stu-id="7c4ed-106">Method</span></span>           | <span data-ttu-id="7c4ed-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7c4ed-107">Return Type</span></span>    |<span data-ttu-id="7c4ed-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7c4ed-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7c4ed-109">Получение объекта ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="7c4ed-109">Get ChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="7c4ed-110">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="7c4ed-110">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="7c4ed-111">Чтение свойств и связей объекта chartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="7c4ed-111">Read properties and relationships of chartLineFormat object.</span></span>|
|<span data-ttu-id="7c4ed-112">[обновление](../api/chartlineformat-update.md).</span><span class="sxs-lookup"><span data-stu-id="7c4ed-112">[Update](../api/chartlineformat-update.md)</span></span> | [<span data-ttu-id="7c4ed-113">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="7c4ed-113">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="7c4ed-114">Обновление объекта ChartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="7c4ed-114">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="7c4ed-115">Clear</span><span class="sxs-lookup"><span data-stu-id="7c4ed-115">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="7c4ed-116">Нет</span><span class="sxs-lookup"><span data-stu-id="7c4ed-116">None</span></span>|<span data-ttu-id="7c4ed-117">Очищает формат линий элемента диаграммы.</span><span class="sxs-lookup"><span data-stu-id="7c4ed-117">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="7c4ed-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="7c4ed-118">Properties</span></span>
| <span data-ttu-id="7c4ed-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c4ed-119">Property</span></span>     | <span data-ttu-id="7c4ed-120">Тип</span><span class="sxs-lookup"><span data-stu-id="7c4ed-120">Type</span></span>   |<span data-ttu-id="7c4ed-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7c4ed-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c4ed-122">color</span><span class="sxs-lookup"><span data-stu-id="7c4ed-122">color</span></span>|<span data-ttu-id="7c4ed-123">строка</span><span class="sxs-lookup"><span data-stu-id="7c4ed-123">string</span></span>|<span data-ttu-id="7c4ed-124">HTML-код цвета, представляющий цвет линий в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="7c4ed-124">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7c4ed-125">Связи</span><span class="sxs-lookup"><span data-stu-id="7c4ed-125">Relationships</span></span>
<span data-ttu-id="7c4ed-126">Нет</span><span class="sxs-lookup"><span data-stu-id="7c4ed-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="7c4ed-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7c4ed-127">JSON representation</span></span>

<span data-ttu-id="7c4ed-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c4ed-128">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartLineFormat"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
