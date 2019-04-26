---
title: Тип ресурса ChartPointFormat
description: Представляет объект форматирования для точек диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1c1b0a4a7d9076771da11061723f275079d429cb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569069"
---
# <a name="chartpointformat-resource-type"></a><span data-ttu-id="80bcf-103">Тип ресурса ChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="80bcf-103">ChartPointFormat resource type</span></span>

<span data-ttu-id="80bcf-104">Представляет объект форматирования для точек диаграммы.</span><span class="sxs-lookup"><span data-stu-id="80bcf-104">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="80bcf-105">Методы</span><span class="sxs-lookup"><span data-stu-id="80bcf-105">Methods</span></span>
<span data-ttu-id="80bcf-106">Нет</span><span class="sxs-lookup"><span data-stu-id="80bcf-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="80bcf-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="80bcf-107">Properties</span></span>
<span data-ttu-id="80bcf-108">Нет</span><span class="sxs-lookup"><span data-stu-id="80bcf-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="80bcf-109">Связи</span><span class="sxs-lookup"><span data-stu-id="80bcf-109">Relationships</span></span>
| <span data-ttu-id="80bcf-110">Отношение</span><span class="sxs-lookup"><span data-stu-id="80bcf-110">Relationship</span></span> | <span data-ttu-id="80bcf-111">Тип</span><span class="sxs-lookup"><span data-stu-id="80bcf-111">Type</span></span>   |<span data-ttu-id="80bcf-112">Описание</span><span class="sxs-lookup"><span data-stu-id="80bcf-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80bcf-113">fill</span><span class="sxs-lookup"><span data-stu-id="80bcf-113">fill</span></span>|[<span data-ttu-id="80bcf-114">Воркбукчартфилл</span><span class="sxs-lookup"><span data-stu-id="80bcf-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="80bcf-115">Представляет формат заливки диаграммы, включая сведения о форматировании фона.</span><span class="sxs-lookup"><span data-stu-id="80bcf-115">Represents the fill format of a chart, which includes background formating information.</span></span> <span data-ttu-id="80bcf-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="80bcf-116">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="80bcf-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="80bcf-117">JSON representation</span></span>

<span data-ttu-id="80bcf-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="80bcf-118">Here is a JSON representation of the resource.</span></span>

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
