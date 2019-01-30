---
title: Тип ресурса RangeFont
description: Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 2dee07b7d2573081650bdd15799e4884c774e171
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640163"
---
# <a name="rangefont-resource-type"></a><span data-ttu-id="9397b-103">Тип ресурса RangeFont</span><span class="sxs-lookup"><span data-stu-id="9397b-103">RangeFont resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9397b-104">Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта.</span><span class="sxs-lookup"><span data-stu-id="9397b-104">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="9397b-105">Методы</span><span class="sxs-lookup"><span data-stu-id="9397b-105">Methods</span></span>

| <span data-ttu-id="9397b-106">Метод</span><span class="sxs-lookup"><span data-stu-id="9397b-106">Method</span></span>           | <span data-ttu-id="9397b-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9397b-107">Return Type</span></span>    |<span data-ttu-id="9397b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9397b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9397b-109">Получение объекта RangeFont</span><span class="sxs-lookup"><span data-stu-id="9397b-109">Get RangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="9397b-110">RangeFont</span><span class="sxs-lookup"><span data-stu-id="9397b-110">RangeFont</span></span>](rangefont.md) |<span data-ttu-id="9397b-111">Чтение свойств и связей объекта rangeFont.</span><span class="sxs-lookup"><span data-stu-id="9397b-111">Read properties and relationships of rangeFont object.</span></span>|
|<span data-ttu-id="9397b-112">[обновление](../api/rangefont-update.md).</span><span class="sxs-lookup"><span data-stu-id="9397b-112">[Update](../api/rangefont-update.md)</span></span> | [<span data-ttu-id="9397b-113">RangeFont</span><span class="sxs-lookup"><span data-stu-id="9397b-113">RangeFont</span></span>](rangefont.md)   |<span data-ttu-id="9397b-114">Обновление объекта RangeFont.</span><span class="sxs-lookup"><span data-stu-id="9397b-114">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9397b-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="9397b-115">Properties</span></span>
| <span data-ttu-id="9397b-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="9397b-116">Property</span></span>     | <span data-ttu-id="9397b-117">Тип</span><span class="sxs-lookup"><span data-stu-id="9397b-117">Type</span></span>   |<span data-ttu-id="9397b-118">Описание</span><span class="sxs-lookup"><span data-stu-id="9397b-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9397b-119">bold</span><span class="sxs-lookup"><span data-stu-id="9397b-119">bold</span></span>|<span data-ttu-id="9397b-120">boolean</span><span class="sxs-lookup"><span data-stu-id="9397b-120">boolean</span></span>|<span data-ttu-id="9397b-121">Указывает, является ли шрифт полужирным.</span><span class="sxs-lookup"><span data-stu-id="9397b-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="9397b-122">color</span><span class="sxs-lookup"><span data-stu-id="9397b-122">color</span></span>|<span data-ttu-id="9397b-123">строка</span><span class="sxs-lookup"><span data-stu-id="9397b-123">string</span></span>|<span data-ttu-id="9397b-p101">HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.</span><span class="sxs-lookup"><span data-stu-id="9397b-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="9397b-127">italic</span><span class="sxs-lookup"><span data-stu-id="9397b-127">italic</span></span>|<span data-ttu-id="9397b-128">boolean</span><span class="sxs-lookup"><span data-stu-id="9397b-128">boolean</span></span>|<span data-ttu-id="9397b-129">Указывает, применяется ли курсив.</span><span class="sxs-lookup"><span data-stu-id="9397b-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="9397b-130">name</span><span class="sxs-lookup"><span data-stu-id="9397b-130">name</span></span>|<span data-ttu-id="9397b-131">строка</span><span class="sxs-lookup"><span data-stu-id="9397b-131">string</span></span>|<span data-ttu-id="9397b-132">Имя шрифта (например, Calibri)</span><span class="sxs-lookup"><span data-stu-id="9397b-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="9397b-133">size</span><span class="sxs-lookup"><span data-stu-id="9397b-133">size</span></span>|<span data-ttu-id="9397b-134">double</span><span class="sxs-lookup"><span data-stu-id="9397b-134">double</span></span>|<span data-ttu-id="9397b-135">font-size</span><span class="sxs-lookup"><span data-stu-id="9397b-135">Font size.</span></span>|
|<span data-ttu-id="9397b-136">underline</span><span class="sxs-lookup"><span data-stu-id="9397b-136">underline</span></span>|<span data-ttu-id="9397b-137">строка</span><span class="sxs-lookup"><span data-stu-id="9397b-137">string</span></span>|<span data-ttu-id="9397b-p102">Тип подчеркивания, применяемый для шрифта. Возможные значения: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="9397b-p102">Type of underline applied to the font. Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9397b-140">Связи</span><span class="sxs-lookup"><span data-stu-id="9397b-140">Relationships</span></span>
<span data-ttu-id="9397b-141">Нет</span><span class="sxs-lookup"><span data-stu-id="9397b-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9397b-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9397b-142">JSON representation</span></span>

<span data-ttu-id="9397b-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9397b-143">Here is a JSON representation of the resource.</span></span>

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
