---
title: Тип ресурса ChartAxis
description: Представляет одну ось на диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 0ae528e68aa3bf28457f2fee04beb6a8013e902d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531895"
---
# <a name="chartaxis-resource-type"></a><span data-ttu-id="9c2d1-103">Тип ресурса ChartAxis</span><span class="sxs-lookup"><span data-stu-id="9c2d1-103">ChartAxis resource type</span></span>

<span data-ttu-id="9c2d1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c2d1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9c2d1-105">Представляет одну ось на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="9c2d1-105">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="9c2d1-106">Методы</span><span class="sxs-lookup"><span data-stu-id="9c2d1-106">Methods</span></span>

| <span data-ttu-id="9c2d1-107">Метод</span><span class="sxs-lookup"><span data-stu-id="9c2d1-107">Method</span></span>           | <span data-ttu-id="9c2d1-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9c2d1-108">Return Type</span></span>    |<span data-ttu-id="9c2d1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9c2d1-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9c2d1-110">Получение объекта ChartAxis</span><span class="sxs-lookup"><span data-stu-id="9c2d1-110">Get ChartAxis</span></span>](../api/chartaxis-get.md) | [<span data-ttu-id="9c2d1-111">воркбукчартаксис</span><span class="sxs-lookup"><span data-stu-id="9c2d1-111">WorkbookChartAxis</span></span>](chartaxis.md) |<span data-ttu-id="9c2d1-112">Чтение свойств и связей объекта chartAxis.</span><span class="sxs-lookup"><span data-stu-id="9c2d1-112">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="9c2d1-113">Обновление</span><span class="sxs-lookup"><span data-stu-id="9c2d1-113">Update</span></span>](../api/chartaxis-update.md) | [<span data-ttu-id="9c2d1-114">воркбукчартаксис</span><span class="sxs-lookup"><span data-stu-id="9c2d1-114">WorkbookChartAxis</span></span>](chartaxis.md)   |<span data-ttu-id="9c2d1-115">Обновление объекта ChartAxis.</span><span class="sxs-lookup"><span data-stu-id="9c2d1-115">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9c2d1-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="9c2d1-116">Properties</span></span>
| <span data-ttu-id="9c2d1-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="9c2d1-117">Property</span></span>     | <span data-ttu-id="9c2d1-118">Тип</span><span class="sxs-lookup"><span data-stu-id="9c2d1-118">Type</span></span>   |<span data-ttu-id="9c2d1-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9c2d1-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9c2d1-120">id</span><span class="sxs-lookup"><span data-stu-id="9c2d1-120">id</span></span>       |<span data-ttu-id="9c2d1-121">string</span><span class="sxs-lookup"><span data-stu-id="9c2d1-121">string</span></span>   | <span data-ttu-id="9c2d1-122">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="9c2d1-122">Unique identifier.</span></span> <span data-ttu-id="9c2d1-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9c2d1-123">Read-only.</span></span>|
|<span data-ttu-id="9c2d1-124">majorUnit</span><span class="sxs-lookup"><span data-stu-id="9c2d1-124">majorUnit</span></span>|<span data-ttu-id="9c2d1-125">Json</span><span class="sxs-lookup"><span data-stu-id="9c2d1-125">Json</span></span>|<span data-ttu-id="9c2d1-p102">Обозначает интервал между двумя основными делениями. Можно указать в виде числового значения или пустой строки.  Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="9c2d1-p102">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="9c2d1-129">maximum</span><span class="sxs-lookup"><span data-stu-id="9c2d1-129">maximum</span></span>|<span data-ttu-id="9c2d1-130">Json</span><span class="sxs-lookup"><span data-stu-id="9c2d1-130">Json</span></span>|<span data-ttu-id="9c2d1-p103">Представляет максимальное значение на оси значений.  Можно указать в виде числового значения или пустой строки (для автоматически заданных значений оси).  Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="9c2d1-p103">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="9c2d1-134">minimum</span><span class="sxs-lookup"><span data-stu-id="9c2d1-134">minimum</span></span>|<span data-ttu-id="9c2d1-135">Json</span><span class="sxs-lookup"><span data-stu-id="9c2d1-135">Json</span></span>|<span data-ttu-id="9c2d1-p104">Представляет минимальное значение на оси значений. Ему можно присвоить числовое значение или пустую строку (для автоматически заданных значений оси). Всегда возвращает числовое значение.</span><span class="sxs-lookup"><span data-stu-id="9c2d1-p104">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="9c2d1-139">minorUnit</span><span class="sxs-lookup"><span data-stu-id="9c2d1-139">minorUnit</span></span>|<span data-ttu-id="9c2d1-140">Json</span><span class="sxs-lookup"><span data-stu-id="9c2d1-140">Json</span></span>|<span data-ttu-id="9c2d1-p105">Представляет интервал между двумя промежуточными делениями. Можно указать в виде числового значения или пустой строки (для автоматически заданных значений оси). Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="9c2d1-p105">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c2d1-144">Связи</span><span class="sxs-lookup"><span data-stu-id="9c2d1-144">Relationships</span></span>
| <span data-ttu-id="9c2d1-145">Связь</span><span class="sxs-lookup"><span data-stu-id="9c2d1-145">Relationship</span></span> | <span data-ttu-id="9c2d1-146">Тип</span><span class="sxs-lookup"><span data-stu-id="9c2d1-146">Type</span></span>   |<span data-ttu-id="9c2d1-147">Описание</span><span class="sxs-lookup"><span data-stu-id="9c2d1-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c2d1-148">format</span><span class="sxs-lookup"><span data-stu-id="9c2d1-148">format</span></span>|[<span data-ttu-id="9c2d1-149">воркбукчартаксисформат</span><span class="sxs-lookup"><span data-stu-id="9c2d1-149">WorkbookChartAxisFormat</span></span>](chartaxisformat.md)|<span data-ttu-id="9c2d1-p106">Представляет форматирование объекта диаграммы, в том числе форматирование линий и шрифта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9c2d1-p106">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="9c2d1-152">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="9c2d1-152">majorGridlines</span></span>|[<span data-ttu-id="9c2d1-153">воркбукчартгридлинес</span><span class="sxs-lookup"><span data-stu-id="9c2d1-153">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="9c2d1-p107">Возвращает объект Gridlines, который представляет основные линии сетки для указанной оси. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9c2d1-p107">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="9c2d1-156">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="9c2d1-156">minorGridlines</span></span>|[<span data-ttu-id="9c2d1-157">воркбукчартгридлинес</span><span class="sxs-lookup"><span data-stu-id="9c2d1-157">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="9c2d1-p108">Возвращает объект Gridlines, который представляет вспомогательные линии сетки для указанной оси. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9c2d1-p108">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="9c2d1-160">title</span><span class="sxs-lookup"><span data-stu-id="9c2d1-160">title</span></span>|[<span data-ttu-id="9c2d1-161">воркбукчартаксиститле</span><span class="sxs-lookup"><span data-stu-id="9c2d1-161">WorkbookChartAxisTitle</span></span>](chartaxistitle.md)|<span data-ttu-id="9c2d1-162">Обозначает название оси.</span><span class="sxs-lookup"><span data-stu-id="9c2d1-162">Represents the axis title.</span></span> <span data-ttu-id="9c2d1-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9c2d1-163">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9c2d1-164">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9c2d1-164">JSON representation</span></span>

<span data-ttu-id="9c2d1-165">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9c2d1-165">Here is a JSON representation of the resource.</span></span>

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
