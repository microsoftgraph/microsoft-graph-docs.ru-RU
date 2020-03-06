---
title: Тип ресурса ChartPointFormat
description: Представляет объект форматирования для точек диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: c71b7158b7ba3cef208fb6bf983d077c9474e77c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533104"
---
# <a name="chartpointformat-resource-type"></a><span data-ttu-id="e20fb-103">Тип ресурса ChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="e20fb-103">ChartPointFormat resource type</span></span>

<span data-ttu-id="e20fb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e20fb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e20fb-105">Представляет объект форматирования для точек диаграммы.</span><span class="sxs-lookup"><span data-stu-id="e20fb-105">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="e20fb-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e20fb-106">Methods</span></span>
<span data-ttu-id="e20fb-107">Нет</span><span class="sxs-lookup"><span data-stu-id="e20fb-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="e20fb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e20fb-108">Properties</span></span>
<span data-ttu-id="e20fb-109">Нет</span><span class="sxs-lookup"><span data-stu-id="e20fb-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="e20fb-110">Связи</span><span class="sxs-lookup"><span data-stu-id="e20fb-110">Relationships</span></span>
| <span data-ttu-id="e20fb-111">Связь</span><span class="sxs-lookup"><span data-stu-id="e20fb-111">Relationship</span></span> | <span data-ttu-id="e20fb-112">Тип</span><span class="sxs-lookup"><span data-stu-id="e20fb-112">Type</span></span>   |<span data-ttu-id="e20fb-113">Описание</span><span class="sxs-lookup"><span data-stu-id="e20fb-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e20fb-114">fill</span><span class="sxs-lookup"><span data-stu-id="e20fb-114">fill</span></span>|[<span data-ttu-id="e20fb-115">воркбукчартфилл</span><span class="sxs-lookup"><span data-stu-id="e20fb-115">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="e20fb-116">Представляет формат заливки диаграммы, включая сведения о форматировании фона.</span><span class="sxs-lookup"><span data-stu-id="e20fb-116">Represents the fill format of a chart, which includes background formating information.</span></span> <span data-ttu-id="e20fb-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e20fb-117">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e20fb-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e20fb-118">JSON representation</span></span>

<span data-ttu-id="e20fb-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e20fb-119">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPointFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPointFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
