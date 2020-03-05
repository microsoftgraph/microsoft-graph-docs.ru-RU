---
title: Тип ресурса Воркбукчартлежендформат
description: Инкапсулирует свойства формата легенды диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 32f9fcec2002039c9ccee399c90f1a26048c71cc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519304"
---
# <a name="workbookchartlegendformat-resource-type"></a><span data-ttu-id="911f6-103">Тип ресурса Воркбукчартлежендформат</span><span class="sxs-lookup"><span data-stu-id="911f6-103">workbookChartLegendFormat resource type</span></span>

<span data-ttu-id="911f6-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="911f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="911f6-105">Инкапсулирует свойства формата легенды диаграммы.</span><span class="sxs-lookup"><span data-stu-id="911f6-105">Encapsulates the format properties of a chart legend.</span></span>

## <a name="methods"></a><span data-ttu-id="911f6-106">Методы</span><span class="sxs-lookup"><span data-stu-id="911f6-106">Methods</span></span>
<span data-ttu-id="911f6-107">Нет</span><span class="sxs-lookup"><span data-stu-id="911f6-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="911f6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="911f6-108">Properties</span></span>
<span data-ttu-id="911f6-109">Нет</span><span class="sxs-lookup"><span data-stu-id="911f6-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="911f6-110">Связи</span><span class="sxs-lookup"><span data-stu-id="911f6-110">Relationships</span></span>
| <span data-ttu-id="911f6-111">Связь</span><span class="sxs-lookup"><span data-stu-id="911f6-111">Relationship</span></span> | <span data-ttu-id="911f6-112">Тип</span><span class="sxs-lookup"><span data-stu-id="911f6-112">Type</span></span>   |<span data-ttu-id="911f6-113">Описание</span><span class="sxs-lookup"><span data-stu-id="911f6-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="911f6-114">fill</span><span class="sxs-lookup"><span data-stu-id="911f6-114">fill</span></span>|[<span data-ttu-id="911f6-115">воркбукчартфилл</span><span class="sxs-lookup"><span data-stu-id="911f6-115">workbookChartFill</span></span>](workbookchartfill.md)|<span data-ttu-id="911f6-p101">Представляет формат заливки объекта, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="911f6-p101">Represents the fill format of an object, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="911f6-118">шрифт</span><span class="sxs-lookup"><span data-stu-id="911f6-118">font</span></span>|[<span data-ttu-id="911f6-119">воркбукчартфонт</span><span class="sxs-lookup"><span data-stu-id="911f6-119">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="911f6-120">Представляет атрибуты шрифта, такие как имя шрифта, размер шрифта, цвет и т. д., в условных обозначениях диаграммы.</span><span class="sxs-lookup"><span data-stu-id="911f6-120">Represents the font attributes such as font name, font size, color, etc. of a chart legend.</span></span> <span data-ttu-id="911f6-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="911f6-121">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="911f6-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="911f6-122">JSON representation</span></span>

<span data-ttu-id="911f6-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="911f6-123">Here is a JSON representation of the resource.</span></span>

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
