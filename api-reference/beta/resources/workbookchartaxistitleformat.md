---
title: Тип ресурса Воркбукчартаксиститлеформат
description: Представляет форматирование для названий осей диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: c585fc426474fe0a7790874331a2ae53227fc1a7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039060"
---
# <a name="workbookchartaxistitleformat-resource-type"></a><span data-ttu-id="808b7-103">Тип ресурса Воркбукчартаксиститлеформат</span><span class="sxs-lookup"><span data-stu-id="808b7-103">workbookChartAxisTitleFormat resource type</span></span>

<span data-ttu-id="808b7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="808b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="808b7-105">Представляет форматирование для названий осей диаграммы.</span><span class="sxs-lookup"><span data-stu-id="808b7-105">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="808b7-106">Методы</span><span class="sxs-lookup"><span data-stu-id="808b7-106">Methods</span></span>
<span data-ttu-id="808b7-107">Нет</span><span class="sxs-lookup"><span data-stu-id="808b7-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="808b7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="808b7-108">Properties</span></span>
<span data-ttu-id="808b7-109">Нет</span><span class="sxs-lookup"><span data-stu-id="808b7-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="808b7-110">Отношения</span><span class="sxs-lookup"><span data-stu-id="808b7-110">Relationships</span></span>
| <span data-ttu-id="808b7-111">Связь</span><span class="sxs-lookup"><span data-stu-id="808b7-111">Relationship</span></span> | <span data-ttu-id="808b7-112">Тип</span><span class="sxs-lookup"><span data-stu-id="808b7-112">Type</span></span>   |<span data-ttu-id="808b7-113">Описание</span><span class="sxs-lookup"><span data-stu-id="808b7-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="808b7-114">font</span><span class="sxs-lookup"><span data-stu-id="808b7-114">font</span></span>|[<span data-ttu-id="808b7-115">воркбукчартфонт</span><span class="sxs-lookup"><span data-stu-id="808b7-115">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="808b7-116">Представляет атрибуты шрифта, такие как имя шрифта, размер шрифта, цвет и т. д. объект заголовка оси диаграммы.</span><span class="sxs-lookup"><span data-stu-id="808b7-116">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object.</span></span> <span data-ttu-id="808b7-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="808b7-117">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="808b7-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="808b7-118">JSON representation</span></span>

<span data-ttu-id="808b7-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="808b7-119">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "font"
    ],
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxisTitleFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


