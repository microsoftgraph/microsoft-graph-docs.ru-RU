---
title: Тип ресурса RangeFont
description: Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта.
localization_priority: Normal
ms.openlocfilehash: 32bbd29706966c4c4b15f038ebdbb872b1dd8193
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856583"
---
# <a name="rangefont-resource-type"></a><span data-ttu-id="41b02-103">Тип ресурса RangeFont</span><span class="sxs-lookup"><span data-stu-id="41b02-103">RangeFont resource type</span></span>

<span data-ttu-id="41b02-104">Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта.</span><span class="sxs-lookup"><span data-stu-id="41b02-104">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="41b02-105">Методы</span><span class="sxs-lookup"><span data-stu-id="41b02-105">Methods</span></span>

| <span data-ttu-id="41b02-106">Метод</span><span class="sxs-lookup"><span data-stu-id="41b02-106">Method</span></span>           | <span data-ttu-id="41b02-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="41b02-107">Return Type</span></span>    |<span data-ttu-id="41b02-108">Описание</span><span class="sxs-lookup"><span data-stu-id="41b02-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="41b02-109">Получение объекта RangeFont</span><span class="sxs-lookup"><span data-stu-id="41b02-109">Get RangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="41b02-110">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="41b02-110">WorkbookRangeFont</span></span>](rangefont.md) |<span data-ttu-id="41b02-111">Чтение свойств и связей объекта rangeFont.</span><span class="sxs-lookup"><span data-stu-id="41b02-111">Read properties and relationships of rangeFont object.</span></span>|
|<span data-ttu-id="41b02-112">[обновление](../api/rangefont-update.md).</span><span class="sxs-lookup"><span data-stu-id="41b02-112">[Update](../api/rangefont-update.md)</span></span> | [<span data-ttu-id="41b02-113">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="41b02-113">WorkbookRangeFont</span></span>](rangefont.md)   |<span data-ttu-id="41b02-114">Обновление объекта RangeFont.</span><span class="sxs-lookup"><span data-stu-id="41b02-114">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="41b02-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="41b02-115">Properties</span></span>
| <span data-ttu-id="41b02-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="41b02-116">Property</span></span>     | <span data-ttu-id="41b02-117">Тип</span><span class="sxs-lookup"><span data-stu-id="41b02-117">Type</span></span>   |<span data-ttu-id="41b02-118">Описание</span><span class="sxs-lookup"><span data-stu-id="41b02-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41b02-119">bold</span><span class="sxs-lookup"><span data-stu-id="41b02-119">bold</span></span>|<span data-ttu-id="41b02-120">boolean</span><span class="sxs-lookup"><span data-stu-id="41b02-120">boolean</span></span>|<span data-ttu-id="41b02-121">Указывает, является ли шрифт полужирным.</span><span class="sxs-lookup"><span data-stu-id="41b02-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="41b02-122">color</span><span class="sxs-lookup"><span data-stu-id="41b02-122">color</span></span>|<span data-ttu-id="41b02-123">строка</span><span class="sxs-lookup"><span data-stu-id="41b02-123">string</span></span>|<span data-ttu-id="41b02-p101">HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.</span><span class="sxs-lookup"><span data-stu-id="41b02-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="41b02-127">italic</span><span class="sxs-lookup"><span data-stu-id="41b02-127">italic</span></span>|<span data-ttu-id="41b02-128">boolean</span><span class="sxs-lookup"><span data-stu-id="41b02-128">boolean</span></span>|<span data-ttu-id="41b02-129">Указывает, применяется ли курсив.</span><span class="sxs-lookup"><span data-stu-id="41b02-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="41b02-130">name</span><span class="sxs-lookup"><span data-stu-id="41b02-130">name</span></span>|<span data-ttu-id="41b02-131">строка</span><span class="sxs-lookup"><span data-stu-id="41b02-131">string</span></span>|<span data-ttu-id="41b02-132">Имя шрифта (например, Calibri)</span><span class="sxs-lookup"><span data-stu-id="41b02-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="41b02-133">size</span><span class="sxs-lookup"><span data-stu-id="41b02-133">size</span></span>|<span data-ttu-id="41b02-134">double</span><span class="sxs-lookup"><span data-stu-id="41b02-134">double</span></span>|<span data-ttu-id="41b02-135">font-size</span><span class="sxs-lookup"><span data-stu-id="41b02-135">Font size.</span></span>|
|<span data-ttu-id="41b02-136">underline</span><span class="sxs-lookup"><span data-stu-id="41b02-136">underline</span></span>|<span data-ttu-id="41b02-137">строка</span><span class="sxs-lookup"><span data-stu-id="41b02-137">string</span></span>|<span data-ttu-id="41b02-138">Тип подчеркивание шрифта.</span><span class="sxs-lookup"><span data-stu-id="41b02-138">Type of underline applied to the font.</span></span> <span data-ttu-id="41b02-139">Возможные значения: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="41b02-139">The possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="41b02-140">Связи</span><span class="sxs-lookup"><span data-stu-id="41b02-140">Relationships</span></span>
<span data-ttu-id="41b02-141">Нет</span><span class="sxs-lookup"><span data-stu-id="41b02-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="41b02-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="41b02-142">JSON representation</span></span>

<span data-ttu-id="41b02-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="41b02-143">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeFont"
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
  "description": "RangeFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
