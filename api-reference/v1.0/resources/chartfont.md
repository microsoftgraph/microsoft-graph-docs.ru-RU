---
title: Тип ресурса ChartFont
description: Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта диаграммы.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 85a11d59e58d6968154a4ede12fa978b1f061de1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972791"
---
# <a name="chartfont-resource-type"></a><span data-ttu-id="c690c-103">Тип ресурса ChartFont</span><span class="sxs-lookup"><span data-stu-id="c690c-103">ChartFont resource type</span></span>

<span data-ttu-id="c690c-104">Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="c690c-104">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="c690c-105">Методы</span><span class="sxs-lookup"><span data-stu-id="c690c-105">Methods</span></span>

| <span data-ttu-id="c690c-106">Метод</span><span class="sxs-lookup"><span data-stu-id="c690c-106">Method</span></span>           | <span data-ttu-id="c690c-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c690c-107">Return Type</span></span>    |<span data-ttu-id="c690c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c690c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c690c-109">Получение объекта ChartFont</span><span class="sxs-lookup"><span data-stu-id="c690c-109">Get ChartFont</span></span>](../api/chartfont-get.md) | [<span data-ttu-id="c690c-110">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="c690c-110">WorkbookChartFont</span></span>](chartfont.md) |<span data-ttu-id="c690c-111">Чтение свойств и связей объекта chartFont.</span><span class="sxs-lookup"><span data-stu-id="c690c-111">Read properties and relationships of chartFont object.</span></span>|
|<span data-ttu-id="c690c-112">[обновление](../api/chartfont-update.md).</span><span class="sxs-lookup"><span data-stu-id="c690c-112">[Update](../api/chartfont-update.md)</span></span> | [<span data-ttu-id="c690c-113">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="c690c-113">WorkbookChartFont</span></span>](chartfont.md)   |<span data-ttu-id="c690c-114">Обновление объекта ChartFont.</span><span class="sxs-lookup"><span data-stu-id="c690c-114">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c690c-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="c690c-115">Properties</span></span>
| <span data-ttu-id="c690c-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="c690c-116">Property</span></span>     | <span data-ttu-id="c690c-117">Тип</span><span class="sxs-lookup"><span data-stu-id="c690c-117">Type</span></span>   |<span data-ttu-id="c690c-118">Описание</span><span class="sxs-lookup"><span data-stu-id="c690c-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c690c-119">bold</span><span class="sxs-lookup"><span data-stu-id="c690c-119">bold</span></span>|<span data-ttu-id="c690c-120">boolean</span><span class="sxs-lookup"><span data-stu-id="c690c-120">boolean</span></span>|<span data-ttu-id="c690c-121">Указывает, является ли шрифт полужирным.</span><span class="sxs-lookup"><span data-stu-id="c690c-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="c690c-122">color</span><span class="sxs-lookup"><span data-stu-id="c690c-122">color</span></span>|<span data-ttu-id="c690c-123">строка</span><span class="sxs-lookup"><span data-stu-id="c690c-123">string</span></span>|<span data-ttu-id="c690c-p101">HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.</span><span class="sxs-lookup"><span data-stu-id="c690c-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="c690c-127">italic</span><span class="sxs-lookup"><span data-stu-id="c690c-127">italic</span></span>|<span data-ttu-id="c690c-128">boolean</span><span class="sxs-lookup"><span data-stu-id="c690c-128">boolean</span></span>|<span data-ttu-id="c690c-129">Указывает, применяется ли курсив.</span><span class="sxs-lookup"><span data-stu-id="c690c-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="c690c-130">name</span><span class="sxs-lookup"><span data-stu-id="c690c-130">name</span></span>|<span data-ttu-id="c690c-131">строка</span><span class="sxs-lookup"><span data-stu-id="c690c-131">string</span></span>|<span data-ttu-id="c690c-132">Имя шрифта (например, Calibri)</span><span class="sxs-lookup"><span data-stu-id="c690c-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="c690c-133">size</span><span class="sxs-lookup"><span data-stu-id="c690c-133">size</span></span>|<span data-ttu-id="c690c-134">Double</span><span class="sxs-lookup"><span data-stu-id="c690c-134">double</span></span>|<span data-ttu-id="c690c-135">Размер шрифта (например, 11)</span><span class="sxs-lookup"><span data-stu-id="c690c-135">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="c690c-136">underline</span><span class="sxs-lookup"><span data-stu-id="c690c-136">underline</span></span>|<span data-ttu-id="c690c-137">строка</span><span class="sxs-lookup"><span data-stu-id="c690c-137">string</span></span>|<span data-ttu-id="c690c-138">Тип подчеркивание шрифта.</span><span class="sxs-lookup"><span data-stu-id="c690c-138">Type of underline applied to the font.</span></span> <span data-ttu-id="c690c-139">Возможные значения: `None`, `Single`.</span><span class="sxs-lookup"><span data-stu-id="c690c-139">The possible values are: `None`, `Single`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c690c-140">Связи</span><span class="sxs-lookup"><span data-stu-id="c690c-140">Relationships</span></span>
<span data-ttu-id="c690c-141">Нет</span><span class="sxs-lookup"><span data-stu-id="c690c-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c690c-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c690c-142">JSON representation</span></span>

<span data-ttu-id="c690c-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c690c-143">Here is a JSON representation of the resource.</span></span>

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
