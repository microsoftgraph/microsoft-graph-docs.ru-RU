---
title: Тип ресурса RangeFont
description: Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: e6f448df142ffdc0c20e39045b4cd77a6c224a6f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912780"
---
# <a name="rangefont-resource-type"></a><span data-ttu-id="96904-103">Тип ресурса RangeFont</span><span class="sxs-lookup"><span data-stu-id="96904-103">RangeFont resource type</span></span>

> <span data-ttu-id="96904-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="96904-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96904-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96904-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="96904-106">Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта.</span><span class="sxs-lookup"><span data-stu-id="96904-106">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="96904-107">Методы</span><span class="sxs-lookup"><span data-stu-id="96904-107">Methods</span></span>

| <span data-ttu-id="96904-108">Метод</span><span class="sxs-lookup"><span data-stu-id="96904-108">Method</span></span>           | <span data-ttu-id="96904-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="96904-109">Return Type</span></span>    |<span data-ttu-id="96904-110">Описание</span><span class="sxs-lookup"><span data-stu-id="96904-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="96904-111">Получение объекта RangeFont</span><span class="sxs-lookup"><span data-stu-id="96904-111">Get RangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="96904-112">RangeFont</span><span class="sxs-lookup"><span data-stu-id="96904-112">RangeFont</span></span>](rangefont.md) |<span data-ttu-id="96904-113">Чтение свойств и связей объекта rangeFont.</span><span class="sxs-lookup"><span data-stu-id="96904-113">Read properties and relationships of rangeFont object.</span></span>|
|<span data-ttu-id="96904-114">[обновление](../api/rangefont-update.md).</span><span class="sxs-lookup"><span data-stu-id="96904-114">[Update](../api/rangefont-update.md)</span></span> | [<span data-ttu-id="96904-115">RangeFont</span><span class="sxs-lookup"><span data-stu-id="96904-115">RangeFont</span></span>](rangefont.md)   |<span data-ttu-id="96904-116">Обновление объекта RangeFont.</span><span class="sxs-lookup"><span data-stu-id="96904-116">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="96904-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="96904-117">Properties</span></span>
| <span data-ttu-id="96904-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="96904-118">Property</span></span>     | <span data-ttu-id="96904-119">Тип</span><span class="sxs-lookup"><span data-stu-id="96904-119">Type</span></span>   |<span data-ttu-id="96904-120">Описание</span><span class="sxs-lookup"><span data-stu-id="96904-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96904-121">bold</span><span class="sxs-lookup"><span data-stu-id="96904-121">bold</span></span>|<span data-ttu-id="96904-122">boolean</span><span class="sxs-lookup"><span data-stu-id="96904-122">boolean</span></span>|<span data-ttu-id="96904-123">Указывает, является ли шрифт полужирным.</span><span class="sxs-lookup"><span data-stu-id="96904-123">Represents the bold status of font.</span></span>|
|<span data-ttu-id="96904-124">color</span><span class="sxs-lookup"><span data-stu-id="96904-124">color</span></span>|<span data-ttu-id="96904-125">строка</span><span class="sxs-lookup"><span data-stu-id="96904-125">string</span></span>|<span data-ttu-id="96904-p102">HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.</span><span class="sxs-lookup"><span data-stu-id="96904-p102">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="96904-129">italic</span><span class="sxs-lookup"><span data-stu-id="96904-129">italic</span></span>|<span data-ttu-id="96904-130">boolean</span><span class="sxs-lookup"><span data-stu-id="96904-130">boolean</span></span>|<span data-ttu-id="96904-131">Указывает, применяется ли курсив.</span><span class="sxs-lookup"><span data-stu-id="96904-131">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="96904-132">name</span><span class="sxs-lookup"><span data-stu-id="96904-132">name</span></span>|<span data-ttu-id="96904-133">строка</span><span class="sxs-lookup"><span data-stu-id="96904-133">string</span></span>|<span data-ttu-id="96904-134">Имя шрифта (например, Calibri)</span><span class="sxs-lookup"><span data-stu-id="96904-134">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="96904-135">size</span><span class="sxs-lookup"><span data-stu-id="96904-135">size</span></span>|<span data-ttu-id="96904-136">double</span><span class="sxs-lookup"><span data-stu-id="96904-136">double</span></span>|<span data-ttu-id="96904-137">font-size</span><span class="sxs-lookup"><span data-stu-id="96904-137">Font size.</span></span>|
|<span data-ttu-id="96904-138">underline</span><span class="sxs-lookup"><span data-stu-id="96904-138">underline</span></span>|<span data-ttu-id="96904-139">строка</span><span class="sxs-lookup"><span data-stu-id="96904-139">string</span></span>|<span data-ttu-id="96904-p103">Тип подчеркивания, применяемый для шрифта. Возможные значения: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="96904-p103">Type of underline applied to the font. Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96904-142">Связи</span><span class="sxs-lookup"><span data-stu-id="96904-142">Relationships</span></span>
<span data-ttu-id="96904-143">Нет</span><span class="sxs-lookup"><span data-stu-id="96904-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="96904-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="96904-144">JSON representation</span></span>

<span data-ttu-id="96904-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="96904-145">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "RangeFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
