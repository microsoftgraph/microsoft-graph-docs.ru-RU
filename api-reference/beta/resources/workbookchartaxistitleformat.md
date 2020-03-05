---
title: Тип ресурса Воркбукчартаксиститлеформат
description: Представляет форматирование для названий осей диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: a676bb28ccce19c7f4293e9fc082a59ec0cfdbb7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519360"
---
# <a name="workbookchartaxistitleformat-resource-type"></a><span data-ttu-id="da3ed-103">Тип ресурса Воркбукчартаксиститлеформат</span><span class="sxs-lookup"><span data-stu-id="da3ed-103">workbookChartAxisTitleFormat resource type</span></span>

<span data-ttu-id="da3ed-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="da3ed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da3ed-105">Представляет форматирование для названий осей диаграммы.</span><span class="sxs-lookup"><span data-stu-id="da3ed-105">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="da3ed-106">Методы</span><span class="sxs-lookup"><span data-stu-id="da3ed-106">Methods</span></span>
<span data-ttu-id="da3ed-107">Нет</span><span class="sxs-lookup"><span data-stu-id="da3ed-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="da3ed-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="da3ed-108">Properties</span></span>
<span data-ttu-id="da3ed-109">Нет</span><span class="sxs-lookup"><span data-stu-id="da3ed-109">None</span></span>

## <a name="relationships"></a><span data-ttu-id="da3ed-110">Связи</span><span class="sxs-lookup"><span data-stu-id="da3ed-110">Relationships</span></span>
| <span data-ttu-id="da3ed-111">Связь</span><span class="sxs-lookup"><span data-stu-id="da3ed-111">Relationship</span></span> | <span data-ttu-id="da3ed-112">Тип</span><span class="sxs-lookup"><span data-stu-id="da3ed-112">Type</span></span>   |<span data-ttu-id="da3ed-113">Описание</span><span class="sxs-lookup"><span data-stu-id="da3ed-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da3ed-114">font</span><span class="sxs-lookup"><span data-stu-id="da3ed-114">font</span></span>|[<span data-ttu-id="da3ed-115">воркбукчартфонт</span><span class="sxs-lookup"><span data-stu-id="da3ed-115">workbookChartFont</span></span>](workbookchartfont.md)|<span data-ttu-id="da3ed-116">Представляет атрибуты шрифта, такие как имя шрифта, размер шрифта, цвет и т. д. объект заголовка оси диаграммы.</span><span class="sxs-lookup"><span data-stu-id="da3ed-116">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object.</span></span> <span data-ttu-id="da3ed-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="da3ed-117">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="da3ed-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="da3ed-118">JSON representation</span></span>

<span data-ttu-id="da3ed-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="da3ed-119">Here is a JSON representation of the resource.</span></span>

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
