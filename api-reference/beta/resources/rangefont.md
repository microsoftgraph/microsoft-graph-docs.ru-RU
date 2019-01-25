---
title: Тип ресурса RangeFont
description: Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 2dee07b7d2573081650bdd15799e4884c774e171
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507966"
---
# <a name="rangefont-resource-type"></a><span data-ttu-id="d17ed-103">Тип ресурса RangeFont</span><span class="sxs-lookup"><span data-stu-id="d17ed-103">RangeFont resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d17ed-104">Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта.</span><span class="sxs-lookup"><span data-stu-id="d17ed-104">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="d17ed-105">Методы</span><span class="sxs-lookup"><span data-stu-id="d17ed-105">Methods</span></span>

| <span data-ttu-id="d17ed-106">Метод</span><span class="sxs-lookup"><span data-stu-id="d17ed-106">Method</span></span>           | <span data-ttu-id="d17ed-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d17ed-107">Return Type</span></span>    |<span data-ttu-id="d17ed-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d17ed-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d17ed-109">Получение объекта RangeFont</span><span class="sxs-lookup"><span data-stu-id="d17ed-109">[Get RangeFont](../api/rangefont-get.md)</span></span> | <span data-ttu-id="d17ed-110">RangeFont</span><span class="sxs-lookup"><span data-stu-id="d17ed-110">[RangeFont](rangefont.md)</span></span> |<span data-ttu-id="d17ed-111">Чтение свойств и связей объекта rangeFont.</span><span class="sxs-lookup"><span data-stu-id="d17ed-111">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="d17ed-112">Update</span><span class="sxs-lookup"><span data-stu-id="d17ed-112">Update</span></span>](../api/rangefont-update.md) | <span data-ttu-id="d17ed-113">RangeFont</span><span class="sxs-lookup"><span data-stu-id="d17ed-113">[RangeFont](rangefont.md)</span></span>   |<span data-ttu-id="d17ed-114">Обновление объекта RangeFont.</span><span class="sxs-lookup"><span data-stu-id="d17ed-114">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d17ed-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="d17ed-115">Properties</span></span>
| <span data-ttu-id="d17ed-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="d17ed-116">Property</span></span>     | <span data-ttu-id="d17ed-117">Тип</span><span class="sxs-lookup"><span data-stu-id="d17ed-117">Type</span></span>   |<span data-ttu-id="d17ed-118">Описание</span><span class="sxs-lookup"><span data-stu-id="d17ed-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d17ed-119">bold</span><span class="sxs-lookup"><span data-stu-id="d17ed-119">bold</span></span>|<span data-ttu-id="d17ed-120">boolean</span><span class="sxs-lookup"><span data-stu-id="d17ed-120">boolean</span></span>|<span data-ttu-id="d17ed-121">Указывает, является ли шрифт полужирным.</span><span class="sxs-lookup"><span data-stu-id="d17ed-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="d17ed-122">color</span><span class="sxs-lookup"><span data-stu-id="d17ed-122">color</span></span>|<span data-ttu-id="d17ed-123">строка</span><span class="sxs-lookup"><span data-stu-id="d17ed-123">string</span></span>|<span data-ttu-id="d17ed-p101">HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.</span><span class="sxs-lookup"><span data-stu-id="d17ed-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="d17ed-127">italic</span><span class="sxs-lookup"><span data-stu-id="d17ed-127">italic</span></span>|<span data-ttu-id="d17ed-128">boolean</span><span class="sxs-lookup"><span data-stu-id="d17ed-128">boolean</span></span>|<span data-ttu-id="d17ed-129">Указывает, применяется ли курсив.</span><span class="sxs-lookup"><span data-stu-id="d17ed-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="d17ed-130">name</span><span class="sxs-lookup"><span data-stu-id="d17ed-130">name</span></span>|<span data-ttu-id="d17ed-131">string</span><span class="sxs-lookup"><span data-stu-id="d17ed-131">string</span></span>|<span data-ttu-id="d17ed-132">Имя шрифта (например, Calibri)</span><span class="sxs-lookup"><span data-stu-id="d17ed-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="d17ed-133">size</span><span class="sxs-lookup"><span data-stu-id="d17ed-133">size</span></span>|<span data-ttu-id="d17ed-134">double</span><span class="sxs-lookup"><span data-stu-id="d17ed-134">double</span></span>|<span data-ttu-id="d17ed-135">font-size</span><span class="sxs-lookup"><span data-stu-id="d17ed-135">Font size.</span></span>|
|<span data-ttu-id="d17ed-136">underline</span><span class="sxs-lookup"><span data-stu-id="d17ed-136">underline</span></span>|<span data-ttu-id="d17ed-137">string</span><span class="sxs-lookup"><span data-stu-id="d17ed-137">string</span></span>|<span data-ttu-id="d17ed-p102">Тип подчеркивания, применяемый для шрифта. Возможные значения: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="d17ed-p102">Type of underline applied to the font. Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d17ed-140">Отношения</span><span class="sxs-lookup"><span data-stu-id="d17ed-140">Relationships</span></span>
<span data-ttu-id="d17ed-141">Нет</span><span class="sxs-lookup"><span data-stu-id="d17ed-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d17ed-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d17ed-142">JSON representation</span></span>

<span data-ttu-id="d17ed-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d17ed-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeFont"
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
  "description": "RangeFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/rangefont.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
