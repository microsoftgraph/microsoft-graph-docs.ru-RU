---
title: Тип ресурса ChartTitle
description: Представляет объект заголовка диаграммы.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 6cf6a2e6355fc4bc8955899dde48f9cc843e920c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879417"
---
# <a name="charttitle-resource-type"></a><span data-ttu-id="0c200-103">Тип ресурса ChartTitle</span><span class="sxs-lookup"><span data-stu-id="0c200-103">ChartTitle resource type</span></span>

<span data-ttu-id="0c200-104">Представляет объект заголовка диаграммы.</span><span class="sxs-lookup"><span data-stu-id="0c200-104">Represents a chart title object of a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="0c200-105">Методы</span><span class="sxs-lookup"><span data-stu-id="0c200-105">Methods</span></span>

| <span data-ttu-id="0c200-106">Метод</span><span class="sxs-lookup"><span data-stu-id="0c200-106">Method</span></span>           | <span data-ttu-id="0c200-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0c200-107">Return Type</span></span>    |<span data-ttu-id="0c200-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0c200-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0c200-109">Получение объекта ChartTitle</span><span class="sxs-lookup"><span data-stu-id="0c200-109">Get ChartTitle</span></span>](../api/charttitle-get.md) | [<span data-ttu-id="0c200-110">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="0c200-110">WorkbookChartTitle</span></span>](charttitle.md) |<span data-ttu-id="0c200-111">Чтение свойств и связей объекта chartTitle.</span><span class="sxs-lookup"><span data-stu-id="0c200-111">Read properties and relationships of chartTitle object.</span></span>|
|<span data-ttu-id="0c200-112">[обновление](../api/charttitle-update.md).</span><span class="sxs-lookup"><span data-stu-id="0c200-112">[Update](../api/charttitle-update.md)</span></span> | [<span data-ttu-id="0c200-113">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="0c200-113">WorkbookChartTitle</span></span>](charttitle.md)    |<span data-ttu-id="0c200-114">Обновление объекта ChartTitle.</span><span class="sxs-lookup"><span data-stu-id="0c200-114">Update ChartTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0c200-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="0c200-115">Properties</span></span>
| <span data-ttu-id="0c200-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c200-116">Property</span></span>     | <span data-ttu-id="0c200-117">Тип</span><span class="sxs-lookup"><span data-stu-id="0c200-117">Type</span></span>   |<span data-ttu-id="0c200-118">Описание</span><span class="sxs-lookup"><span data-stu-id="0c200-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c200-119">overlay</span><span class="sxs-lookup"><span data-stu-id="0c200-119">overlay</span></span>|<span data-ttu-id="0c200-120">boolean</span><span class="sxs-lookup"><span data-stu-id="0c200-120">boolean</span></span>|<span data-ttu-id="0c200-121">Логическое значение, указывающее, отображается ли заголовок диаграммы поверх нее.</span><span class="sxs-lookup"><span data-stu-id="0c200-121">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="0c200-122">text</span><span class="sxs-lookup"><span data-stu-id="0c200-122">text</span></span>|<span data-ttu-id="0c200-123">строка</span><span class="sxs-lookup"><span data-stu-id="0c200-123">string</span></span>|<span data-ttu-id="0c200-124">Представляет текст заголовка диаграммы.</span><span class="sxs-lookup"><span data-stu-id="0c200-124">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="0c200-125">visible</span><span class="sxs-lookup"><span data-stu-id="0c200-125">visible</span></span>|<span data-ttu-id="0c200-126">boolean</span><span class="sxs-lookup"><span data-stu-id="0c200-126">boolean</span></span>|<span data-ttu-id="0c200-127">Логическое значение, представляющее видимость объекта заголовка диаграммы.</span><span class="sxs-lookup"><span data-stu-id="0c200-127">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c200-128">Связи</span><span class="sxs-lookup"><span data-stu-id="0c200-128">Relationships</span></span>
| <span data-ttu-id="0c200-129">Связь</span><span class="sxs-lookup"><span data-stu-id="0c200-129">Relationship</span></span> | <span data-ttu-id="0c200-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0c200-130">Type</span></span>   |<span data-ttu-id="0c200-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0c200-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c200-132">format</span><span class="sxs-lookup"><span data-stu-id="0c200-132">format</span></span>|[<span data-ttu-id="0c200-133">WorkbookChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="0c200-133">WorkbookChartTitleFormat</span></span>](charttitleformat.md)|<span data-ttu-id="0c200-p101">Представляет форматирование названия диаграммы, включая формат заливки и шрифта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0c200-p101">Represents the formatting of a chart title, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0c200-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0c200-136">JSON representation</span></span>

<span data-ttu-id="0c200-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c200-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartTitle"
}-->

```json
{
  "overlay": true,
  "text": "string",
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
