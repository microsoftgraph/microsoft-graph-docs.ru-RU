---
title: Тип ресурса Воркбукчартаксис
description: Представляет одну ось на диаграмме.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 929fd2569067e67af6770b9281bce1d09cd9eca4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007377"
---
# <a name="workbookchartaxis-resource-type"></a><span data-ttu-id="1c612-103">Тип ресурса Воркбукчартаксис</span><span class="sxs-lookup"><span data-stu-id="1c612-103">workbookChartAxis resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c612-104">Представляет одну ось на диаграмме.</span><span class="sxs-lookup"><span data-stu-id="1c612-104">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="1c612-105">Методы</span><span class="sxs-lookup"><span data-stu-id="1c612-105">Methods</span></span>

| <span data-ttu-id="1c612-106">Метод</span><span class="sxs-lookup"><span data-stu-id="1c612-106">Method</span></span>           | <span data-ttu-id="1c612-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1c612-107">Return Type</span></span>    |<span data-ttu-id="1c612-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1c612-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1c612-109">Получение объекта ChartAxis</span><span class="sxs-lookup"><span data-stu-id="1c612-109">Get ChartAxis</span></span>](../api/chartaxis-get.md) | [<span data-ttu-id="1c612-110">Воркбукчартаксис</span><span class="sxs-lookup"><span data-stu-id="1c612-110">workbookChartAxis</span></span>](workbookchartaxis.md) |<span data-ttu-id="1c612-111">Чтение свойств и связей объекта chartAxis.</span><span class="sxs-lookup"><span data-stu-id="1c612-111">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="1c612-112">Обновление</span><span class="sxs-lookup"><span data-stu-id="1c612-112">Update</span></span>](../api/chartaxis-update.md) | [<span data-ttu-id="1c612-113">Воркбукчартаксис</span><span class="sxs-lookup"><span data-stu-id="1c612-113">workbookChartAxis</span></span>](workbookchartaxis.md)   |<span data-ttu-id="1c612-114">Обновление объекта ChartAxis.</span><span class="sxs-lookup"><span data-stu-id="1c612-114">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1c612-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="1c612-115">Properties</span></span>
| <span data-ttu-id="1c612-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="1c612-116">Property</span></span>     | <span data-ttu-id="1c612-117">Тип</span><span class="sxs-lookup"><span data-stu-id="1c612-117">Type</span></span>   |<span data-ttu-id="1c612-118">Описание</span><span class="sxs-lookup"><span data-stu-id="1c612-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1c612-119">id</span><span class="sxs-lookup"><span data-stu-id="1c612-119">id</span></span>       |<span data-ttu-id="1c612-120">string</span><span class="sxs-lookup"><span data-stu-id="1c612-120">string</span></span>   | <span data-ttu-id="1c612-121">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="1c612-121">Unique identifier.</span></span> <span data-ttu-id="1c612-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1c612-122">Read-only.</span></span>|
|<span data-ttu-id="1c612-123">majorUnit</span><span class="sxs-lookup"><span data-stu-id="1c612-123">majorUnit</span></span>|<span data-ttu-id="1c612-124">Json</span><span class="sxs-lookup"><span data-stu-id="1c612-124">Json</span></span>|<span data-ttu-id="1c612-p102">Обозначает интервал между двумя основными делениями. Можно указать в виде числового значения или пустой строки.  Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="1c612-p102">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="1c612-128">maximum</span><span class="sxs-lookup"><span data-stu-id="1c612-128">maximum</span></span>|<span data-ttu-id="1c612-129">Json</span><span class="sxs-lookup"><span data-stu-id="1c612-129">Json</span></span>|<span data-ttu-id="1c612-p103">Представляет максимальное значение на оси значений.  Можно указать в виде числового значения или пустой строки (для автоматически заданных значений оси).  Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="1c612-p103">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="1c612-133">minimum</span><span class="sxs-lookup"><span data-stu-id="1c612-133">minimum</span></span>|<span data-ttu-id="1c612-134">Json</span><span class="sxs-lookup"><span data-stu-id="1c612-134">Json</span></span>|<span data-ttu-id="1c612-p104">Представляет минимальное значение на оси значений. Ему можно присвоить числовое значение или пустую строку (для автоматически заданных значений оси). Всегда возвращает числовое значение.</span><span class="sxs-lookup"><span data-stu-id="1c612-p104">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="1c612-138">minorUnit</span><span class="sxs-lookup"><span data-stu-id="1c612-138">minorUnit</span></span>|<span data-ttu-id="1c612-139">Json</span><span class="sxs-lookup"><span data-stu-id="1c612-139">Json</span></span>|<span data-ttu-id="1c612-p105">Представляет интервал между двумя промежуточными делениями. Можно указать в виде числового значения или пустой строки (для автоматически заданных значений оси). Возвращаемое значение всегда является числом.</span><span class="sxs-lookup"><span data-stu-id="1c612-p105">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c612-143">Отношения</span><span class="sxs-lookup"><span data-stu-id="1c612-143">Relationships</span></span>
| <span data-ttu-id="1c612-144">Отношение</span><span class="sxs-lookup"><span data-stu-id="1c612-144">Relationship</span></span> | <span data-ttu-id="1c612-145">Тип</span><span class="sxs-lookup"><span data-stu-id="1c612-145">Type</span></span>   |<span data-ttu-id="1c612-146">Описание</span><span class="sxs-lookup"><span data-stu-id="1c612-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1c612-147">format</span><span class="sxs-lookup"><span data-stu-id="1c612-147">format</span></span>|[<span data-ttu-id="1c612-148">Воркбукчартаксисформат</span><span class="sxs-lookup"><span data-stu-id="1c612-148">workbookChartAxisFormat</span></span>](workbookchartaxisformat.md)|<span data-ttu-id="1c612-p106">Представляет форматирование объекта диаграммы, в том числе форматирование линий и шрифта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1c612-p106">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="1c612-151">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="1c612-151">majorGridlines</span></span>|[<span data-ttu-id="1c612-152">Воркбукчартгридлинес</span><span class="sxs-lookup"><span data-stu-id="1c612-152">workbookChartGridlines</span></span>](workbookchartgridlines.md)|<span data-ttu-id="1c612-p107">Возвращает объект Gridlines, который представляет основные линии сетки для указанной оси. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1c612-p107">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="1c612-155">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="1c612-155">minorGridlines</span></span>|[<span data-ttu-id="1c612-156">Воркбукчартгридлинес</span><span class="sxs-lookup"><span data-stu-id="1c612-156">workbookChartGridlines</span></span>](workbookchartgridlines.md)|<span data-ttu-id="1c612-p108">Возвращает объект Gridlines, который представляет вспомогательные линии сетки для указанной оси. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1c612-p108">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="1c612-159">title</span><span class="sxs-lookup"><span data-stu-id="1c612-159">title</span></span>|[<span data-ttu-id="1c612-160">Воркбукчартаксиститле</span><span class="sxs-lookup"><span data-stu-id="1c612-160">workbookChartAxisTitle</span></span>](workbookchartaxistitle.md)|<span data-ttu-id="1c612-161">Обозначает название оси.</span><span class="sxs-lookup"><span data-stu-id="1c612-161">Represents the axis title.</span></span> <span data-ttu-id="1c612-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1c612-162">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1c612-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1c612-163">JSON representation</span></span>

<span data-ttu-id="1c612-164">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1c612-164">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "title",
    "minorGridlines",
    "majorGridlines",
    "format"
   ],
  "keyProperty": "id",
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
  "suppressions": []
}
-->
