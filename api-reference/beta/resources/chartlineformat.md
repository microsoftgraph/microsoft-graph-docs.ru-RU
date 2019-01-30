---
title: Тип ресурса ChartLineFormat
description: Инкапсулирует параметры форматирования для элементов линий.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b4409eb18dab41d43adc038b702a65fa8d63e4de
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640583"
---
# <a name="chartlineformat-resource-type"></a><span data-ttu-id="6e4ef-103">Тип ресурса ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="6e4ef-103">ChartLineFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e4ef-104">Инкапсулирует параметры форматирования для элементов линий.</span><span class="sxs-lookup"><span data-stu-id="6e4ef-104">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="6e4ef-105">Методы</span><span class="sxs-lookup"><span data-stu-id="6e4ef-105">Methods</span></span>

| <span data-ttu-id="6e4ef-106">Метод</span><span class="sxs-lookup"><span data-stu-id="6e4ef-106">Method</span></span>           | <span data-ttu-id="6e4ef-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6e4ef-107">Return Type</span></span>    |<span data-ttu-id="6e4ef-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6e4ef-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6e4ef-109">Получение объекта ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="6e4ef-109">Get ChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="6e4ef-110">ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="6e4ef-110">ChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="6e4ef-111">Чтение свойств и связей объекта chartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="6e4ef-111">Read properties and relationships of chartLineFormat object.</span></span>|
|<span data-ttu-id="6e4ef-112">[обновление](../api/chartlineformat-update.md).</span><span class="sxs-lookup"><span data-stu-id="6e4ef-112">[Update](../api/chartlineformat-update.md)</span></span> | [<span data-ttu-id="6e4ef-113">ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="6e4ef-113">ChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="6e4ef-114">Обновление объекта ChartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="6e4ef-114">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="6e4ef-115">Clear</span><span class="sxs-lookup"><span data-stu-id="6e4ef-115">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="6e4ef-116">Нет</span><span class="sxs-lookup"><span data-stu-id="6e4ef-116">None</span></span>|<span data-ttu-id="6e4ef-117">Очищает формат линий элемента диаграммы.</span><span class="sxs-lookup"><span data-stu-id="6e4ef-117">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="6e4ef-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="6e4ef-118">Properties</span></span>
| <span data-ttu-id="6e4ef-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e4ef-119">Property</span></span>     | <span data-ttu-id="6e4ef-120">Тип</span><span class="sxs-lookup"><span data-stu-id="6e4ef-120">Type</span></span>   |<span data-ttu-id="6e4ef-121">Описание</span><span class="sxs-lookup"><span data-stu-id="6e4ef-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e4ef-122">color</span><span class="sxs-lookup"><span data-stu-id="6e4ef-122">color</span></span>|<span data-ttu-id="6e4ef-123">строка</span><span class="sxs-lookup"><span data-stu-id="6e4ef-123">string</span></span>|<span data-ttu-id="6e4ef-124">HTML-код цвета, представляющий цвет линий в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="6e4ef-124">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e4ef-125">Связи</span><span class="sxs-lookup"><span data-stu-id="6e4ef-125">Relationships</span></span>
<span data-ttu-id="6e4ef-126">Нет</span><span class="sxs-lookup"><span data-stu-id="6e4ef-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6e4ef-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6e4ef-127">JSON representation</span></span>

<span data-ttu-id="6e4ef-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e4ef-128">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartLineFormat"
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
