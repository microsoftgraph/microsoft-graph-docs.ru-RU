---
title: Тип ресурса ChartLineFormat
description: Инкапсулирует параметры форматирования для элементов линий.
ms.openlocfilehash: 6646f985fd106ed738432852fec5a3bad187ab61
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078817"
---
# <a name="chartlineformat-resource-type"></a><span data-ttu-id="0cdce-103">Тип ресурса ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="0cdce-103">ChartLineFormat resource type</span></span>

> <span data-ttu-id="0cdce-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0cdce-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0cdce-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0cdce-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0cdce-106">Инкапсулирует параметры форматирования для элементов линий.</span><span class="sxs-lookup"><span data-stu-id="0cdce-106">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="0cdce-107">Методы</span><span class="sxs-lookup"><span data-stu-id="0cdce-107">Methods</span></span>

| <span data-ttu-id="0cdce-108">Метод</span><span class="sxs-lookup"><span data-stu-id="0cdce-108">Method</span></span>           | <span data-ttu-id="0cdce-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0cdce-109">Return Type</span></span>    |<span data-ttu-id="0cdce-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0cdce-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0cdce-111">Получение объекта ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="0cdce-111">Get ChartLineFormat</span></span>](../api/chartlineformat-get.md) | [<span data-ttu-id="0cdce-112">ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="0cdce-112">ChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="0cdce-113">Чтение свойств и связей объекта chartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="0cdce-113">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="0cdce-114">Update</span><span class="sxs-lookup"><span data-stu-id="0cdce-114">Update</span></span>](../api/chartlineformat-update.md) | [<span data-ttu-id="0cdce-115">ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="0cdce-115">ChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="0cdce-116">Обновление объекта ChartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="0cdce-116">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="0cdce-117">Clear</span><span class="sxs-lookup"><span data-stu-id="0cdce-117">Clear</span></span>](../api/chartlineformat-clear.md)|<span data-ttu-id="0cdce-118">Нет</span><span class="sxs-lookup"><span data-stu-id="0cdce-118">None</span></span>|<span data-ttu-id="0cdce-119">Очищает формат линий элемента диаграммы.</span><span class="sxs-lookup"><span data-stu-id="0cdce-119">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="0cdce-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="0cdce-120">Properties</span></span>
| <span data-ttu-id="0cdce-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="0cdce-121">Property</span></span>     | <span data-ttu-id="0cdce-122">Тип</span><span class="sxs-lookup"><span data-stu-id="0cdce-122">Type</span></span>   |<span data-ttu-id="0cdce-123">Описание</span><span class="sxs-lookup"><span data-stu-id="0cdce-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0cdce-124">color</span><span class="sxs-lookup"><span data-stu-id="0cdce-124">color</span></span>|<span data-ttu-id="0cdce-125">строка</span><span class="sxs-lookup"><span data-stu-id="0cdce-125">string</span></span>|<span data-ttu-id="0cdce-126">HTML-код цвета, представляющий цвет линий в диаграмме.</span><span class="sxs-lookup"><span data-stu-id="0cdce-126">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0cdce-127">Связи</span><span class="sxs-lookup"><span data-stu-id="0cdce-127">Relationships</span></span>
<span data-ttu-id="0cdce-128">Нет</span><span class="sxs-lookup"><span data-stu-id="0cdce-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0cdce-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0cdce-129">JSON representation</span></span>

<span data-ttu-id="0cdce-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0cdce-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartLineFormat"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->