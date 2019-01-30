---
title: Тип ресурса ChartFont
description: Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта диаграммы.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: c507a966dc6b29e46935c5c77a85b557a84cc69c
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641171"
---
# <a name="chartfont-resource-type"></a><span data-ttu-id="a3060-103">Тип ресурса ChartFont</span><span class="sxs-lookup"><span data-stu-id="a3060-103">ChartFont resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3060-104">Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="a3060-104">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="a3060-105">Методы</span><span class="sxs-lookup"><span data-stu-id="a3060-105">Methods</span></span>

| <span data-ttu-id="a3060-106">Метод</span><span class="sxs-lookup"><span data-stu-id="a3060-106">Method</span></span>           | <span data-ttu-id="a3060-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a3060-107">Return Type</span></span>    |<span data-ttu-id="a3060-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a3060-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a3060-109">Получение объекта ChartFont</span><span class="sxs-lookup"><span data-stu-id="a3060-109">Get ChartFont</span></span>](../api/chartfont-get.md) | [<span data-ttu-id="a3060-110">ChartFont</span><span class="sxs-lookup"><span data-stu-id="a3060-110">ChartFont</span></span>](chartfont.md) |<span data-ttu-id="a3060-111">Чтение свойств и связей объекта chartFont.</span><span class="sxs-lookup"><span data-stu-id="a3060-111">Read properties and relationships of chartFont object.</span></span>|
|<span data-ttu-id="a3060-112">[обновление](../api/chartfont-update.md).</span><span class="sxs-lookup"><span data-stu-id="a3060-112">[Update](../api/chartfont-update.md)</span></span> | [<span data-ttu-id="a3060-113">ChartFont</span><span class="sxs-lookup"><span data-stu-id="a3060-113">ChartFont</span></span>](chartfont.md)   |<span data-ttu-id="a3060-114">Обновление объекта ChartFont.</span><span class="sxs-lookup"><span data-stu-id="a3060-114">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a3060-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="a3060-115">Properties</span></span>
| <span data-ttu-id="a3060-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3060-116">Property</span></span>     | <span data-ttu-id="a3060-117">Тип</span><span class="sxs-lookup"><span data-stu-id="a3060-117">Type</span></span>   |<span data-ttu-id="a3060-118">Описание</span><span class="sxs-lookup"><span data-stu-id="a3060-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a3060-119">bold</span><span class="sxs-lookup"><span data-stu-id="a3060-119">bold</span></span>|<span data-ttu-id="a3060-120">boolean</span><span class="sxs-lookup"><span data-stu-id="a3060-120">boolean</span></span>|<span data-ttu-id="a3060-121">Указывает, является ли шрифт полужирным.</span><span class="sxs-lookup"><span data-stu-id="a3060-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="a3060-122">color</span><span class="sxs-lookup"><span data-stu-id="a3060-122">color</span></span>|<span data-ttu-id="a3060-123">строка</span><span class="sxs-lookup"><span data-stu-id="a3060-123">string</span></span>|<span data-ttu-id="a3060-p101">HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.</span><span class="sxs-lookup"><span data-stu-id="a3060-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="a3060-127">italic</span><span class="sxs-lookup"><span data-stu-id="a3060-127">italic</span></span>|<span data-ttu-id="a3060-128">boolean</span><span class="sxs-lookup"><span data-stu-id="a3060-128">boolean</span></span>|<span data-ttu-id="a3060-129">Указывает, применяется ли курсив.</span><span class="sxs-lookup"><span data-stu-id="a3060-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="a3060-130">name</span><span class="sxs-lookup"><span data-stu-id="a3060-130">name</span></span>|<span data-ttu-id="a3060-131">строка</span><span class="sxs-lookup"><span data-stu-id="a3060-131">string</span></span>|<span data-ttu-id="a3060-132">Имя шрифта (например, Calibri)</span><span class="sxs-lookup"><span data-stu-id="a3060-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="a3060-133">size</span><span class="sxs-lookup"><span data-stu-id="a3060-133">size</span></span>|<span data-ttu-id="a3060-134">Double</span><span class="sxs-lookup"><span data-stu-id="a3060-134">double</span></span>|<span data-ttu-id="a3060-135">Размер шрифта (например, 11)</span><span class="sxs-lookup"><span data-stu-id="a3060-135">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="a3060-136">underline</span><span class="sxs-lookup"><span data-stu-id="a3060-136">underline</span></span>|<span data-ttu-id="a3060-137">строка</span><span class="sxs-lookup"><span data-stu-id="a3060-137">string</span></span>|<span data-ttu-id="a3060-p102">Тип подчеркивания, применяемый для шрифта. Возможные значения: `None`, `Single`.</span><span class="sxs-lookup"><span data-stu-id="a3060-p102">Type of underline applied to the font. Possible values are: `None`, `Single`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3060-140">Связи</span><span class="sxs-lookup"><span data-stu-id="a3060-140">Relationships</span></span>
<span data-ttu-id="a3060-141">Нет</span><span class="sxs-lookup"><span data-stu-id="a3060-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a3060-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a3060-142">JSON representation</span></span>

<span data-ttu-id="a3060-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3060-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartFont"
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
<!--
{
  "type": "#page.annotation",
  "description": "ChartFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartfont.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
