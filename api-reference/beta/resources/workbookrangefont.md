---
title: Тип ресурса Воркбукранжефонт
description: Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: b3982a8026cd720fe614b11405a37bed8626042d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964053"
---
# <a name="workbookrangefont-resource-type"></a><span data-ttu-id="6eb86-103">Тип ресурса Воркбукранжефонт</span><span class="sxs-lookup"><span data-stu-id="6eb86-103">workbookRangeFont resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6eb86-104">Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта.</span><span class="sxs-lookup"><span data-stu-id="6eb86-104">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="6eb86-105">Методы</span><span class="sxs-lookup"><span data-stu-id="6eb86-105">Methods</span></span>

| <span data-ttu-id="6eb86-106">Метод</span><span class="sxs-lookup"><span data-stu-id="6eb86-106">Method</span></span>           | <span data-ttu-id="6eb86-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6eb86-107">Return Type</span></span>    |<span data-ttu-id="6eb86-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6eb86-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6eb86-109">Получение Воркбукранжефонт</span><span class="sxs-lookup"><span data-stu-id="6eb86-109">Get workbookRangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="6eb86-110">Воркбукранжефонт</span><span class="sxs-lookup"><span data-stu-id="6eb86-110">workbookRangeFont</span></span>](workbookrangefont.md) |<span data-ttu-id="6eb86-111">Чтение свойств и связей объекта rangeFont.</span><span class="sxs-lookup"><span data-stu-id="6eb86-111">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="6eb86-112">Обновление</span><span class="sxs-lookup"><span data-stu-id="6eb86-112">Update</span></span>](../api/rangefont-update.md) | [<span data-ttu-id="6eb86-113">Воркбукранжефонт</span><span class="sxs-lookup"><span data-stu-id="6eb86-113">workbookRangeFont</span></span>](workbookrangefont.md)   |<span data-ttu-id="6eb86-114">Обновление объекта RangeFont.</span><span class="sxs-lookup"><span data-stu-id="6eb86-114">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6eb86-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="6eb86-115">Properties</span></span>
| <span data-ttu-id="6eb86-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="6eb86-116">Property</span></span>     | <span data-ttu-id="6eb86-117">Тип</span><span class="sxs-lookup"><span data-stu-id="6eb86-117">Type</span></span>   |<span data-ttu-id="6eb86-118">Описание</span><span class="sxs-lookup"><span data-stu-id="6eb86-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6eb86-119">bold</span><span class="sxs-lookup"><span data-stu-id="6eb86-119">bold</span></span>|<span data-ttu-id="6eb86-120">boolean</span><span class="sxs-lookup"><span data-stu-id="6eb86-120">boolean</span></span>|<span data-ttu-id="6eb86-121">Указывает, является ли шрифт полужирным.</span><span class="sxs-lookup"><span data-stu-id="6eb86-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="6eb86-122">color</span><span class="sxs-lookup"><span data-stu-id="6eb86-122">color</span></span>|<span data-ttu-id="6eb86-123">строка</span><span class="sxs-lookup"><span data-stu-id="6eb86-123">string</span></span>|<span data-ttu-id="6eb86-p101">HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.</span><span class="sxs-lookup"><span data-stu-id="6eb86-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="6eb86-127">italic</span><span class="sxs-lookup"><span data-stu-id="6eb86-127">italic</span></span>|<span data-ttu-id="6eb86-128">boolean</span><span class="sxs-lookup"><span data-stu-id="6eb86-128">boolean</span></span>|<span data-ttu-id="6eb86-129">Указывает, применяется ли курсив.</span><span class="sxs-lookup"><span data-stu-id="6eb86-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="6eb86-130">name</span><span class="sxs-lookup"><span data-stu-id="6eb86-130">name</span></span>|<span data-ttu-id="6eb86-131">string</span><span class="sxs-lookup"><span data-stu-id="6eb86-131">string</span></span>|<span data-ttu-id="6eb86-132">Имя шрифта (например, Calibri)</span><span class="sxs-lookup"><span data-stu-id="6eb86-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="6eb86-133">size</span><span class="sxs-lookup"><span data-stu-id="6eb86-133">size</span></span>|<span data-ttu-id="6eb86-134">double</span><span class="sxs-lookup"><span data-stu-id="6eb86-134">double</span></span>|<span data-ttu-id="6eb86-135">размер шрифта</span><span class="sxs-lookup"><span data-stu-id="6eb86-135">Font size.</span></span>|
|<span data-ttu-id="6eb86-136">underline</span><span class="sxs-lookup"><span data-stu-id="6eb86-136">underline</span></span>| <span data-ttu-id="6eb86-137">String</span><span class="sxs-lookup"><span data-stu-id="6eb86-137">String</span></span> |<span data-ttu-id="6eb86-138">Тип подчеркивания, применяемый для шрифта.</span><span class="sxs-lookup"><span data-stu-id="6eb86-138">Type of underline applied to the font.</span></span> <span data-ttu-id="6eb86-139">Возможные значения: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="6eb86-139">Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6eb86-140">Отношения</span><span class="sxs-lookup"><span data-stu-id="6eb86-140">Relationships</span></span>
<span data-ttu-id="6eb86-141">Нет</span><span class="sxs-lookup"><span data-stu-id="6eb86-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6eb86-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6eb86-142">JSON representation</span></span>

<span data-ttu-id="6eb86-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6eb86-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "RangeFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
