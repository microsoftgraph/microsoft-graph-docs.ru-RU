---
title: Тип ресурса Воркбукчартлежендформат
description: Инкапсулирует свойства формата легенды диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6bd5fd708574950aea8752396b7fd6495ca6b782
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348968"
---
# <a name="workbookchartlegendformat-resource-type"></a><span data-ttu-id="64491-103">Тип ресурса Воркбукчартлежендформат</span><span class="sxs-lookup"><span data-stu-id="64491-103">workbookChartLegendFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64491-104">Инкапсулирует свойства формата легенды диаграммы.</span><span class="sxs-lookup"><span data-stu-id="64491-104">Encapsulates the format properties of a chart legend.</span></span>

## <a name="methods"></a><span data-ttu-id="64491-105">Методы</span><span class="sxs-lookup"><span data-stu-id="64491-105">Methods</span></span>
<span data-ttu-id="64491-106">Отсутствует</span><span class="sxs-lookup"><span data-stu-id="64491-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="64491-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="64491-107">Properties</span></span>
<span data-ttu-id="64491-108">Нет</span><span class="sxs-lookup"><span data-stu-id="64491-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="64491-109">Отношения</span><span class="sxs-lookup"><span data-stu-id="64491-109">Relationships</span></span>
| <span data-ttu-id="64491-110">Отношение</span><span class="sxs-lookup"><span data-stu-id="64491-110">Relationship</span></span> | <span data-ttu-id="64491-111">Тип</span><span class="sxs-lookup"><span data-stu-id="64491-111">Type</span></span>   |<span data-ttu-id="64491-112">Описание</span><span class="sxs-lookup"><span data-stu-id="64491-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="64491-113">fill</span><span class="sxs-lookup"><span data-stu-id="64491-113">fill</span></span>|[<span data-ttu-id="64491-114">Воркбукчартфилл</span><span class="sxs-lookup"><span data-stu-id="64491-114">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="64491-p101">Представляет формат заливки объекта, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64491-p101">Represents the fill format of an object, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="64491-117">шрифт</span><span class="sxs-lookup"><span data-stu-id="64491-117">font</span></span>|[<span data-ttu-id="64491-118">Воркбукчартфонт</span><span class="sxs-lookup"><span data-stu-id="64491-118">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="64491-119">Представляет атрибуты шрифта, такие как имя шрифта, размер шрифта, цвет и т. д., в условных обозначениях диаграммы.</span><span class="sxs-lookup"><span data-stu-id="64491-119">Represents the font attributes such as font name, font size, color, etc. of a chart legend.</span></span> <span data-ttu-id="64491-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64491-120">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="64491-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="64491-121">JSON representation</span></span>

<span data-ttu-id="64491-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64491-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "fill",
    "font"
    ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartLegendFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookChartLegendFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
