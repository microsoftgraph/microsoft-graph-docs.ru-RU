---
title: Тип ресурса ChartLineFormat
description: Инкапсулирует параметры форматирования для элементов линий.
author: lumine2008
ms.openlocfilehash: 1940b5dfe09c2895fbf1b8eb6bf4e5227194367c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357304"
---
# <a name="chartlineformat-resource-type"></a><span data-ttu-id="ede15-103">Тип ресурса ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="ede15-103">ChartLineFormat resource type</span></span>

<span data-ttu-id="ede15-104">Инкапсулирует параметры форматирования для элементов линий.</span><span class="sxs-lookup"><span data-stu-id="ede15-104">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="ede15-105">Методы</span><span class="sxs-lookup"><span data-stu-id="ede15-105">Methods</span></span>

| <span data-ttu-id="ede15-106">Метод</span><span class="sxs-lookup"><span data-stu-id="ede15-106">Method</span></span>           | <span data-ttu-id="ede15-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ede15-107">Return Type</span></span>    |<span data-ttu-id="ede15-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ede15-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ede15-109">Получение объекта ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="ede15-109">Get ChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="ede15-110">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="ede15-110">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="ede15-111">Чтение свойств и связей объекта chartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="ede15-111">Read properties and relationships of chartLineFormat object.</span></span>|
|<span data-ttu-id="ede15-112">[обновление](../api/chartlineformat-update.md).</span><span class="sxs-lookup"><span data-stu-id="ede15-112">[Update](../api/chartlineformat-update.md)</span></span> | [<span data-ttu-id="ede15-113">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="ede15-113">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="ede15-114">Обновление объекта ChartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="ede15-114">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="ede15-115">Clear</span><span class="sxs-lookup"><span data-stu-id="ede15-115">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="ede15-116">Нет</span><span class="sxs-lookup"><span data-stu-id="ede15-116">None</span></span>|<span data-ttu-id="ede15-117">Очищает формат линий элемента диаграммы.</span><span class="sxs-lookup"><span data-stu-id="ede15-117">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="ede15-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="ede15-118">Properties</span></span>
| <span data-ttu-id="ede15-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="ede15-119">Property</span></span>     | <span data-ttu-id="ede15-120">Тип</span><span class="sxs-lookup"><span data-stu-id="ede15-120">Type</span></span>   |<span data-ttu-id="ede15-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ede15-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ede15-122">color</span><span class="sxs-lookup"><span data-stu-id="ede15-122">color</span></span>|<span data-ttu-id="ede15-123">строка</span><span class="sxs-lookup"><span data-stu-id="ede15-123">string</span></span>|<span data-ttu-id="ede15-124">HTML-код цвета, представляющий цвет линий в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="ede15-124">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ede15-125">Связи</span><span class="sxs-lookup"><span data-stu-id="ede15-125">Relationships</span></span>
<span data-ttu-id="ede15-126">Нет</span><span class="sxs-lookup"><span data-stu-id="ede15-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ede15-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ede15-127">JSON representation</span></span>

<span data-ttu-id="ede15-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ede15-128">Here is a JSON representation of the resource.</span></span>

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