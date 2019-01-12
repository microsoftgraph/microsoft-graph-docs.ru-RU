---
title: Тип ресурса RangeFont
description: Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 829b391d561aae63ae94972c55039acfdf4c48d7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962298"
---
# <a name="rangefont-resource-type"></a><span data-ttu-id="42b95-103">Тип ресурса RangeFont</span><span class="sxs-lookup"><span data-stu-id="42b95-103">RangeFont resource type</span></span>

<span data-ttu-id="42b95-104">Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта.</span><span class="sxs-lookup"><span data-stu-id="42b95-104">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="42b95-105">Методы</span><span class="sxs-lookup"><span data-stu-id="42b95-105">Methods</span></span>

| <span data-ttu-id="42b95-106">Метод</span><span class="sxs-lookup"><span data-stu-id="42b95-106">Method</span></span>           | <span data-ttu-id="42b95-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="42b95-107">Return Type</span></span>    |<span data-ttu-id="42b95-108">Описание</span><span class="sxs-lookup"><span data-stu-id="42b95-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="42b95-109">Получение объекта RangeFont</span><span class="sxs-lookup"><span data-stu-id="42b95-109">Get RangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="42b95-110">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="42b95-110">WorkbookRangeFont</span></span>](rangefont.md) |<span data-ttu-id="42b95-111">Чтение свойств и связей объекта rangeFont.</span><span class="sxs-lookup"><span data-stu-id="42b95-111">Read properties and relationships of rangeFont object.</span></span>|
|<span data-ttu-id="42b95-112">[обновление](../api/rangefont-update.md).</span><span class="sxs-lookup"><span data-stu-id="42b95-112">[Update](../api/rangefont-update.md)</span></span> | [<span data-ttu-id="42b95-113">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="42b95-113">WorkbookRangeFont</span></span>](rangefont.md)   |<span data-ttu-id="42b95-114">Обновление объекта RangeFont.</span><span class="sxs-lookup"><span data-stu-id="42b95-114">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="42b95-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="42b95-115">Properties</span></span>
| <span data-ttu-id="42b95-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="42b95-116">Property</span></span>     | <span data-ttu-id="42b95-117">Тип</span><span class="sxs-lookup"><span data-stu-id="42b95-117">Type</span></span>   |<span data-ttu-id="42b95-118">Описание</span><span class="sxs-lookup"><span data-stu-id="42b95-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42b95-119">bold</span><span class="sxs-lookup"><span data-stu-id="42b95-119">bold</span></span>|<span data-ttu-id="42b95-120">boolean</span><span class="sxs-lookup"><span data-stu-id="42b95-120">boolean</span></span>|<span data-ttu-id="42b95-121">Указывает, является ли шрифт полужирным.</span><span class="sxs-lookup"><span data-stu-id="42b95-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="42b95-122">color</span><span class="sxs-lookup"><span data-stu-id="42b95-122">color</span></span>|<span data-ttu-id="42b95-123">строка</span><span class="sxs-lookup"><span data-stu-id="42b95-123">string</span></span>|<span data-ttu-id="42b95-p101">HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.</span><span class="sxs-lookup"><span data-stu-id="42b95-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="42b95-127">italic</span><span class="sxs-lookup"><span data-stu-id="42b95-127">italic</span></span>|<span data-ttu-id="42b95-128">boolean</span><span class="sxs-lookup"><span data-stu-id="42b95-128">boolean</span></span>|<span data-ttu-id="42b95-129">Указывает, применяется ли курсив.</span><span class="sxs-lookup"><span data-stu-id="42b95-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="42b95-130">name</span><span class="sxs-lookup"><span data-stu-id="42b95-130">name</span></span>|<span data-ttu-id="42b95-131">строка</span><span class="sxs-lookup"><span data-stu-id="42b95-131">string</span></span>|<span data-ttu-id="42b95-132">Имя шрифта (например, Calibri)</span><span class="sxs-lookup"><span data-stu-id="42b95-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="42b95-133">size</span><span class="sxs-lookup"><span data-stu-id="42b95-133">size</span></span>|<span data-ttu-id="42b95-134">double</span><span class="sxs-lookup"><span data-stu-id="42b95-134">double</span></span>|<span data-ttu-id="42b95-135">font-size</span><span class="sxs-lookup"><span data-stu-id="42b95-135">Font size.</span></span>|
|<span data-ttu-id="42b95-136">underline</span><span class="sxs-lookup"><span data-stu-id="42b95-136">underline</span></span>|<span data-ttu-id="42b95-137">строка</span><span class="sxs-lookup"><span data-stu-id="42b95-137">string</span></span>|<span data-ttu-id="42b95-138">Тип подчеркивание шрифта.</span><span class="sxs-lookup"><span data-stu-id="42b95-138">Type of underline applied to the font.</span></span> <span data-ttu-id="42b95-139">Возможные значения: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="42b95-139">The possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="42b95-140">Связи</span><span class="sxs-lookup"><span data-stu-id="42b95-140">Relationships</span></span>
<span data-ttu-id="42b95-141">Нет</span><span class="sxs-lookup"><span data-stu-id="42b95-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="42b95-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="42b95-142">JSON representation</span></span>

<span data-ttu-id="42b95-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42b95-143">Here is a JSON representation of the resource.</span></span>

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
