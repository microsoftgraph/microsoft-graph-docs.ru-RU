---
title: Тип ресурса ChartAxisTitleFormat
description: Представляет форматирование для названий осей диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 26d305d8bd4a0059123f77bd86cbbf5fd01dcea7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569083"
---
# <a name="chartaxistitleformat-resource-type"></a><span data-ttu-id="5ffcf-103">Тип ресурса ChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="5ffcf-103">ChartAxisTitleFormat resource type</span></span>

<span data-ttu-id="5ffcf-104">Представляет форматирование для названий осей диаграммы.</span><span class="sxs-lookup"><span data-stu-id="5ffcf-104">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="5ffcf-105">Методы</span><span class="sxs-lookup"><span data-stu-id="5ffcf-105">Methods</span></span>
<span data-ttu-id="5ffcf-106">Нет</span><span class="sxs-lookup"><span data-stu-id="5ffcf-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="5ffcf-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5ffcf-107">Properties</span></span>
<span data-ttu-id="5ffcf-108">Нет</span><span class="sxs-lookup"><span data-stu-id="5ffcf-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="5ffcf-109">Связи</span><span class="sxs-lookup"><span data-stu-id="5ffcf-109">Relationships</span></span>
| <span data-ttu-id="5ffcf-110">Отношение</span><span class="sxs-lookup"><span data-stu-id="5ffcf-110">Relationship</span></span> | <span data-ttu-id="5ffcf-111">Тип</span><span class="sxs-lookup"><span data-stu-id="5ffcf-111">Type</span></span>   |<span data-ttu-id="5ffcf-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5ffcf-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ffcf-113">font</span><span class="sxs-lookup"><span data-stu-id="5ffcf-113">font</span></span>|[<span data-ttu-id="5ffcf-114">Воркбукчартфонт</span><span class="sxs-lookup"><span data-stu-id="5ffcf-114">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="5ffcf-115">Представляет атрибуты шрифта, такие как имя шрифта, размер шрифта, цвет и т. д. объект заголовка оси диаграммы.</span><span class="sxs-lookup"><span data-stu-id="5ffcf-115">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object.</span></span> <span data-ttu-id="5ffcf-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5ffcf-116">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5ffcf-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5ffcf-117">JSON representation</span></span>

<span data-ttu-id="5ffcf-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5ffcf-118">Here is a JSON representation of the resource.</span></span>

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
