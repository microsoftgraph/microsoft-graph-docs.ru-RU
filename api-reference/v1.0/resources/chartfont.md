---
title: Тип ресурса ChartFont
description: Этот объект представляет атрибуты шрифта (название, размер, цвет и т. д.) для объекта диаграммы.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 9241691296b93eb21e19e10b81f36e692fea0692
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033000"
---
# <a name="chartfont-resource-type"></a><span data-ttu-id="60f48-103">Тип ресурса ChartFont</span><span class="sxs-lookup"><span data-stu-id="60f48-103">ChartFont resource type</span></span>

<span data-ttu-id="60f48-104">Этот объект представляет атрибуты шрифта (название, размер, цвет и т. д.) для объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="60f48-104">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="60f48-105">Методы</span><span class="sxs-lookup"><span data-stu-id="60f48-105">Methods</span></span>

| <span data-ttu-id="60f48-106">Метод</span><span class="sxs-lookup"><span data-stu-id="60f48-106">Method</span></span>           | <span data-ttu-id="60f48-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="60f48-107">Return Type</span></span>    |<span data-ttu-id="60f48-108">Описание</span><span class="sxs-lookup"><span data-stu-id="60f48-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="60f48-109">Получение объекта ChartFont</span><span class="sxs-lookup"><span data-stu-id="60f48-109">Get ChartFont</span></span>](../api/chartfont-get.md) | [<span data-ttu-id="60f48-110">Воркбукчартфонт</span><span class="sxs-lookup"><span data-stu-id="60f48-110">WorkbookChartFont</span></span>](chartfont.md) |<span data-ttu-id="60f48-111">Чтение свойств и связей объекта chartFont.</span><span class="sxs-lookup"><span data-stu-id="60f48-111">Read properties and relationships of chartFont object.</span></span>|
|[<span data-ttu-id="60f48-112">Обновление</span><span class="sxs-lookup"><span data-stu-id="60f48-112">Update</span></span>](../api/chartfont-update.md) | [<span data-ttu-id="60f48-113">Воркбукчартфонт</span><span class="sxs-lookup"><span data-stu-id="60f48-113">WorkbookChartFont</span></span>](chartfont.md)   |<span data-ttu-id="60f48-114">Обновление объекта ChartFont.</span><span class="sxs-lookup"><span data-stu-id="60f48-114">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="60f48-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="60f48-115">Properties</span></span>
| <span data-ttu-id="60f48-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="60f48-116">Property</span></span>     | <span data-ttu-id="60f48-117">Тип</span><span class="sxs-lookup"><span data-stu-id="60f48-117">Type</span></span>   |<span data-ttu-id="60f48-118">Описание</span><span class="sxs-lookup"><span data-stu-id="60f48-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60f48-119">bold</span><span class="sxs-lookup"><span data-stu-id="60f48-119">bold</span></span>|<span data-ttu-id="60f48-120">boolean</span><span class="sxs-lookup"><span data-stu-id="60f48-120">boolean</span></span>|<span data-ttu-id="60f48-121">Указывает, является ли шрифт полужирным.</span><span class="sxs-lookup"><span data-stu-id="60f48-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="60f48-122">color</span><span class="sxs-lookup"><span data-stu-id="60f48-122">color</span></span>|<span data-ttu-id="60f48-123">строка</span><span class="sxs-lookup"><span data-stu-id="60f48-123">string</span></span>|<span data-ttu-id="60f48-p101">HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.</span><span class="sxs-lookup"><span data-stu-id="60f48-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="60f48-127">italic</span><span class="sxs-lookup"><span data-stu-id="60f48-127">italic</span></span>|<span data-ttu-id="60f48-128">boolean</span><span class="sxs-lookup"><span data-stu-id="60f48-128">boolean</span></span>|<span data-ttu-id="60f48-129">Указывает, применяется ли курсив.</span><span class="sxs-lookup"><span data-stu-id="60f48-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="60f48-130">name</span><span class="sxs-lookup"><span data-stu-id="60f48-130">name</span></span>|<span data-ttu-id="60f48-131">string</span><span class="sxs-lookup"><span data-stu-id="60f48-131">string</span></span>|<span data-ttu-id="60f48-132">Имя шрифта (например, Calibri)</span><span class="sxs-lookup"><span data-stu-id="60f48-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="60f48-133">size</span><span class="sxs-lookup"><span data-stu-id="60f48-133">size</span></span>|<span data-ttu-id="60f48-134">Double</span><span class="sxs-lookup"><span data-stu-id="60f48-134">double</span></span>|<span data-ttu-id="60f48-135">Размер шрифта (например, 11)</span><span class="sxs-lookup"><span data-stu-id="60f48-135">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="60f48-136">underline</span><span class="sxs-lookup"><span data-stu-id="60f48-136">underline</span></span>|<span data-ttu-id="60f48-137">string</span><span class="sxs-lookup"><span data-stu-id="60f48-137">string</span></span>|<span data-ttu-id="60f48-138">Тип подчеркивания, применяемый для шрифта.</span><span class="sxs-lookup"><span data-stu-id="60f48-138">Type of underline applied to the font.</span></span> <span data-ttu-id="60f48-139">Возможные значения: `None`, `Single`.</span><span class="sxs-lookup"><span data-stu-id="60f48-139">The possible values are: `None`, `Single`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60f48-140">Отношения</span><span class="sxs-lookup"><span data-stu-id="60f48-140">Relationships</span></span>
<span data-ttu-id="60f48-141">Нет</span><span class="sxs-lookup"><span data-stu-id="60f48-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="60f48-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="60f48-142">JSON representation</span></span>

<span data-ttu-id="60f48-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60f48-143">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartFont"
}-->

```json
{
  "bold": true,
  "color": "string",
  "italic": true,
  "name": "string",
  "size": 1024,
  "underline": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
