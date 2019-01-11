---
title: Тип ресурса RangeFont
description: Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта.
localization_priority: Normal
ms.openlocfilehash: b1ec2d6dc97b0403c3e52cb2faec11b25d805391
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864206"
---
# <a name="rangefont-resource-type"></a><span data-ttu-id="3afb0-103">Тип ресурса RangeFont</span><span class="sxs-lookup"><span data-stu-id="3afb0-103">RangeFont resource type</span></span>

> <span data-ttu-id="3afb0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3afb0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3afb0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3afb0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3afb0-106">Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта.</span><span class="sxs-lookup"><span data-stu-id="3afb0-106">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="3afb0-107">Методы</span><span class="sxs-lookup"><span data-stu-id="3afb0-107">Methods</span></span>

| <span data-ttu-id="3afb0-108">Метод</span><span class="sxs-lookup"><span data-stu-id="3afb0-108">Method</span></span>           | <span data-ttu-id="3afb0-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3afb0-109">Return Type</span></span>    |<span data-ttu-id="3afb0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3afb0-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3afb0-111">Получение объекта RangeFont</span><span class="sxs-lookup"><span data-stu-id="3afb0-111">Get RangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="3afb0-112">RangeFont</span><span class="sxs-lookup"><span data-stu-id="3afb0-112">RangeFont</span></span>](rangefont.md) |<span data-ttu-id="3afb0-113">Чтение свойств и связей объекта rangeFont.</span><span class="sxs-lookup"><span data-stu-id="3afb0-113">Read properties and relationships of rangeFont object.</span></span>|
|<span data-ttu-id="3afb0-114">[обновление](../api/rangefont-update.md).</span><span class="sxs-lookup"><span data-stu-id="3afb0-114">[Update](../api/rangefont-update.md)</span></span> | [<span data-ttu-id="3afb0-115">RangeFont</span><span class="sxs-lookup"><span data-stu-id="3afb0-115">RangeFont</span></span>](rangefont.md)   |<span data-ttu-id="3afb0-116">Обновление объекта RangeFont.</span><span class="sxs-lookup"><span data-stu-id="3afb0-116">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3afb0-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="3afb0-117">Properties</span></span>
| <span data-ttu-id="3afb0-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="3afb0-118">Property</span></span>     | <span data-ttu-id="3afb0-119">Тип</span><span class="sxs-lookup"><span data-stu-id="3afb0-119">Type</span></span>   |<span data-ttu-id="3afb0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3afb0-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3afb0-121">bold</span><span class="sxs-lookup"><span data-stu-id="3afb0-121">bold</span></span>|<span data-ttu-id="3afb0-122">boolean</span><span class="sxs-lookup"><span data-stu-id="3afb0-122">boolean</span></span>|<span data-ttu-id="3afb0-123">Указывает, является ли шрифт полужирным.</span><span class="sxs-lookup"><span data-stu-id="3afb0-123">Represents the bold status of font.</span></span>|
|<span data-ttu-id="3afb0-124">color</span><span class="sxs-lookup"><span data-stu-id="3afb0-124">color</span></span>|<span data-ttu-id="3afb0-125">строка</span><span class="sxs-lookup"><span data-stu-id="3afb0-125">string</span></span>|<span data-ttu-id="3afb0-p102">HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.</span><span class="sxs-lookup"><span data-stu-id="3afb0-p102">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="3afb0-129">italic</span><span class="sxs-lookup"><span data-stu-id="3afb0-129">italic</span></span>|<span data-ttu-id="3afb0-130">boolean</span><span class="sxs-lookup"><span data-stu-id="3afb0-130">boolean</span></span>|<span data-ttu-id="3afb0-131">Указывает, применяется ли курсив.</span><span class="sxs-lookup"><span data-stu-id="3afb0-131">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="3afb0-132">name</span><span class="sxs-lookup"><span data-stu-id="3afb0-132">name</span></span>|<span data-ttu-id="3afb0-133">строка</span><span class="sxs-lookup"><span data-stu-id="3afb0-133">string</span></span>|<span data-ttu-id="3afb0-134">Имя шрифта (например, Calibri)</span><span class="sxs-lookup"><span data-stu-id="3afb0-134">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="3afb0-135">size</span><span class="sxs-lookup"><span data-stu-id="3afb0-135">size</span></span>|<span data-ttu-id="3afb0-136">double</span><span class="sxs-lookup"><span data-stu-id="3afb0-136">double</span></span>|<span data-ttu-id="3afb0-137">font-size</span><span class="sxs-lookup"><span data-stu-id="3afb0-137">Font size.</span></span>|
|<span data-ttu-id="3afb0-138">underline</span><span class="sxs-lookup"><span data-stu-id="3afb0-138">underline</span></span>|<span data-ttu-id="3afb0-139">строка</span><span class="sxs-lookup"><span data-stu-id="3afb0-139">string</span></span>|<span data-ttu-id="3afb0-p103">Тип подчеркивания, применяемый для шрифта. Возможные значения: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="3afb0-p103">Type of underline applied to the font. Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3afb0-142">Связи</span><span class="sxs-lookup"><span data-stu-id="3afb0-142">Relationships</span></span>
<span data-ttu-id="3afb0-143">Нет</span><span class="sxs-lookup"><span data-stu-id="3afb0-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3afb0-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3afb0-144">JSON representation</span></span>

<span data-ttu-id="3afb0-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3afb0-145">Here is a JSON representation of the resource.</span></span>

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
