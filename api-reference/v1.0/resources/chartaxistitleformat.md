---
title: Тип ресурса ChartAxisTitleFormat
description: Представляет форматирование для названий осей диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 3ae74b7353a0b4198b42a04fdd420eb3447d4c11
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029850"
---
# <a name="chartaxistitleformat-resource-type"></a><span data-ttu-id="ff5c6-103">Тип ресурса ChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="ff5c6-103">ChartAxisTitleFormat resource type</span></span>

<span data-ttu-id="ff5c6-104">Представляет форматирование для названий осей диаграммы.</span><span class="sxs-lookup"><span data-stu-id="ff5c6-104">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="ff5c6-105">Методы</span><span class="sxs-lookup"><span data-stu-id="ff5c6-105">Methods</span></span>
<span data-ttu-id="ff5c6-106">Нет</span><span class="sxs-lookup"><span data-stu-id="ff5c6-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="ff5c6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff5c6-107">Properties</span></span>
<span data-ttu-id="ff5c6-108">Нет</span><span class="sxs-lookup"><span data-stu-id="ff5c6-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="ff5c6-109">Отношения</span><span class="sxs-lookup"><span data-stu-id="ff5c6-109">Relationships</span></span>
| <span data-ttu-id="ff5c6-110">Отношение</span><span class="sxs-lookup"><span data-stu-id="ff5c6-110">Relationship</span></span> | <span data-ttu-id="ff5c6-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ff5c6-111">Type</span></span>   |<span data-ttu-id="ff5c6-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ff5c6-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff5c6-113">font</span><span class="sxs-lookup"><span data-stu-id="ff5c6-113">font</span></span>|[<span data-ttu-id="ff5c6-114">Воркбукчартфонт</span><span class="sxs-lookup"><span data-stu-id="ff5c6-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="ff5c6-115">Представляет атрибуты шрифта, такие как имя шрифта, размер шрифта, цвет и т. д. объект заголовка оси диаграммы.</span><span class="sxs-lookup"><span data-stu-id="ff5c6-115">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object.</span></span> <span data-ttu-id="ff5c6-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ff5c6-116">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ff5c6-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff5c6-117">JSON representation</span></span>

<span data-ttu-id="ff5c6-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff5c6-118">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisTitleFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitleFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
