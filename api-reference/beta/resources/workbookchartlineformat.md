---
title: Тип ресурса Воркбукчартлинеформат
description: Инкапсулирует параметры форматирования для элементов линий.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: fe36b0448d430566b51ee836e93d02f08cdbdbd5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007244"
---
# <a name="workbookchartlineformat-resource-type"></a><span data-ttu-id="9157b-103">Тип ресурса Воркбукчартлинеформат</span><span class="sxs-lookup"><span data-stu-id="9157b-103">workbookChartLineFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9157b-104">Инкапсулирует параметры форматирования для элементов линий.</span><span class="sxs-lookup"><span data-stu-id="9157b-104">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="9157b-105">Методы</span><span class="sxs-lookup"><span data-stu-id="9157b-105">Methods</span></span>

| <span data-ttu-id="9157b-106">Метод</span><span class="sxs-lookup"><span data-stu-id="9157b-106">Method</span></span>           | <span data-ttu-id="9157b-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9157b-107">Return Type</span></span>    |<span data-ttu-id="9157b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9157b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9157b-109">Получение Воркбукчартлинеформат</span><span class="sxs-lookup"><span data-stu-id="9157b-109">Get workbookChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="9157b-110">Воркбукчартлинеформат</span><span class="sxs-lookup"><span data-stu-id="9157b-110">workbookChartLineFormat</span></span>](workbookchartlineformat.md) |<span data-ttu-id="9157b-111">Чтение свойств и связей объекта chartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="9157b-111">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="9157b-112">Обновление</span><span class="sxs-lookup"><span data-stu-id="9157b-112">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="9157b-113">Воркбукчартлинеформат</span><span class="sxs-lookup"><span data-stu-id="9157b-113">workbookChartLineFormat</span></span>](workbookchartlineformat.md) |<span data-ttu-id="9157b-114">Обновление объекта ChartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="9157b-114">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="9157b-115">Clear</span><span class="sxs-lookup"><span data-stu-id="9157b-115">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="9157b-116">Нет</span><span class="sxs-lookup"><span data-stu-id="9157b-116">None</span></span>|<span data-ttu-id="9157b-117">Очищает формат линий элемента диаграммы.</span><span class="sxs-lookup"><span data-stu-id="9157b-117">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="9157b-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="9157b-118">Properties</span></span>
| <span data-ttu-id="9157b-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="9157b-119">Property</span></span>     | <span data-ttu-id="9157b-120">Тип</span><span class="sxs-lookup"><span data-stu-id="9157b-120">Type</span></span>   |<span data-ttu-id="9157b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9157b-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9157b-122">color</span><span class="sxs-lookup"><span data-stu-id="9157b-122">color</span></span>|<span data-ttu-id="9157b-123">string</span><span class="sxs-lookup"><span data-stu-id="9157b-123">string</span></span>|<span data-ttu-id="9157b-124">HTML-код цвета, представляющий цвет линий в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="9157b-124">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9157b-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="9157b-125">Relationships</span></span>
<span data-ttu-id="9157b-126">Нет</span><span class="sxs-lookup"><span data-stu-id="9157b-126">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9157b-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9157b-127">JSON representation</span></span>

<span data-ttu-id="9157b-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9157b-128">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "workbookChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
