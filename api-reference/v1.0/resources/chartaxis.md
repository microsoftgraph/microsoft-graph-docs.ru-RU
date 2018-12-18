---
title: Тип ресурса ChartAxis
description: Представляет одну ось на диаграмме.
author: lumine2008
ms.openlocfilehash: 39c71e9fa832ffb967a1ef147ccd7e07d6b9aaec
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344368"
---
# <a name="chartaxis-resource-type"></a><span data-ttu-id="4b85d-103">Тип ресурса ChartAxis</span><span class="sxs-lookup"><span data-stu-id="4b85d-103">ChartAxis resource type</span></span>

<span data-ttu-id="4b85d-104">Представляет одну ось на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="4b85d-104">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="4b85d-105">Методы</span><span class="sxs-lookup"><span data-stu-id="4b85d-105">Methods</span></span>

| <span data-ttu-id="4b85d-106">Метод</span><span class="sxs-lookup"><span data-stu-id="4b85d-106">Method</span></span>           | <span data-ttu-id="4b85d-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4b85d-107">Return Type</span></span>    |<span data-ttu-id="4b85d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4b85d-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4b85d-109">Получение объекта ChartAxis</span><span class="sxs-lookup"><span data-stu-id="4b85d-109">Get ChartAxis</span></span>](../api/chartaxis-get.md) | [<span data-ttu-id="4b85d-110">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="4b85d-110">WorkbookChartAxis</span></span>](chartaxis.md) |<span data-ttu-id="4b85d-111">Чтение свойств и связей объекта chartAxis.</span><span class="sxs-lookup"><span data-stu-id="4b85d-111">Read properties and relationships of chartAxis object.</span></span>|
|<span data-ttu-id="4b85d-112">[обновление](../api/chartaxis-update.md).</span><span class="sxs-lookup"><span data-stu-id="4b85d-112">[Update](../api/chartaxis-update.md)</span></span> | [<span data-ttu-id="4b85d-113">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="4b85d-113">WorkbookChartAxis</span></span>](chartaxis.md)   |<span data-ttu-id="4b85d-114">Обновление объекта ChartAxis.</span><span class="sxs-lookup"><span data-stu-id="4b85d-114">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4b85d-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="4b85d-115">Properties</span></span>
| <span data-ttu-id="4b85d-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b85d-116">Property</span></span>     | <span data-ttu-id="4b85d-117">Тип</span><span class="sxs-lookup"><span data-stu-id="4b85d-117">Type</span></span>   |<span data-ttu-id="4b85d-118">Описание</span><span class="sxs-lookup"><span data-stu-id="4b85d-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4b85d-119">id</span><span class="sxs-lookup"><span data-stu-id="4b85d-119">id</span></span>       |<span data-ttu-id="4b85d-120">строка</span><span class="sxs-lookup"><span data-stu-id="4b85d-120">string</span></span>   | <span data-ttu-id="4b85d-121">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="4b85d-121">Unique identifier.</span></span> <span data-ttu-id="4b85d-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4b85d-122">Read-only.</span></span>|
|<span data-ttu-id="4b85d-123">majorUnit</span><span class="sxs-lookup"><span data-stu-id="4b85d-123">majorUnit</span></span>|<span data-ttu-id="4b85d-124">Json</span><span class="sxs-lookup"><span data-stu-id="4b85d-124">Json</span></span>|<span data-ttu-id="4b85d-p102">Обозначает интервал между двумя основными делениями. Можно указать в виде числового значения или пустой строки.  Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="4b85d-p102">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="4b85d-128">maximum</span><span class="sxs-lookup"><span data-stu-id="4b85d-128">maximum</span></span>|<span data-ttu-id="4b85d-129">Json</span><span class="sxs-lookup"><span data-stu-id="4b85d-129">Json</span></span>|<span data-ttu-id="4b85d-p103">Представляет максимальное значение на оси значений.  Можно указать в виде числового значения или пустой строки (для автоматически заданных значений оси).  Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="4b85d-p103">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="4b85d-133">minimum</span><span class="sxs-lookup"><span data-stu-id="4b85d-133">minimum</span></span>|<span data-ttu-id="4b85d-134">Json</span><span class="sxs-lookup"><span data-stu-id="4b85d-134">Json</span></span>|<span data-ttu-id="4b85d-p104">Представляет минимальное значение на оси значений. Ему можно присвоить числовое значение или пустую строку (для автоматически заданных значений оси). Всегда возвращает числовое значение.</span><span class="sxs-lookup"><span data-stu-id="4b85d-p104">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="4b85d-138">minorUnit</span><span class="sxs-lookup"><span data-stu-id="4b85d-138">minorUnit</span></span>|<span data-ttu-id="4b85d-139">Json</span><span class="sxs-lookup"><span data-stu-id="4b85d-139">Json</span></span>|<span data-ttu-id="4b85d-p105">Представляет интервал между двумя промежуточными делениями. Можно указать в виде числового значения или пустой строки (для автоматически заданных значений оси). Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="4b85d-p105">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b85d-143">Связи</span><span class="sxs-lookup"><span data-stu-id="4b85d-143">Relationships</span></span>
| <span data-ttu-id="4b85d-144">Связь</span><span class="sxs-lookup"><span data-stu-id="4b85d-144">Relationship</span></span> | <span data-ttu-id="4b85d-145">Тип</span><span class="sxs-lookup"><span data-stu-id="4b85d-145">Type</span></span>   |<span data-ttu-id="4b85d-146">Описание</span><span class="sxs-lookup"><span data-stu-id="4b85d-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b85d-147">format</span><span class="sxs-lookup"><span data-stu-id="4b85d-147">format</span></span>|[<span data-ttu-id="4b85d-148">WorkbookChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="4b85d-148">WorkbookChartAxisFormat</span></span>](chartaxisformat.md)|<span data-ttu-id="4b85d-p106">Представляет форматирование объекта диаграммы, в том числе форматирование линий и шрифта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4b85d-p106">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="4b85d-151">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="4b85d-151">majorGridlines</span></span>|[<span data-ttu-id="4b85d-152">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="4b85d-152">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="4b85d-p107">Возвращает объект Gridlines, который представляет основные линии сетки для указанной оси. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4b85d-p107">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="4b85d-155">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="4b85d-155">minorGridlines</span></span>|[<span data-ttu-id="4b85d-156">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="4b85d-156">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="4b85d-p108">Возвращает объект Gridlines, который представляет вспомогательные линии сетки для указанной оси. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4b85d-p108">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="4b85d-159">должности.</span><span class="sxs-lookup"><span data-stu-id="4b85d-159">title</span></span>|[<span data-ttu-id="4b85d-160">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="4b85d-160">WorkbookChartAxisTitle</span></span>](chartaxistitle.md)|<span data-ttu-id="4b85d-p109">Представляет название оси. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4b85d-p109">Represents the axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4b85d-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4b85d-163">JSON representation</span></span>

<span data-ttu-id="4b85d-164">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b85d-164">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxis resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->