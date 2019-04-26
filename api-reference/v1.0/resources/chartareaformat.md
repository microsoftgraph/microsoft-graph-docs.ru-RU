---
title: Тип ресурса ChartAreaFormat
description: Инкапсулирует свойства формата для всей области диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a447b604807f3ae223445db953d45928eda9f36b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569391"
---
# <a name="chartareaformat-resource-type"></a><span data-ttu-id="67205-103">Тип ресурса ChartAreaFormat</span><span class="sxs-lookup"><span data-stu-id="67205-103">ChartAreaFormat resource type</span></span>

<span data-ttu-id="67205-104">Инкапсулирует свойства формата для всей области диаграммы.</span><span class="sxs-lookup"><span data-stu-id="67205-104">Encapsulates the format properties for the overall chart area.</span></span>


## <a name="methods"></a><span data-ttu-id="67205-105">Методы</span><span class="sxs-lookup"><span data-stu-id="67205-105">Methods</span></span>
<span data-ttu-id="67205-106">Нет</span><span class="sxs-lookup"><span data-stu-id="67205-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="67205-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="67205-107">Properties</span></span>
<span data-ttu-id="67205-108">Нет</span><span class="sxs-lookup"><span data-stu-id="67205-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="67205-109">Связи</span><span class="sxs-lookup"><span data-stu-id="67205-109">Relationships</span></span>
| <span data-ttu-id="67205-110">Отношение</span><span class="sxs-lookup"><span data-stu-id="67205-110">Relationship</span></span> | <span data-ttu-id="67205-111">Тип</span><span class="sxs-lookup"><span data-stu-id="67205-111">Type</span></span>   |<span data-ttu-id="67205-112">Описание</span><span class="sxs-lookup"><span data-stu-id="67205-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67205-113">fill</span><span class="sxs-lookup"><span data-stu-id="67205-113">fill</span></span>|[<span data-ttu-id="67205-114">Воркбукчартфилл</span><span class="sxs-lookup"><span data-stu-id="67205-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="67205-p101">Представляет формат заливки объекта, включая сведения о форматировании фона. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="67205-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="67205-117">font</span><span class="sxs-lookup"><span data-stu-id="67205-117">font</span></span>|[<span data-ttu-id="67205-118">Воркбукчартфонт</span><span class="sxs-lookup"><span data-stu-id="67205-118">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="67205-119">Представляет атрибуты шрифта (имя, размер шрифта, цвет и т. д.) для текущего объекта.</span><span class="sxs-lookup"><span data-stu-id="67205-119">Represents the font attributes (font name, font size, color, etc.) for the current object.</span></span> <span data-ttu-id="67205-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="67205-120">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="67205-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="67205-121">JSON representation</span></span>

<span data-ttu-id="67205-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="67205-122">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAreaFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAreaFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
