---
title: Тип ресурса ChartAxis
description: Представляет одну ось на диаграмме.
ms.openlocfilehash: f92e8dd12dc2d7036d5022e2b293cfc290faf910
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079262"
---
# <a name="chartaxis-resource-type"></a><span data-ttu-id="ab309-103">Тип ресурса ChartAxis</span><span class="sxs-lookup"><span data-stu-id="ab309-103">ChartAxis resource type</span></span>

> <span data-ttu-id="ab309-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ab309-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab309-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab309-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ab309-106">Представляет одну ось на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="ab309-106">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="ab309-107">Методы</span><span class="sxs-lookup"><span data-stu-id="ab309-107">Methods</span></span>

| <span data-ttu-id="ab309-108">Метод</span><span class="sxs-lookup"><span data-stu-id="ab309-108">Method</span></span>           | <span data-ttu-id="ab309-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ab309-109">Return Type</span></span>    |<span data-ttu-id="ab309-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ab309-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ab309-111">Получение объекта ChartAxis</span><span class="sxs-lookup"><span data-stu-id="ab309-111">Get ChartAxis</span></span>](../api/chartaxis-get.md) | [<span data-ttu-id="ab309-112">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="ab309-112">ChartAxis</span></span>](chartaxis.md) |<span data-ttu-id="ab309-113">Чтение свойств и связей объекта chartAxis.</span><span class="sxs-lookup"><span data-stu-id="ab309-113">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="ab309-114">Update</span><span class="sxs-lookup"><span data-stu-id="ab309-114">Update</span></span>](../api/chartaxis-update.md) | [<span data-ttu-id="ab309-115">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="ab309-115">ChartAxis</span></span>](chartaxis.md)   |<span data-ttu-id="ab309-116">Обновление объекта ChartAxis.</span><span class="sxs-lookup"><span data-stu-id="ab309-116">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ab309-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="ab309-117">Properties</span></span>
| <span data-ttu-id="ab309-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab309-118">Property</span></span>     | <span data-ttu-id="ab309-119">Тип</span><span class="sxs-lookup"><span data-stu-id="ab309-119">Type</span></span>   |<span data-ttu-id="ab309-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ab309-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ab309-121">majorUnit</span><span class="sxs-lookup"><span data-stu-id="ab309-121">majorUnit</span></span>|<span data-ttu-id="ab309-122">object</span><span class="sxs-lookup"><span data-stu-id="ab309-122">object</span></span>|<span data-ttu-id="ab309-p102">Обозначает интервал между двумя основными делениями. Можно указать в виде числового значения или пустой строки.  Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="ab309-p102">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="ab309-126">maximum</span><span class="sxs-lookup"><span data-stu-id="ab309-126">maximum</span></span>|<span data-ttu-id="ab309-127">object</span><span class="sxs-lookup"><span data-stu-id="ab309-127">object</span></span>|<span data-ttu-id="ab309-p103">Представляет максимальное значение на оси значений.  Можно указать в виде числового значения или пустой строки (для автоматически заданных значений оси).  Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="ab309-p103">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="ab309-131">minimum</span><span class="sxs-lookup"><span data-stu-id="ab309-131">minimum</span></span>|<span data-ttu-id="ab309-132">object</span><span class="sxs-lookup"><span data-stu-id="ab309-132">object</span></span>|<span data-ttu-id="ab309-p104">Представляет минимальное значение на оси значений. Ему можно присвоить числовое значение или пустую строку (для автоматически заданных значений оси). Всегда возвращает числовое значение.</span><span class="sxs-lookup"><span data-stu-id="ab309-p104">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="ab309-136">minorUnit</span><span class="sxs-lookup"><span data-stu-id="ab309-136">minorUnit</span></span>|<span data-ttu-id="ab309-137">object</span><span class="sxs-lookup"><span data-stu-id="ab309-137">object</span></span>|<span data-ttu-id="ab309-p105">Представляет интервал между двумя промежуточными делениями. Можно указать в виде числового значения или пустой строки (для автоматически заданных значений оси). Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="ab309-p105">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab309-141">Связи</span><span class="sxs-lookup"><span data-stu-id="ab309-141">Relationships</span></span>
| <span data-ttu-id="ab309-142">Связь</span><span class="sxs-lookup"><span data-stu-id="ab309-142">Relationship</span></span> | <span data-ttu-id="ab309-143">Тип</span><span class="sxs-lookup"><span data-stu-id="ab309-143">Type</span></span>   |<span data-ttu-id="ab309-144">Описание</span><span class="sxs-lookup"><span data-stu-id="ab309-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ab309-145">format</span><span class="sxs-lookup"><span data-stu-id="ab309-145">format</span></span>|[<span data-ttu-id="ab309-146">ChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="ab309-146">ChartAxisFormat</span></span>](chartaxisformat.md)|<span data-ttu-id="ab309-p106">Представляет форматирование объекта диаграммы, в том числе форматирование линий и шрифта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab309-p106">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="ab309-149">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="ab309-149">majorGridlines</span></span>|[<span data-ttu-id="ab309-150">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="ab309-150">ChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="ab309-p107">Возвращает объект Gridlines, который представляет основные линии сетки для указанной оси. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab309-p107">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="ab309-153">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="ab309-153">minorGridlines</span></span>|[<span data-ttu-id="ab309-154">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="ab309-154">ChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="ab309-p108">Возвращает объект Gridlines, который представляет вспомогательные линии сетки для указанной оси. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab309-p108">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="ab309-157">должности.</span><span class="sxs-lookup"><span data-stu-id="ab309-157">title</span></span>|[<span data-ttu-id="ab309-158">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="ab309-158">ChartAxisTitle</span></span>](chartaxistitle.md)|<span data-ttu-id="ab309-p109">Представляет название оси. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab309-p109">Represents the axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ab309-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ab309-161">JSON representation</span></span>

<span data-ttu-id="ab309-162">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab309-162">Here is a JSON representation of the resource.</span></span>

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