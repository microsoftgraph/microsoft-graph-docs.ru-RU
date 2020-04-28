---
title: Тип ресурса Воркбукчартпоинтформат
description: Представляет объект форматирования для точек диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 9e947fa02624f2c24ea6433dc2e62eb0da218308
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519283"
---
# <a name="workbookchartpointformat-resource-type"></a><span data-ttu-id="1a53b-103">Тип ресурса Воркбукчартпоинтформат</span><span class="sxs-lookup"><span data-stu-id="1a53b-103">workbookChartPointFormat resource type</span></span>

<span data-ttu-id="1a53b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a53b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a53b-105">Представляет объект форматирования для точек диаграммы.</span><span class="sxs-lookup"><span data-stu-id="1a53b-105">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="1a53b-106">Methods</span><span class="sxs-lookup"><span data-stu-id="1a53b-106">Methods</span></span>
<span data-ttu-id="1a53b-107">Нет</span><span class="sxs-lookup"><span data-stu-id="1a53b-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="1a53b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1a53b-108">Properties</span></span>
<span data-ttu-id="1a53b-109">Нет</span><span class="sxs-lookup"><span data-stu-id="1a53b-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="1a53b-110">Связи</span><span class="sxs-lookup"><span data-stu-id="1a53b-110">Relationships</span></span>
| <span data-ttu-id="1a53b-111">Связь</span><span class="sxs-lookup"><span data-stu-id="1a53b-111">Relationship</span></span> | <span data-ttu-id="1a53b-112">Тип</span><span class="sxs-lookup"><span data-stu-id="1a53b-112">Type</span></span>   |<span data-ttu-id="1a53b-113">Описание</span><span class="sxs-lookup"><span data-stu-id="1a53b-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a53b-114">fill</span><span class="sxs-lookup"><span data-stu-id="1a53b-114">fill</span></span>|[<span data-ttu-id="1a53b-115">воркбукчартфилл</span><span class="sxs-lookup"><span data-stu-id="1a53b-115">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="1a53b-116">Представляет формат заливки диаграммы, включая сведения о форматировании фона.</span><span class="sxs-lookup"><span data-stu-id="1a53b-116">Represents the fill format of a chart, which includes background formating information.</span></span> <span data-ttu-id="1a53b-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1a53b-117">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="1a53b-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1a53b-118">JSON representation</span></span>

<span data-ttu-id="1a53b-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a53b-119">Here is a JSON representation of the resource.</span></span>

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
