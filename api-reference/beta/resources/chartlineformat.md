---
title: Тип ресурса ChartLineFormat
description: Инкапсулирует параметры форматирования для элементов линий.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6bede2e3e8eeb44dbac67832621a2b1586c6b319
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577055"
---
# <a name="chartlineformat-resource-type"></a><span data-ttu-id="2e26f-103">Тип ресурса ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="2e26f-103">ChartLineFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e26f-104">Инкапсулирует параметры форматирования для элементов линий.</span><span class="sxs-lookup"><span data-stu-id="2e26f-104">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="2e26f-105">Методы</span><span class="sxs-lookup"><span data-stu-id="2e26f-105">Methods</span></span>

| <span data-ttu-id="2e26f-106">Метод</span><span class="sxs-lookup"><span data-stu-id="2e26f-106">Method</span></span>           | <span data-ttu-id="2e26f-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2e26f-107">Return Type</span></span>    |<span data-ttu-id="2e26f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2e26f-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2e26f-109">Получение объекта ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="2e26f-109">Get ChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="2e26f-110">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="2e26f-110">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="2e26f-111">Чтение свойств и связей объекта chartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="2e26f-111">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="2e26f-112">Update</span><span class="sxs-lookup"><span data-stu-id="2e26f-112">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="2e26f-113">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="2e26f-113">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="2e26f-114">Обновление объекта ChartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="2e26f-114">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="2e26f-115">Clear</span><span class="sxs-lookup"><span data-stu-id="2e26f-115">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="2e26f-116">Нет</span><span class="sxs-lookup"><span data-stu-id="2e26f-116">None</span></span>|<span data-ttu-id="2e26f-117">Очищает формат линий элемента диаграммы.</span><span class="sxs-lookup"><span data-stu-id="2e26f-117">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="2e26f-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="2e26f-118">Properties</span></span>
| <span data-ttu-id="2e26f-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e26f-119">Property</span></span>     | <span data-ttu-id="2e26f-120">Тип</span><span class="sxs-lookup"><span data-stu-id="2e26f-120">Type</span></span>   |<span data-ttu-id="2e26f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="2e26f-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e26f-122">color</span><span class="sxs-lookup"><span data-stu-id="2e26f-122">color</span></span>|<span data-ttu-id="2e26f-123">строка</span><span class="sxs-lookup"><span data-stu-id="2e26f-123">string</span></span>|<span data-ttu-id="2e26f-124">HTML-код цвета, представляющий цвет линий в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="2e26f-124">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e26f-125">Связи</span><span class="sxs-lookup"><span data-stu-id="2e26f-125">Relationships</span></span>
<span data-ttu-id="2e26f-126">Нет</span><span class="sxs-lookup"><span data-stu-id="2e26f-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="2e26f-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2e26f-127">JSON representation</span></span>

<span data-ttu-id="2e26f-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e26f-128">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartlineformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
