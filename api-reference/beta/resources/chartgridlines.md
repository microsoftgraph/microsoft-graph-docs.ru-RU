---
title: Тип ресурса ChartGridlines
description: Представляет основные или вспомогательные линии сетки на оси диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3c57c68e7d9dfcd26741d15e302dd5dddeaae378
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572537"
---
# <a name="chartgridlines-resource-type"></a><span data-ttu-id="48de2-103">Тип ресурса ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="48de2-103">ChartGridlines resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48de2-104">Представляет основные или вспомогательные линии сетки на оси диаграммы.</span><span class="sxs-lookup"><span data-stu-id="48de2-104">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="48de2-105">Методы</span><span class="sxs-lookup"><span data-stu-id="48de2-105">Methods</span></span>

| <span data-ttu-id="48de2-106">Метод</span><span class="sxs-lookup"><span data-stu-id="48de2-106">Method</span></span>           | <span data-ttu-id="48de2-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="48de2-107">Return Type</span></span>    |<span data-ttu-id="48de2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="48de2-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="48de2-109">Получение объекта ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="48de2-109">Get ChartGridlines</span></span>](../api/chartgridlines-get.md) | [<span data-ttu-id="48de2-110">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="48de2-110">WorkbookChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="48de2-111">Чтение свойств и связей объекта chartGridlines.</span><span class="sxs-lookup"><span data-stu-id="48de2-111">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="48de2-112">Update</span><span class="sxs-lookup"><span data-stu-id="48de2-112">Update</span></span>](../api/chartgridlines-update.md) | [<span data-ttu-id="48de2-113">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="48de2-113">WorkbookChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="48de2-114">Обновление объекта ChartGridlines.</span><span class="sxs-lookup"><span data-stu-id="48de2-114">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="48de2-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="48de2-115">Properties</span></span>
| <span data-ttu-id="48de2-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="48de2-116">Property</span></span>     | <span data-ttu-id="48de2-117">Тип</span><span class="sxs-lookup"><span data-stu-id="48de2-117">Type</span></span>   |<span data-ttu-id="48de2-118">Описание</span><span class="sxs-lookup"><span data-stu-id="48de2-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48de2-119">visible</span><span class="sxs-lookup"><span data-stu-id="48de2-119">visible</span></span>|<span data-ttu-id="48de2-120">boolean</span><span class="sxs-lookup"><span data-stu-id="48de2-120">boolean</span></span>|<span data-ttu-id="48de2-121">Логическое значение, определяющее, отображаются ли линии сетки оси.</span><span class="sxs-lookup"><span data-stu-id="48de2-121">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="48de2-122">Связи</span><span class="sxs-lookup"><span data-stu-id="48de2-122">Relationships</span></span>
| <span data-ttu-id="48de2-123">Связь</span><span class="sxs-lookup"><span data-stu-id="48de2-123">Relationship</span></span> | <span data-ttu-id="48de2-124">Тип</span><span class="sxs-lookup"><span data-stu-id="48de2-124">Type</span></span>   |<span data-ttu-id="48de2-125">Описание</span><span class="sxs-lookup"><span data-stu-id="48de2-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48de2-126">format</span><span class="sxs-lookup"><span data-stu-id="48de2-126">format</span></span>|[<span data-ttu-id="48de2-127">WorkbookChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="48de2-127">WorkbookChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="48de2-p101">Представляет форматирование линий сетки диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="48de2-p101">Represents the formatting of chart gridlines. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="48de2-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="48de2-130">JSON representation</span></span>

<span data-ttu-id="48de2-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48de2-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartGridlines"
}-->

```json
{
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartGridlines resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartgridlines.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
