---
title: Тип ресурса Воркбукчартпоинтформат
description: Представляет объект форматирования для точек диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f0896001fda140ff1d2693b3463c472568f1d28e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348980"
---
# <a name="workbookchartpointformat-resource-type"></a><span data-ttu-id="ee202-103">Тип ресурса Воркбукчартпоинтформат</span><span class="sxs-lookup"><span data-stu-id="ee202-103">workbookChartPointFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee202-104">Представляет объект форматирования для точек диаграммы.</span><span class="sxs-lookup"><span data-stu-id="ee202-104">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="ee202-105">Методы</span><span class="sxs-lookup"><span data-stu-id="ee202-105">Methods</span></span>
<span data-ttu-id="ee202-106">Отсутствует</span><span class="sxs-lookup"><span data-stu-id="ee202-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="ee202-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ee202-107">Properties</span></span>
<span data-ttu-id="ee202-108">Нет</span><span class="sxs-lookup"><span data-stu-id="ee202-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="ee202-109">Отношения</span><span class="sxs-lookup"><span data-stu-id="ee202-109">Relationships</span></span>
| <span data-ttu-id="ee202-110">Отношение</span><span class="sxs-lookup"><span data-stu-id="ee202-110">Relationship</span></span> | <span data-ttu-id="ee202-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ee202-111">Type</span></span>   |<span data-ttu-id="ee202-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ee202-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee202-113">fill</span><span class="sxs-lookup"><span data-stu-id="ee202-113">fill</span></span>|[<span data-ttu-id="ee202-114">Воркбукчартфилл</span><span class="sxs-lookup"><span data-stu-id="ee202-114">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="ee202-115">Представляет формат заливки диаграммы, включая сведения о форматировании фона.</span><span class="sxs-lookup"><span data-stu-id="ee202-115">Represents the fill format of a chart, which includes background formating information.</span></span> <span data-ttu-id="ee202-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ee202-116">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="ee202-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ee202-117">JSON representation</span></span>

<span data-ttu-id="ee202-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee202-118">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "fill"
    ],
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartPointFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
