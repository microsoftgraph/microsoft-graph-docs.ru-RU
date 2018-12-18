---
title: Тип ресурса ChartGridlines
description: Представляет основные или вспомогательные линии сетки на оси диаграммы.
author: lumine2008
ms.openlocfilehash: 2aaf044b09d061af4853e76e0f2ba118bd1b2321
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353034"
---
# <a name="chartgridlines-resource-type"></a><span data-ttu-id="012aa-103">Тип ресурса ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="012aa-103">ChartGridlines resource type</span></span>

<span data-ttu-id="012aa-104">Представляет основные или вспомогательные линии сетки на оси диаграммы.</span><span class="sxs-lookup"><span data-stu-id="012aa-104">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="012aa-105">Методы</span><span class="sxs-lookup"><span data-stu-id="012aa-105">Methods</span></span>

| <span data-ttu-id="012aa-106">Метод</span><span class="sxs-lookup"><span data-stu-id="012aa-106">Method</span></span>           | <span data-ttu-id="012aa-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="012aa-107">Return Type</span></span>    |<span data-ttu-id="012aa-108">Описание</span><span class="sxs-lookup"><span data-stu-id="012aa-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="012aa-109">Получение объекта ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="012aa-109">Get ChartGridlines</span></span>](../api/chartgridlines-get.md) | [<span data-ttu-id="012aa-110">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="012aa-110">WorkbookChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="012aa-111">Чтение свойств и связей объекта chartGridlines.</span><span class="sxs-lookup"><span data-stu-id="012aa-111">Read properties and relationships of chartGridlines object.</span></span>|
|<span data-ttu-id="012aa-112">[обновление](../api/chartgridlines-update.md).</span><span class="sxs-lookup"><span data-stu-id="012aa-112">[Update](../api/chartgridlines-update.md)</span></span> | [<span data-ttu-id="012aa-113">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="012aa-113">WorkbookChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="012aa-114">Обновление объекта ChartGridlines.</span><span class="sxs-lookup"><span data-stu-id="012aa-114">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="012aa-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="012aa-115">Properties</span></span>
| <span data-ttu-id="012aa-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="012aa-116">Property</span></span>     | <span data-ttu-id="012aa-117">Тип</span><span class="sxs-lookup"><span data-stu-id="012aa-117">Type</span></span>   |<span data-ttu-id="012aa-118">Описание</span><span class="sxs-lookup"><span data-stu-id="012aa-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="012aa-119">visible</span><span class="sxs-lookup"><span data-stu-id="012aa-119">visible</span></span>|<span data-ttu-id="012aa-120">boolean</span><span class="sxs-lookup"><span data-stu-id="012aa-120">boolean</span></span>|<span data-ttu-id="012aa-121">Логическое значение, определяющее, отображаются ли линии сетки оси.</span><span class="sxs-lookup"><span data-stu-id="012aa-121">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="012aa-122">Связи</span><span class="sxs-lookup"><span data-stu-id="012aa-122">Relationships</span></span>
| <span data-ttu-id="012aa-123">Связь</span><span class="sxs-lookup"><span data-stu-id="012aa-123">Relationship</span></span> | <span data-ttu-id="012aa-124">Тип</span><span class="sxs-lookup"><span data-stu-id="012aa-124">Type</span></span>   |<span data-ttu-id="012aa-125">Описание</span><span class="sxs-lookup"><span data-stu-id="012aa-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="012aa-126">format</span><span class="sxs-lookup"><span data-stu-id="012aa-126">format</span></span>|[<span data-ttu-id="012aa-127">WorkbookChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="012aa-127">WorkbookChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="012aa-p101">Представляет форматирование линий сетки диаграммы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="012aa-p101">Represents the formatting of chart gridlines. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="012aa-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="012aa-130">JSON representation</span></span>

<span data-ttu-id="012aa-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="012aa-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartGridlines"
}-->

```json
{
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartGridlines resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->