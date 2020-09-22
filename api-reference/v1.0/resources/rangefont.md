---
title: Тип ресурса RangeFont
description: Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 95a58a62355c70b1f2588b83594ab5497ac3db49
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037075"
---
# <a name="rangefont-resource-type"></a><span data-ttu-id="6a23d-103">Тип ресурса RangeFont</span><span class="sxs-lookup"><span data-stu-id="6a23d-103">RangeFont resource type</span></span>

<span data-ttu-id="6a23d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a23d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6a23d-105">Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта.</span><span class="sxs-lookup"><span data-stu-id="6a23d-105">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="6a23d-106">Методы</span><span class="sxs-lookup"><span data-stu-id="6a23d-106">Methods</span></span>

| <span data-ttu-id="6a23d-107">Метод</span><span class="sxs-lookup"><span data-stu-id="6a23d-107">Method</span></span>           | <span data-ttu-id="6a23d-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6a23d-108">Return Type</span></span>    |<span data-ttu-id="6a23d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6a23d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6a23d-110">Получение объекта RangeFont</span><span class="sxs-lookup"><span data-stu-id="6a23d-110">Get RangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="6a23d-111">воркбукранжефонт</span><span class="sxs-lookup"><span data-stu-id="6a23d-111">WorkbookRangeFont</span></span>](rangefont.md) |<span data-ttu-id="6a23d-112">Чтение свойств и связей объекта rangeFont.</span><span class="sxs-lookup"><span data-stu-id="6a23d-112">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="6a23d-113">Обновление</span><span class="sxs-lookup"><span data-stu-id="6a23d-113">Update</span></span>](../api/rangefont-update.md) | [<span data-ttu-id="6a23d-114">воркбукранжефонт</span><span class="sxs-lookup"><span data-stu-id="6a23d-114">WorkbookRangeFont</span></span>](rangefont.md)   |<span data-ttu-id="6a23d-115">Обновление объекта RangeFont.</span><span class="sxs-lookup"><span data-stu-id="6a23d-115">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6a23d-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="6a23d-116">Properties</span></span>
| <span data-ttu-id="6a23d-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a23d-117">Property</span></span>     | <span data-ttu-id="6a23d-118">Тип</span><span class="sxs-lookup"><span data-stu-id="6a23d-118">Type</span></span>   |<span data-ttu-id="6a23d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="6a23d-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a23d-120">bold</span><span class="sxs-lookup"><span data-stu-id="6a23d-120">bold</span></span>|<span data-ttu-id="6a23d-121">boolean</span><span class="sxs-lookup"><span data-stu-id="6a23d-121">boolean</span></span>|<span data-ttu-id="6a23d-122">Указывает, является ли шрифт полужирным.</span><span class="sxs-lookup"><span data-stu-id="6a23d-122">Represents the bold status of font.</span></span>|
|<span data-ttu-id="6a23d-123">color</span><span class="sxs-lookup"><span data-stu-id="6a23d-123">color</span></span>|<span data-ttu-id="6a23d-124">string</span><span class="sxs-lookup"><span data-stu-id="6a23d-124">string</span></span>|<span data-ttu-id="6a23d-p101">HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.</span><span class="sxs-lookup"><span data-stu-id="6a23d-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="6a23d-128">italic</span><span class="sxs-lookup"><span data-stu-id="6a23d-128">italic</span></span>|<span data-ttu-id="6a23d-129">boolean</span><span class="sxs-lookup"><span data-stu-id="6a23d-129">boolean</span></span>|<span data-ttu-id="6a23d-130">Указывает, применяется ли курсив.</span><span class="sxs-lookup"><span data-stu-id="6a23d-130">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="6a23d-131">name</span><span class="sxs-lookup"><span data-stu-id="6a23d-131">name</span></span>|<span data-ttu-id="6a23d-132">string</span><span class="sxs-lookup"><span data-stu-id="6a23d-132">string</span></span>|<span data-ttu-id="6a23d-133">Имя шрифта (например, Calibri)</span><span class="sxs-lookup"><span data-stu-id="6a23d-133">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="6a23d-134">size</span><span class="sxs-lookup"><span data-stu-id="6a23d-134">size</span></span>|<span data-ttu-id="6a23d-135">double</span><span class="sxs-lookup"><span data-stu-id="6a23d-135">double</span></span>|<span data-ttu-id="6a23d-136">размер шрифта</span><span class="sxs-lookup"><span data-stu-id="6a23d-136">Font size.</span></span>|
|<span data-ttu-id="6a23d-137">underline</span><span class="sxs-lookup"><span data-stu-id="6a23d-137">underline</span></span>|<span data-ttu-id="6a23d-138">string</span><span class="sxs-lookup"><span data-stu-id="6a23d-138">string</span></span>|<span data-ttu-id="6a23d-139">Тип подчеркивания, применяемый для шрифта.</span><span class="sxs-lookup"><span data-stu-id="6a23d-139">Type of underline applied to the font.</span></span> <span data-ttu-id="6a23d-140">Допустимые значения: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="6a23d-140">The possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a23d-141">Связи</span><span class="sxs-lookup"><span data-stu-id="6a23d-141">Relationships</span></span>
<span data-ttu-id="6a23d-142">Нет</span><span class="sxs-lookup"><span data-stu-id="6a23d-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6a23d-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6a23d-143">JSON representation</span></span>

<span data-ttu-id="6a23d-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a23d-144">Here is a JSON representation of the resource.</span></span>

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

