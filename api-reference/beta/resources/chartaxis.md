---
title: Тип ресурса ChartAxis
description: Представляет одну ось на диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: d7485c57e45066731eb2e9101840681480ade401
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572824"
---
# <a name="chartaxis-resource-type"></a><span data-ttu-id="935cf-103">Тип ресурса ChartAxis</span><span class="sxs-lookup"><span data-stu-id="935cf-103">ChartAxis resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="935cf-104">Представляет одну ось на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="935cf-104">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="935cf-105">Методы</span><span class="sxs-lookup"><span data-stu-id="935cf-105">Methods</span></span>

| <span data-ttu-id="935cf-106">Метод</span><span class="sxs-lookup"><span data-stu-id="935cf-106">Method</span></span>           | <span data-ttu-id="935cf-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="935cf-107">Return Type</span></span>    |<span data-ttu-id="935cf-108">Описание</span><span class="sxs-lookup"><span data-stu-id="935cf-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="935cf-109">Получение объекта ChartAxis</span><span class="sxs-lookup"><span data-stu-id="935cf-109">Get ChartAxis</span></span>](../api/chartaxis-get.md) | [<span data-ttu-id="935cf-110">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="935cf-110">WorkbookChartAxis</span></span>](chartaxis.md) |<span data-ttu-id="935cf-111">Чтение свойств и связей объекта chartAxis.</span><span class="sxs-lookup"><span data-stu-id="935cf-111">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="935cf-112">Update</span><span class="sxs-lookup"><span data-stu-id="935cf-112">Update</span></span>](../api/chartaxis-update.md) | [<span data-ttu-id="935cf-113">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="935cf-113">WorkbookChartAxis</span></span>](chartaxis.md)   |<span data-ttu-id="935cf-114">Обновление объекта ChartAxis.</span><span class="sxs-lookup"><span data-stu-id="935cf-114">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="935cf-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="935cf-115">Properties</span></span>
| <span data-ttu-id="935cf-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="935cf-116">Property</span></span>     | <span data-ttu-id="935cf-117">Тип</span><span class="sxs-lookup"><span data-stu-id="935cf-117">Type</span></span>   |<span data-ttu-id="935cf-118">Описание</span><span class="sxs-lookup"><span data-stu-id="935cf-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="935cf-119">id</span><span class="sxs-lookup"><span data-stu-id="935cf-119">id</span></span>       |<span data-ttu-id="935cf-120">string</span><span class="sxs-lookup"><span data-stu-id="935cf-120">string</span></span>   | <span data-ttu-id="935cf-121">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="935cf-121">Unique identifier.</span></span> <span data-ttu-id="935cf-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="935cf-122">Read-only.</span></span>|
|<span data-ttu-id="935cf-123">majorUnit</span><span class="sxs-lookup"><span data-stu-id="935cf-123">majorUnit</span></span>|<span data-ttu-id="935cf-124">Json</span><span class="sxs-lookup"><span data-stu-id="935cf-124">Json</span></span>|<span data-ttu-id="935cf-p102">Обозначает интервал между двумя основными делениями. Можно указать в виде числового значения или пустой строки.  Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="935cf-p102">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="935cf-128">maximum</span><span class="sxs-lookup"><span data-stu-id="935cf-128">maximum</span></span>|<span data-ttu-id="935cf-129">Json</span><span class="sxs-lookup"><span data-stu-id="935cf-129">Json</span></span>|<span data-ttu-id="935cf-p103">Представляет максимальное значение на оси значений.  Можно указать в виде числового значения или пустой строки (для автоматически заданных значений оси).  Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="935cf-p103">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="935cf-133">minimum</span><span class="sxs-lookup"><span data-stu-id="935cf-133">minimum</span></span>|<span data-ttu-id="935cf-134">Json</span><span class="sxs-lookup"><span data-stu-id="935cf-134">Json</span></span>|<span data-ttu-id="935cf-p104">Представляет минимальное значение на оси значений. Ему можно присвоить числовое значение или пустую строку (для автоматически заданных значений оси). Всегда возвращает числовое значение.</span><span class="sxs-lookup"><span data-stu-id="935cf-p104">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="935cf-138">minorUnit</span><span class="sxs-lookup"><span data-stu-id="935cf-138">minorUnit</span></span>|<span data-ttu-id="935cf-139">Json</span><span class="sxs-lookup"><span data-stu-id="935cf-139">Json</span></span>|<span data-ttu-id="935cf-p105">Представляет интервал между двумя промежуточными делениями. Можно указать в виде числового значения или пустой строки (для автоматически заданных значений оси). Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="935cf-p105">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="935cf-143">Связи</span><span class="sxs-lookup"><span data-stu-id="935cf-143">Relationships</span></span>
| <span data-ttu-id="935cf-144">Связь</span><span class="sxs-lookup"><span data-stu-id="935cf-144">Relationship</span></span> | <span data-ttu-id="935cf-145">Тип</span><span class="sxs-lookup"><span data-stu-id="935cf-145">Type</span></span>   |<span data-ttu-id="935cf-146">Описание</span><span class="sxs-lookup"><span data-stu-id="935cf-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="935cf-147">format</span><span class="sxs-lookup"><span data-stu-id="935cf-147">format</span></span>|[<span data-ttu-id="935cf-148">WorkbookChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="935cf-148">WorkbookChartAxisFormat</span></span>](chartaxisformat.md)|<span data-ttu-id="935cf-p106">Представляет форматирование объекта диаграммы, в том числе форматирование линий и шрифта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="935cf-p106">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="935cf-151">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="935cf-151">majorGridlines</span></span>|[<span data-ttu-id="935cf-152">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="935cf-152">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="935cf-p107">Возвращает объект Gridlines, который представляет основные линии сетки для указанной оси. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="935cf-p107">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="935cf-155">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="935cf-155">minorGridlines</span></span>|[<span data-ttu-id="935cf-156">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="935cf-156">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="935cf-p108">Возвращает объект Gridlines, который представляет вспомогательные линии сетки для указанной оси. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="935cf-p108">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="935cf-159">должности.</span><span class="sxs-lookup"><span data-stu-id="935cf-159">title</span></span>|[<span data-ttu-id="935cf-160">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="935cf-160">WorkbookChartAxisTitle</span></span>](chartaxistitle.md)|<span data-ttu-id="935cf-p109">Представляет название оси. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="935cf-p109">Represents the axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="935cf-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="935cf-163">JSON representation</span></span>

<span data-ttu-id="935cf-164">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="935cf-164">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxis"
}-->

```json
{
  "id": "string",
  "majorUnit": "string",
  "maximum": "string",
  "minimum": "string",
  "minorUnit": "string",
   "format": {"@odata.type": "microsoft.graph.workbookChartAxisFormat"},
  "majorGridlines": {"@odata.type": "microsoft.graph.workbookChartGridlines"},
  "minorGridlines": {"@odata.type": "microsoft.graph.workbookChartGridlines"},
  "title": {"@odata.type": "microsoft.graph.workbookChartAxisTitle"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxis resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartaxis.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
