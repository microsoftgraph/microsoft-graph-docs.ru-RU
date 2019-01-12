---
title: Тип ресурса ChartAxis
description: Представляет одну ось на диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c6344f2bbb102e2e2402dba267538cb46d4c0fbe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914194"
---
# <a name="chartaxis-resource-type"></a><span data-ttu-id="f2774-103">Тип ресурса ChartAxis</span><span class="sxs-lookup"><span data-stu-id="f2774-103">ChartAxis resource type</span></span>

> <span data-ttu-id="f2774-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f2774-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2774-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2774-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f2774-106">Представляет одну ось на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="f2774-106">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="f2774-107">Методы</span><span class="sxs-lookup"><span data-stu-id="f2774-107">Methods</span></span>

| <span data-ttu-id="f2774-108">Метод</span><span class="sxs-lookup"><span data-stu-id="f2774-108">Method</span></span>           | <span data-ttu-id="f2774-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f2774-109">Return Type</span></span>    |<span data-ttu-id="f2774-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f2774-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f2774-111">Получение объекта ChartAxis</span><span class="sxs-lookup"><span data-stu-id="f2774-111">Get ChartAxis</span></span>](../api/chartaxis-get.md) | [<span data-ttu-id="f2774-112">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="f2774-112">ChartAxis</span></span>](chartaxis.md) |<span data-ttu-id="f2774-113">Чтение свойств и связей объекта chartAxis.</span><span class="sxs-lookup"><span data-stu-id="f2774-113">Read properties and relationships of chartAxis object.</span></span>|
|<span data-ttu-id="f2774-114">[обновление](../api/chartaxis-update.md).</span><span class="sxs-lookup"><span data-stu-id="f2774-114">[Update](../api/chartaxis-update.md)</span></span> | [<span data-ttu-id="f2774-115">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="f2774-115">ChartAxis</span></span>](chartaxis.md)   |<span data-ttu-id="f2774-116">Обновление объекта ChartAxis.</span><span class="sxs-lookup"><span data-stu-id="f2774-116">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f2774-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="f2774-117">Properties</span></span>
| <span data-ttu-id="f2774-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="f2774-118">Property</span></span>     | <span data-ttu-id="f2774-119">Тип</span><span class="sxs-lookup"><span data-stu-id="f2774-119">Type</span></span>   |<span data-ttu-id="f2774-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f2774-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2774-121">majorUnit</span><span class="sxs-lookup"><span data-stu-id="f2774-121">majorUnit</span></span>|<span data-ttu-id="f2774-122">object</span><span class="sxs-lookup"><span data-stu-id="f2774-122">object</span></span>|<span data-ttu-id="f2774-p102">Обозначает интервал между двумя основными делениями. Можно указать в виде числового значения или пустой строки.  Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="f2774-p102">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="f2774-126">maximum</span><span class="sxs-lookup"><span data-stu-id="f2774-126">maximum</span></span>|<span data-ttu-id="f2774-127">object</span><span class="sxs-lookup"><span data-stu-id="f2774-127">object</span></span>|<span data-ttu-id="f2774-p103">Представляет максимальное значение на оси значений.  Можно указать в виде числового значения или пустой строки (для автоматически заданных значений оси).  Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="f2774-p103">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="f2774-131">minimum</span><span class="sxs-lookup"><span data-stu-id="f2774-131">minimum</span></span>|<span data-ttu-id="f2774-132">object</span><span class="sxs-lookup"><span data-stu-id="f2774-132">object</span></span>|<span data-ttu-id="f2774-p104">Представляет минимальное значение на оси значений. Ему можно присвоить числовое значение или пустую строку (для автоматически заданных значений оси). Всегда возвращает числовое значение.</span><span class="sxs-lookup"><span data-stu-id="f2774-p104">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="f2774-136">minorUnit</span><span class="sxs-lookup"><span data-stu-id="f2774-136">minorUnit</span></span>|<span data-ttu-id="f2774-137">object</span><span class="sxs-lookup"><span data-stu-id="f2774-137">object</span></span>|<span data-ttu-id="f2774-p105">Представляет интервал между двумя промежуточными делениями. Можно указать в виде числового значения или пустой строки (для автоматически заданных значений оси). Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="f2774-p105">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2774-141">Связи</span><span class="sxs-lookup"><span data-stu-id="f2774-141">Relationships</span></span>
| <span data-ttu-id="f2774-142">Связь</span><span class="sxs-lookup"><span data-stu-id="f2774-142">Relationship</span></span> | <span data-ttu-id="f2774-143">Тип</span><span class="sxs-lookup"><span data-stu-id="f2774-143">Type</span></span>   |<span data-ttu-id="f2774-144">Описание</span><span class="sxs-lookup"><span data-stu-id="f2774-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2774-145">format</span><span class="sxs-lookup"><span data-stu-id="f2774-145">format</span></span>|[<span data-ttu-id="f2774-146">ChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="f2774-146">ChartAxisFormat</span></span>](chartaxisformat.md)|<span data-ttu-id="f2774-p106">Представляет форматирование объекта диаграммы, в том числе форматирование линий и шрифта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f2774-p106">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="f2774-149">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="f2774-149">majorGridlines</span></span>|[<span data-ttu-id="f2774-150">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="f2774-150">ChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="f2774-p107">Возвращает объект Gridlines, который представляет основные линии сетки для указанной оси. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f2774-p107">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="f2774-153">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="f2774-153">minorGridlines</span></span>|[<span data-ttu-id="f2774-154">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="f2774-154">ChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="f2774-p108">Возвращает объект Gridlines, который представляет вспомогательные линии сетки для указанной оси. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f2774-p108">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="f2774-157">должности.</span><span class="sxs-lookup"><span data-stu-id="f2774-157">title</span></span>|[<span data-ttu-id="f2774-158">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="f2774-158">ChartAxisTitle</span></span>](chartaxistitle.md)|<span data-ttu-id="f2774-p109">Представляет название оси. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f2774-p109">Represents the axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f2774-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f2774-161">JSON representation</span></span>

<span data-ttu-id="f2774-162">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f2774-162">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartaxis"
}-->

```json
{
  "majorUnit": "string",
  "maximum": "string",
  "minimum": "string",
  "minorUnit": "string"
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
