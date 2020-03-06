---
title: Тип ресурса RangeFont
description: Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 2d519d4a21af17dd10fa840e2e81bab9aef35c19
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533908"
---
# <a name="rangefont-resource-type"></a><span data-ttu-id="30596-103">Тип ресурса RangeFont</span><span class="sxs-lookup"><span data-stu-id="30596-103">RangeFont resource type</span></span>

<span data-ttu-id="30596-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30596-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="30596-105">Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта.</span><span class="sxs-lookup"><span data-stu-id="30596-105">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="30596-106">Методы</span><span class="sxs-lookup"><span data-stu-id="30596-106">Methods</span></span>

| <span data-ttu-id="30596-107">Метод</span><span class="sxs-lookup"><span data-stu-id="30596-107">Method</span></span>           | <span data-ttu-id="30596-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="30596-108">Return Type</span></span>    |<span data-ttu-id="30596-109">Описание</span><span class="sxs-lookup"><span data-stu-id="30596-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="30596-110">Получение объекта RangeFont</span><span class="sxs-lookup"><span data-stu-id="30596-110">Get RangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="30596-111">воркбукранжефонт</span><span class="sxs-lookup"><span data-stu-id="30596-111">WorkbookRangeFont</span></span>](rangefont.md) |<span data-ttu-id="30596-112">Чтение свойств и связей объекта rangeFont.</span><span class="sxs-lookup"><span data-stu-id="30596-112">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="30596-113">Обновление</span><span class="sxs-lookup"><span data-stu-id="30596-113">Update</span></span>](../api/rangefont-update.md) | [<span data-ttu-id="30596-114">воркбукранжефонт</span><span class="sxs-lookup"><span data-stu-id="30596-114">WorkbookRangeFont</span></span>](rangefont.md)   |<span data-ttu-id="30596-115">Обновление объекта RangeFont.</span><span class="sxs-lookup"><span data-stu-id="30596-115">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="30596-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="30596-116">Properties</span></span>
| <span data-ttu-id="30596-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="30596-117">Property</span></span>     | <span data-ttu-id="30596-118">Тип</span><span class="sxs-lookup"><span data-stu-id="30596-118">Type</span></span>   |<span data-ttu-id="30596-119">Описание</span><span class="sxs-lookup"><span data-stu-id="30596-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30596-120">bold</span><span class="sxs-lookup"><span data-stu-id="30596-120">bold</span></span>|<span data-ttu-id="30596-121">boolean</span><span class="sxs-lookup"><span data-stu-id="30596-121">boolean</span></span>|<span data-ttu-id="30596-122">Указывает, является ли шрифт полужирным.</span><span class="sxs-lookup"><span data-stu-id="30596-122">Represents the bold status of font.</span></span>|
|<span data-ttu-id="30596-123">color</span><span class="sxs-lookup"><span data-stu-id="30596-123">color</span></span>|<span data-ttu-id="30596-124">строка</span><span class="sxs-lookup"><span data-stu-id="30596-124">string</span></span>|<span data-ttu-id="30596-p101">HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.</span><span class="sxs-lookup"><span data-stu-id="30596-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="30596-128">italic</span><span class="sxs-lookup"><span data-stu-id="30596-128">italic</span></span>|<span data-ttu-id="30596-129">boolean</span><span class="sxs-lookup"><span data-stu-id="30596-129">boolean</span></span>|<span data-ttu-id="30596-130">Указывает, применяется ли курсив.</span><span class="sxs-lookup"><span data-stu-id="30596-130">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="30596-131">name</span><span class="sxs-lookup"><span data-stu-id="30596-131">name</span></span>|<span data-ttu-id="30596-132">string</span><span class="sxs-lookup"><span data-stu-id="30596-132">string</span></span>|<span data-ttu-id="30596-133">Имя шрифта (например, Calibri)</span><span class="sxs-lookup"><span data-stu-id="30596-133">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="30596-134">size</span><span class="sxs-lookup"><span data-stu-id="30596-134">size</span></span>|<span data-ttu-id="30596-135">double</span><span class="sxs-lookup"><span data-stu-id="30596-135">double</span></span>|<span data-ttu-id="30596-136">размер шрифта</span><span class="sxs-lookup"><span data-stu-id="30596-136">Font size.</span></span>|
|<span data-ttu-id="30596-137">underline</span><span class="sxs-lookup"><span data-stu-id="30596-137">underline</span></span>|<span data-ttu-id="30596-138">string</span><span class="sxs-lookup"><span data-stu-id="30596-138">string</span></span>|<span data-ttu-id="30596-139">Тип подчеркивания, применяемый для шрифта.</span><span class="sxs-lookup"><span data-stu-id="30596-139">Type of underline applied to the font.</span></span> <span data-ttu-id="30596-140">Допустимые значения: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="30596-140">The possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="30596-141">Связи</span><span class="sxs-lookup"><span data-stu-id="30596-141">Relationships</span></span>
<span data-ttu-id="30596-142">Нет</span><span class="sxs-lookup"><span data-stu-id="30596-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="30596-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="30596-143">JSON representation</span></span>

<span data-ttu-id="30596-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30596-144">Here is a JSON representation of the resource.</span></span>

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
