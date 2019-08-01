---
title: Тип ресурса ChartAxis
description: Представляет одну ось на диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 77d688d71757cac9f6d58b9d1bc344d37550e3a3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033019"
---
# <a name="chartaxis-resource-type"></a><span data-ttu-id="16c86-103">Тип ресурса ChartAxis</span><span class="sxs-lookup"><span data-stu-id="16c86-103">ChartAxis resource type</span></span>

<span data-ttu-id="16c86-104">Представляет одну ось на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="16c86-104">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="16c86-105">Методы</span><span class="sxs-lookup"><span data-stu-id="16c86-105">Methods</span></span>

| <span data-ttu-id="16c86-106">Метод</span><span class="sxs-lookup"><span data-stu-id="16c86-106">Method</span></span>           | <span data-ttu-id="16c86-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="16c86-107">Return Type</span></span>    |<span data-ttu-id="16c86-108">Описание</span><span class="sxs-lookup"><span data-stu-id="16c86-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="16c86-109">Получение объекта ChartAxis</span><span class="sxs-lookup"><span data-stu-id="16c86-109">Get ChartAxis</span></span>](../api/chartaxis-get.md) | [<span data-ttu-id="16c86-110">Воркбукчартаксис</span><span class="sxs-lookup"><span data-stu-id="16c86-110">WorkbookChartAxis</span></span>](chartaxis.md) |<span data-ttu-id="16c86-111">Чтение свойств и связей объекта chartAxis.</span><span class="sxs-lookup"><span data-stu-id="16c86-111">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="16c86-112">Обновление</span><span class="sxs-lookup"><span data-stu-id="16c86-112">Update</span></span>](../api/chartaxis-update.md) | [<span data-ttu-id="16c86-113">Воркбукчартаксис</span><span class="sxs-lookup"><span data-stu-id="16c86-113">WorkbookChartAxis</span></span>](chartaxis.md)   |<span data-ttu-id="16c86-114">Обновление объекта ChartAxis.</span><span class="sxs-lookup"><span data-stu-id="16c86-114">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="16c86-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="16c86-115">Properties</span></span>
| <span data-ttu-id="16c86-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="16c86-116">Property</span></span>     | <span data-ttu-id="16c86-117">Тип</span><span class="sxs-lookup"><span data-stu-id="16c86-117">Type</span></span>   |<span data-ttu-id="16c86-118">Описание</span><span class="sxs-lookup"><span data-stu-id="16c86-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="16c86-119">id</span><span class="sxs-lookup"><span data-stu-id="16c86-119">id</span></span>       |<span data-ttu-id="16c86-120">string</span><span class="sxs-lookup"><span data-stu-id="16c86-120">string</span></span>   | <span data-ttu-id="16c86-121">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="16c86-121">Unique identifier.</span></span> <span data-ttu-id="16c86-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="16c86-122">Read-only.</span></span>|
|<span data-ttu-id="16c86-123">majorUnit</span><span class="sxs-lookup"><span data-stu-id="16c86-123">majorUnit</span></span>|<span data-ttu-id="16c86-124">Json</span><span class="sxs-lookup"><span data-stu-id="16c86-124">Json</span></span>|<span data-ttu-id="16c86-p102">Обозначает интервал между двумя основными делениями. Можно указать в виде числового значения или пустой строки.  Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="16c86-p102">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="16c86-128">maximum</span><span class="sxs-lookup"><span data-stu-id="16c86-128">maximum</span></span>|<span data-ttu-id="16c86-129">Json</span><span class="sxs-lookup"><span data-stu-id="16c86-129">Json</span></span>|<span data-ttu-id="16c86-p103">Представляет максимальное значение на оси значений.  Можно указать в виде числового значения или пустой строки (для автоматически заданных значений оси).  Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="16c86-p103">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="16c86-133">minimum</span><span class="sxs-lookup"><span data-stu-id="16c86-133">minimum</span></span>|<span data-ttu-id="16c86-134">Json</span><span class="sxs-lookup"><span data-stu-id="16c86-134">Json</span></span>|<span data-ttu-id="16c86-p104">Представляет минимальное значение на оси значений. Ему можно присвоить числовое значение или пустую строку (для автоматически заданных значений оси). Всегда возвращает числовое значение.</span><span class="sxs-lookup"><span data-stu-id="16c86-p104">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="16c86-138">minorUnit</span><span class="sxs-lookup"><span data-stu-id="16c86-138">minorUnit</span></span>|<span data-ttu-id="16c86-139">Json</span><span class="sxs-lookup"><span data-stu-id="16c86-139">Json</span></span>|<span data-ttu-id="16c86-p105">Представляет интервал между двумя промежуточными делениями. Можно указать в виде числового значения или пустой строки (для автоматически заданных значений оси). Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="16c86-p105">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="16c86-143">Отношения</span><span class="sxs-lookup"><span data-stu-id="16c86-143">Relationships</span></span>
| <span data-ttu-id="16c86-144">Отношение</span><span class="sxs-lookup"><span data-stu-id="16c86-144">Relationship</span></span> | <span data-ttu-id="16c86-145">Тип</span><span class="sxs-lookup"><span data-stu-id="16c86-145">Type</span></span>   |<span data-ttu-id="16c86-146">Описание</span><span class="sxs-lookup"><span data-stu-id="16c86-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16c86-147">format</span><span class="sxs-lookup"><span data-stu-id="16c86-147">format</span></span>|[<span data-ttu-id="16c86-148">Воркбукчартаксисформат</span><span class="sxs-lookup"><span data-stu-id="16c86-148">WorkbookChartAxisFormat</span></span>](chartaxisformat.md)|<span data-ttu-id="16c86-p106">Представляет форматирование объекта диаграммы, в том числе форматирование линий и шрифта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="16c86-p106">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="16c86-151">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="16c86-151">majorGridlines</span></span>|[<span data-ttu-id="16c86-152">Воркбукчартгридлинес</span><span class="sxs-lookup"><span data-stu-id="16c86-152">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="16c86-p107">Возвращает объект Gridlines, который представляет основные линии сетки для указанной оси. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="16c86-p107">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="16c86-155">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="16c86-155">minorGridlines</span></span>|[<span data-ttu-id="16c86-156">Воркбукчартгридлинес</span><span class="sxs-lookup"><span data-stu-id="16c86-156">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="16c86-p108">Возвращает объект Gridlines, который представляет вспомогательные линии сетки для указанной оси. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="16c86-p108">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="16c86-159">title</span><span class="sxs-lookup"><span data-stu-id="16c86-159">title</span></span>|[<span data-ttu-id="16c86-160">Воркбукчартаксиститле</span><span class="sxs-lookup"><span data-stu-id="16c86-160">WorkbookChartAxisTitle</span></span>](chartaxistitle.md)|<span data-ttu-id="16c86-161">Обозначает название оси.</span><span class="sxs-lookup"><span data-stu-id="16c86-161">Represents the axis title.</span></span> <span data-ttu-id="16c86-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="16c86-162">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="16c86-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="16c86-163">JSON representation</span></span>

<span data-ttu-id="16c86-164">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="16c86-164">Here is a JSON representation of the resource.</span></span>

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
