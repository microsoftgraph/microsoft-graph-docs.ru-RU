---
title: Тип ресурса ChartAxisTitleFormat
description: Представляет форматирование для названий осей диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 62522cee67684141911511de26731879936b4f2b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531884"
---
# <a name="chartaxistitleformat-resource-type"></a><span data-ttu-id="f363a-103">Тип ресурса ChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="f363a-103">ChartAxisTitleFormat resource type</span></span>

<span data-ttu-id="f363a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f363a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f363a-105">Представляет форматирование для названий осей диаграммы.</span><span class="sxs-lookup"><span data-stu-id="f363a-105">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="f363a-106">Методы</span><span class="sxs-lookup"><span data-stu-id="f363a-106">Methods</span></span>
<span data-ttu-id="f363a-107">Нет</span><span class="sxs-lookup"><span data-stu-id="f363a-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="f363a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f363a-108">Properties</span></span>
<span data-ttu-id="f363a-109">Нет</span><span class="sxs-lookup"><span data-stu-id="f363a-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="f363a-110">Связи</span><span class="sxs-lookup"><span data-stu-id="f363a-110">Relationships</span></span>
| <span data-ttu-id="f363a-111">Связь</span><span class="sxs-lookup"><span data-stu-id="f363a-111">Relationship</span></span> | <span data-ttu-id="f363a-112">Тип</span><span class="sxs-lookup"><span data-stu-id="f363a-112">Type</span></span>   |<span data-ttu-id="f363a-113">Описание</span><span class="sxs-lookup"><span data-stu-id="f363a-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f363a-114">font</span><span class="sxs-lookup"><span data-stu-id="f363a-114">font</span></span>|[<span data-ttu-id="f363a-115">воркбукчартфонт</span><span class="sxs-lookup"><span data-stu-id="f363a-115">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="f363a-116">Представляет атрибуты шрифта, такие как имя шрифта, размер шрифта, цвет и т. д. объект заголовка оси диаграммы.</span><span class="sxs-lookup"><span data-stu-id="f363a-116">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object.</span></span> <span data-ttu-id="f363a-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f363a-117">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f363a-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f363a-118">JSON representation</span></span>

<span data-ttu-id="f363a-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f363a-119">Here is a JSON representation of the resource.</span></span>

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
