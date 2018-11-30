---
title: Тип ресурса RangeFont
description: Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта.
ms.openlocfilehash: bafb7c052458c7b3f4001d7e999acc14c7aaabee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027335"
---
# <a name="rangefont-resource-type"></a><span data-ttu-id="8d45c-103">Тип ресурса RangeFont</span><span class="sxs-lookup"><span data-stu-id="8d45c-103">RangeFont resource type</span></span>

<span data-ttu-id="8d45c-104">Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта.</span><span class="sxs-lookup"><span data-stu-id="8d45c-104">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="8d45c-105">Методы</span><span class="sxs-lookup"><span data-stu-id="8d45c-105">Methods</span></span>

| <span data-ttu-id="8d45c-106">Метод</span><span class="sxs-lookup"><span data-stu-id="8d45c-106">Method</span></span>           | <span data-ttu-id="8d45c-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8d45c-107">Return Type</span></span>    |<span data-ttu-id="8d45c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8d45c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8d45c-109">Получение объекта RangeFont</span><span class="sxs-lookup"><span data-stu-id="8d45c-109">Get RangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="8d45c-110">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="8d45c-110">WorkbookRangeFont</span></span>](rangefont.md) |<span data-ttu-id="8d45c-111">Чтение свойств и связей объекта rangeFont.</span><span class="sxs-lookup"><span data-stu-id="8d45c-111">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="8d45c-112">Update</span><span class="sxs-lookup"><span data-stu-id="8d45c-112">Update</span></span>](../api/rangefont-update.md) | [<span data-ttu-id="8d45c-113">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="8d45c-113">WorkbookRangeFont</span></span>](rangefont.md)   |<span data-ttu-id="8d45c-114">Обновление объекта RangeFont.</span><span class="sxs-lookup"><span data-stu-id="8d45c-114">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8d45c-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="8d45c-115">Properties</span></span>
| <span data-ttu-id="8d45c-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d45c-116">Property</span></span>     | <span data-ttu-id="8d45c-117">Тип</span><span class="sxs-lookup"><span data-stu-id="8d45c-117">Type</span></span>   |<span data-ttu-id="8d45c-118">Описание</span><span class="sxs-lookup"><span data-stu-id="8d45c-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d45c-119">bold</span><span class="sxs-lookup"><span data-stu-id="8d45c-119">bold</span></span>|<span data-ttu-id="8d45c-120">boolean</span><span class="sxs-lookup"><span data-stu-id="8d45c-120">boolean</span></span>|<span data-ttu-id="8d45c-121">Указывает, является ли шрифт полужирным.</span><span class="sxs-lookup"><span data-stu-id="8d45c-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="8d45c-122">color</span><span class="sxs-lookup"><span data-stu-id="8d45c-122">color</span></span>|<span data-ttu-id="8d45c-123">строка</span><span class="sxs-lookup"><span data-stu-id="8d45c-123">string</span></span>|<span data-ttu-id="8d45c-p101">HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.</span><span class="sxs-lookup"><span data-stu-id="8d45c-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="8d45c-127">italic</span><span class="sxs-lookup"><span data-stu-id="8d45c-127">italic</span></span>|<span data-ttu-id="8d45c-128">boolean</span><span class="sxs-lookup"><span data-stu-id="8d45c-128">boolean</span></span>|<span data-ttu-id="8d45c-129">Указывает, применяется ли курсив.</span><span class="sxs-lookup"><span data-stu-id="8d45c-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="8d45c-130">name</span><span class="sxs-lookup"><span data-stu-id="8d45c-130">name</span></span>|<span data-ttu-id="8d45c-131">строка</span><span class="sxs-lookup"><span data-stu-id="8d45c-131">string</span></span>|<span data-ttu-id="8d45c-132">Имя шрифта (например, Calibri)</span><span class="sxs-lookup"><span data-stu-id="8d45c-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="8d45c-133">size</span><span class="sxs-lookup"><span data-stu-id="8d45c-133">size</span></span>|<span data-ttu-id="8d45c-134">double</span><span class="sxs-lookup"><span data-stu-id="8d45c-134">double</span></span>|<span data-ttu-id="8d45c-135">font-size</span><span class="sxs-lookup"><span data-stu-id="8d45c-135">Font size.</span></span>|
|<span data-ttu-id="8d45c-136">underline</span><span class="sxs-lookup"><span data-stu-id="8d45c-136">underline</span></span>|<span data-ttu-id="8d45c-137">строка</span><span class="sxs-lookup"><span data-stu-id="8d45c-137">string</span></span>|<span data-ttu-id="8d45c-138">Тип подчеркивание шрифта.</span><span class="sxs-lookup"><span data-stu-id="8d45c-138">Type of underline applied to the font.</span></span> <span data-ttu-id="8d45c-139">Возможные значения: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="8d45c-139">The possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d45c-140">Связи</span><span class="sxs-lookup"><span data-stu-id="8d45c-140">Relationships</span></span>
<span data-ttu-id="8d45c-141">Нет</span><span class="sxs-lookup"><span data-stu-id="8d45c-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8d45c-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8d45c-142">JSON representation</span></span>

<span data-ttu-id="8d45c-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d45c-143">Here is a JSON representation of the resource.</span></span>

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