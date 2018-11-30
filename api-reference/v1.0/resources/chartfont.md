---
title: Тип ресурса ChartFont
description: Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта диаграммы.
ms.openlocfilehash: dc4b1f8cd0653d89c3486a61604dd09c0e23cb2c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025556"
---
# <a name="chartfont-resource-type"></a><span data-ttu-id="bcf6f-103">Тип ресурса ChartFont</span><span class="sxs-lookup"><span data-stu-id="bcf6f-103">ChartFont resource type</span></span>

<span data-ttu-id="bcf6f-104">Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="bcf6f-104">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="bcf6f-105">Методы</span><span class="sxs-lookup"><span data-stu-id="bcf6f-105">Methods</span></span>

| <span data-ttu-id="bcf6f-106">Метод</span><span class="sxs-lookup"><span data-stu-id="bcf6f-106">Method</span></span>           | <span data-ttu-id="bcf6f-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bcf6f-107">Return Type</span></span>    |<span data-ttu-id="bcf6f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="bcf6f-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bcf6f-109">Получение объекта ChartFont</span><span class="sxs-lookup"><span data-stu-id="bcf6f-109">Get ChartFont</span></span>](../api/chartfont-get.md) | [<span data-ttu-id="bcf6f-110">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="bcf6f-110">WorkbookChartFont</span></span>](chartfont.md) |<span data-ttu-id="bcf6f-111">Чтение свойств и связей объекта chartFont.</span><span class="sxs-lookup"><span data-stu-id="bcf6f-111">Read properties and relationships of chartFont object.</span></span>|
|[<span data-ttu-id="bcf6f-112">Update</span><span class="sxs-lookup"><span data-stu-id="bcf6f-112">Update</span></span>](../api/chartfont-update.md) | [<span data-ttu-id="bcf6f-113">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="bcf6f-113">WorkbookChartFont</span></span>](chartfont.md)   |<span data-ttu-id="bcf6f-114">Обновление объекта ChartFont.</span><span class="sxs-lookup"><span data-stu-id="bcf6f-114">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="bcf6f-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="bcf6f-115">Properties</span></span>
| <span data-ttu-id="bcf6f-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="bcf6f-116">Property</span></span>     | <span data-ttu-id="bcf6f-117">Тип</span><span class="sxs-lookup"><span data-stu-id="bcf6f-117">Type</span></span>   |<span data-ttu-id="bcf6f-118">Описание</span><span class="sxs-lookup"><span data-stu-id="bcf6f-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bcf6f-119">bold</span><span class="sxs-lookup"><span data-stu-id="bcf6f-119">bold</span></span>|<span data-ttu-id="bcf6f-120">boolean</span><span class="sxs-lookup"><span data-stu-id="bcf6f-120">boolean</span></span>|<span data-ttu-id="bcf6f-121">Указывает, является ли шрифт полужирным.</span><span class="sxs-lookup"><span data-stu-id="bcf6f-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="bcf6f-122">color</span><span class="sxs-lookup"><span data-stu-id="bcf6f-122">color</span></span>|<span data-ttu-id="bcf6f-123">строка</span><span class="sxs-lookup"><span data-stu-id="bcf6f-123">string</span></span>|<span data-ttu-id="bcf6f-p101">HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.</span><span class="sxs-lookup"><span data-stu-id="bcf6f-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="bcf6f-127">italic</span><span class="sxs-lookup"><span data-stu-id="bcf6f-127">italic</span></span>|<span data-ttu-id="bcf6f-128">boolean</span><span class="sxs-lookup"><span data-stu-id="bcf6f-128">boolean</span></span>|<span data-ttu-id="bcf6f-129">Указывает, применяется ли курсив.</span><span class="sxs-lookup"><span data-stu-id="bcf6f-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="bcf6f-130">name</span><span class="sxs-lookup"><span data-stu-id="bcf6f-130">name</span></span>|<span data-ttu-id="bcf6f-131">строка</span><span class="sxs-lookup"><span data-stu-id="bcf6f-131">string</span></span>|<span data-ttu-id="bcf6f-132">Имя шрифта (например, Calibri)</span><span class="sxs-lookup"><span data-stu-id="bcf6f-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="bcf6f-133">size</span><span class="sxs-lookup"><span data-stu-id="bcf6f-133">size</span></span>|<span data-ttu-id="bcf6f-134">Double</span><span class="sxs-lookup"><span data-stu-id="bcf6f-134">double</span></span>|<span data-ttu-id="bcf6f-135">Размер шрифта (например, 11)</span><span class="sxs-lookup"><span data-stu-id="bcf6f-135">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="bcf6f-136">underline</span><span class="sxs-lookup"><span data-stu-id="bcf6f-136">underline</span></span>|<span data-ttu-id="bcf6f-137">строка</span><span class="sxs-lookup"><span data-stu-id="bcf6f-137">string</span></span>|<span data-ttu-id="bcf6f-138">Тип подчеркивание шрифта.</span><span class="sxs-lookup"><span data-stu-id="bcf6f-138">Type of underline applied to the font.</span></span> <span data-ttu-id="bcf6f-139">Возможные значения: `None`, `Single`.</span><span class="sxs-lookup"><span data-stu-id="bcf6f-139">The possible values are: `None`, `Single`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bcf6f-140">Связи</span><span class="sxs-lookup"><span data-stu-id="bcf6f-140">Relationships</span></span>
<span data-ttu-id="bcf6f-141">Нет</span><span class="sxs-lookup"><span data-stu-id="bcf6f-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="bcf6f-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bcf6f-142">JSON representation</span></span>

<span data-ttu-id="bcf6f-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bcf6f-143">Here is a JSON representation of the resource.</span></span>

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