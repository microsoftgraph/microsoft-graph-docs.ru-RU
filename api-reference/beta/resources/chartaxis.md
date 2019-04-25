---
title: Тип ресурса ChartAxis
description: Представляет одну ось на диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6cb780272887b6a9b637bbec24b68b37db93657e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535588"
---
# <a name="chartaxis-resource-type"></a><span data-ttu-id="53be9-103">Тип ресурса ChartAxis</span><span class="sxs-lookup"><span data-stu-id="53be9-103">ChartAxis resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53be9-104">Представляет одну ось на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="53be9-104">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="53be9-105">Методы</span><span class="sxs-lookup"><span data-stu-id="53be9-105">Methods</span></span>

| <span data-ttu-id="53be9-106">Метод</span><span class="sxs-lookup"><span data-stu-id="53be9-106">Method</span></span>           | <span data-ttu-id="53be9-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="53be9-107">Return Type</span></span>    |<span data-ttu-id="53be9-108">Описание</span><span class="sxs-lookup"><span data-stu-id="53be9-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="53be9-109">Получение объекта ChartAxis</span><span class="sxs-lookup"><span data-stu-id="53be9-109">Get ChartAxis</span></span>](../api/chartaxis-get.md) | [<span data-ttu-id="53be9-110">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="53be9-110">ChartAxis</span></span>](chartaxis.md) |<span data-ttu-id="53be9-111">Чтение свойств и связей объекта chartAxis.</span><span class="sxs-lookup"><span data-stu-id="53be9-111">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="53be9-112">Обновление</span><span class="sxs-lookup"><span data-stu-id="53be9-112">Update</span></span>](../api/chartaxis-update.md) | [<span data-ttu-id="53be9-113">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="53be9-113">ChartAxis</span></span>](chartaxis.md)   |<span data-ttu-id="53be9-114">Обновление объекта ChartAxis.</span><span class="sxs-lookup"><span data-stu-id="53be9-114">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="53be9-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="53be9-115">Properties</span></span>
| <span data-ttu-id="53be9-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="53be9-116">Property</span></span>     | <span data-ttu-id="53be9-117">Тип</span><span class="sxs-lookup"><span data-stu-id="53be9-117">Type</span></span>   |<span data-ttu-id="53be9-118">Описание</span><span class="sxs-lookup"><span data-stu-id="53be9-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53be9-119">majorUnit</span><span class="sxs-lookup"><span data-stu-id="53be9-119">majorUnit</span></span>|<span data-ttu-id="53be9-120">объект</span><span class="sxs-lookup"><span data-stu-id="53be9-120">object</span></span>|<span data-ttu-id="53be9-p101">Обозначает интервал между двумя основными делениями. Можно указать в виде числового значения или пустой строки.  Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="53be9-p101">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="53be9-124">maximum</span><span class="sxs-lookup"><span data-stu-id="53be9-124">maximum</span></span>|<span data-ttu-id="53be9-125">объект</span><span class="sxs-lookup"><span data-stu-id="53be9-125">object</span></span>|<span data-ttu-id="53be9-p102">Представляет максимальное значение на оси значений.  Можно указать в виде числового значения или пустой строки (для автоматически заданных значений оси).  Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="53be9-p102">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="53be9-129">minimum</span><span class="sxs-lookup"><span data-stu-id="53be9-129">minimum</span></span>|<span data-ttu-id="53be9-130">объект</span><span class="sxs-lookup"><span data-stu-id="53be9-130">object</span></span>|<span data-ttu-id="53be9-p103">Представляет минимальное значение на оси значений. Ему можно присвоить числовое значение или пустую строку (для автоматически заданных значений оси). Всегда возвращает числовое значение.</span><span class="sxs-lookup"><span data-stu-id="53be9-p103">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="53be9-134">minorUnit</span><span class="sxs-lookup"><span data-stu-id="53be9-134">minorUnit</span></span>|<span data-ttu-id="53be9-135">object</span><span class="sxs-lookup"><span data-stu-id="53be9-135">object</span></span>|<span data-ttu-id="53be9-p104">Представляет интервал между двумя промежуточными делениями. Можно указать в виде числового значения или пустой строки (для автоматически заданных значений оси). Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="53be9-p104">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="53be9-139">Связи</span><span class="sxs-lookup"><span data-stu-id="53be9-139">Relationships</span></span>
| <span data-ttu-id="53be9-140">Отношение</span><span class="sxs-lookup"><span data-stu-id="53be9-140">Relationship</span></span> | <span data-ttu-id="53be9-141">Тип</span><span class="sxs-lookup"><span data-stu-id="53be9-141">Type</span></span>   |<span data-ttu-id="53be9-142">Описание</span><span class="sxs-lookup"><span data-stu-id="53be9-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53be9-143">format</span><span class="sxs-lookup"><span data-stu-id="53be9-143">format</span></span>|[<span data-ttu-id="53be9-144">ChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="53be9-144">ChartAxisFormat</span></span>](chartaxisformat.md)|<span data-ttu-id="53be9-p105">Представляет форматирование объекта диаграммы, в том числе форматирование линий и шрифта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="53be9-p105">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="53be9-147">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="53be9-147">majorGridlines</span></span>|[<span data-ttu-id="53be9-148">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="53be9-148">ChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="53be9-p106">Возвращает объект Gridlines, который представляет основные линии сетки для указанной оси. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="53be9-p106">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="53be9-151">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="53be9-151">minorGridlines</span></span>|[<span data-ttu-id="53be9-152">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="53be9-152">ChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="53be9-p107">Возвращает объект Gridlines, который представляет вспомогательные линии сетки для указанной оси. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="53be9-p107">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="53be9-155">title</span><span class="sxs-lookup"><span data-stu-id="53be9-155">title</span></span>|[<span data-ttu-id="53be9-156">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="53be9-156">ChartAxisTitle</span></span>](chartaxistitle.md)|<span data-ttu-id="53be9-p108">Представляет название оси. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="53be9-p108">Represents the axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="53be9-159">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="53be9-159">JSON representation</span></span>

<span data-ttu-id="53be9-160">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53be9-160">Here is a JSON representation of the resource.</span></span>

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
