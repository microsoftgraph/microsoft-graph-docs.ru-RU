---
title: Тип ресурса ChartLineFormat
description: Инкапсулирует параметры форматирования для элементов линий.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 7224f7d5d0b41814c17081eefab79de47ca89ebb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533114"
---
# <a name="chartlineformat-resource-type"></a><span data-ttu-id="e1ac6-103">Тип ресурса ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="e1ac6-103">ChartLineFormat resource type</span></span>

<span data-ttu-id="e1ac6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1ac6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e1ac6-105">Инкапсулирует параметры форматирования для элементов линий.</span><span class="sxs-lookup"><span data-stu-id="e1ac6-105">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="e1ac6-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e1ac6-106">Methods</span></span>

| <span data-ttu-id="e1ac6-107">Метод</span><span class="sxs-lookup"><span data-stu-id="e1ac6-107">Method</span></span>           | <span data-ttu-id="e1ac6-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e1ac6-108">Return Type</span></span>    |<span data-ttu-id="e1ac6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e1ac6-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e1ac6-110">Получение объекта ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="e1ac6-110">Get ChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="e1ac6-111">воркбукчартлинеформат</span><span class="sxs-lookup"><span data-stu-id="e1ac6-111">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="e1ac6-112">Чтение свойств и связей объекта chartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="e1ac6-112">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="e1ac6-113">Обновление</span><span class="sxs-lookup"><span data-stu-id="e1ac6-113">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="e1ac6-114">воркбукчартлинеформат</span><span class="sxs-lookup"><span data-stu-id="e1ac6-114">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="e1ac6-115">Обновление объекта ChartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="e1ac6-115">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="e1ac6-116">Clear</span><span class="sxs-lookup"><span data-stu-id="e1ac6-116">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="e1ac6-117">Нет</span><span class="sxs-lookup"><span data-stu-id="e1ac6-117">None</span></span>|<span data-ttu-id="e1ac6-118">Очищает формат линий элемента диаграммы.</span><span class="sxs-lookup"><span data-stu-id="e1ac6-118">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="e1ac6-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="e1ac6-119">Properties</span></span>
| <span data-ttu-id="e1ac6-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1ac6-120">Property</span></span>     | <span data-ttu-id="e1ac6-121">Тип</span><span class="sxs-lookup"><span data-stu-id="e1ac6-121">Type</span></span>   |<span data-ttu-id="e1ac6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e1ac6-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1ac6-123">color</span><span class="sxs-lookup"><span data-stu-id="e1ac6-123">color</span></span>|<span data-ttu-id="e1ac6-124">string</span><span class="sxs-lookup"><span data-stu-id="e1ac6-124">string</span></span>|<span data-ttu-id="e1ac6-125">HTML-код цвета, представляющий цвет линий в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="e1ac6-125">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1ac6-126">Связи</span><span class="sxs-lookup"><span data-stu-id="e1ac6-126">Relationships</span></span>
<span data-ttu-id="e1ac6-127">Нет</span><span class="sxs-lookup"><span data-stu-id="e1ac6-127">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e1ac6-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e1ac6-128">JSON representation</span></span>

<span data-ttu-id="e1ac6-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1ac6-129">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartLineFormat"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
