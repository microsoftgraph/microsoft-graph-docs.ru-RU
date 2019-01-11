---
title: Тип ресурса ChartFont
description: Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта диаграммы.
localization_priority: Normal
ms.openlocfilehash: 0df14f98993c33b6b3eb3c0b2ea9fbdf211a8124
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824166"
---
# <a name="chartfont-resource-type"></a><span data-ttu-id="3b52f-103">Тип ресурса ChartFont</span><span class="sxs-lookup"><span data-stu-id="3b52f-103">ChartFont resource type</span></span>

> <span data-ttu-id="3b52f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3b52f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b52f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b52f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3b52f-106">Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="3b52f-106">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="3b52f-107">Методы</span><span class="sxs-lookup"><span data-stu-id="3b52f-107">Methods</span></span>

| <span data-ttu-id="3b52f-108">Метод</span><span class="sxs-lookup"><span data-stu-id="3b52f-108">Method</span></span>           | <span data-ttu-id="3b52f-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3b52f-109">Return Type</span></span>    |<span data-ttu-id="3b52f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3b52f-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3b52f-111">Получение объекта ChartFont</span><span class="sxs-lookup"><span data-stu-id="3b52f-111">Get ChartFont</span></span>](../api/chartfont-get.md) | [<span data-ttu-id="3b52f-112">ChartFont</span><span class="sxs-lookup"><span data-stu-id="3b52f-112">ChartFont</span></span>](chartfont.md) |<span data-ttu-id="3b52f-113">Чтение свойств и связей объекта chartFont.</span><span class="sxs-lookup"><span data-stu-id="3b52f-113">Read properties and relationships of chartFont object.</span></span>|
|<span data-ttu-id="3b52f-114">[обновление](../api/chartfont-update.md).</span><span class="sxs-lookup"><span data-stu-id="3b52f-114">[Update](../api/chartfont-update.md)</span></span> | [<span data-ttu-id="3b52f-115">ChartFont</span><span class="sxs-lookup"><span data-stu-id="3b52f-115">ChartFont</span></span>](chartfont.md)   |<span data-ttu-id="3b52f-116">Обновление объекта ChartFont.</span><span class="sxs-lookup"><span data-stu-id="3b52f-116">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3b52f-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="3b52f-117">Properties</span></span>
| <span data-ttu-id="3b52f-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b52f-118">Property</span></span>     | <span data-ttu-id="3b52f-119">Тип</span><span class="sxs-lookup"><span data-stu-id="3b52f-119">Type</span></span>   |<span data-ttu-id="3b52f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3b52f-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b52f-121">bold</span><span class="sxs-lookup"><span data-stu-id="3b52f-121">bold</span></span>|<span data-ttu-id="3b52f-122">boolean</span><span class="sxs-lookup"><span data-stu-id="3b52f-122">boolean</span></span>|<span data-ttu-id="3b52f-123">Указывает, является ли шрифт полужирным.</span><span class="sxs-lookup"><span data-stu-id="3b52f-123">Represents the bold status of font.</span></span>|
|<span data-ttu-id="3b52f-124">color</span><span class="sxs-lookup"><span data-stu-id="3b52f-124">color</span></span>|<span data-ttu-id="3b52f-125">строка</span><span class="sxs-lookup"><span data-stu-id="3b52f-125">string</span></span>|<span data-ttu-id="3b52f-p102">HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.</span><span class="sxs-lookup"><span data-stu-id="3b52f-p102">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="3b52f-129">italic</span><span class="sxs-lookup"><span data-stu-id="3b52f-129">italic</span></span>|<span data-ttu-id="3b52f-130">boolean</span><span class="sxs-lookup"><span data-stu-id="3b52f-130">boolean</span></span>|<span data-ttu-id="3b52f-131">Указывает, применяется ли курсив.</span><span class="sxs-lookup"><span data-stu-id="3b52f-131">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="3b52f-132">name</span><span class="sxs-lookup"><span data-stu-id="3b52f-132">name</span></span>|<span data-ttu-id="3b52f-133">строка</span><span class="sxs-lookup"><span data-stu-id="3b52f-133">string</span></span>|<span data-ttu-id="3b52f-134">Имя шрифта (например, Calibri)</span><span class="sxs-lookup"><span data-stu-id="3b52f-134">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="3b52f-135">size</span><span class="sxs-lookup"><span data-stu-id="3b52f-135">size</span></span>|<span data-ttu-id="3b52f-136">Double</span><span class="sxs-lookup"><span data-stu-id="3b52f-136">double</span></span>|<span data-ttu-id="3b52f-137">Размер шрифта (например, 11)</span><span class="sxs-lookup"><span data-stu-id="3b52f-137">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="3b52f-138">underline</span><span class="sxs-lookup"><span data-stu-id="3b52f-138">underline</span></span>|<span data-ttu-id="3b52f-139">строка</span><span class="sxs-lookup"><span data-stu-id="3b52f-139">string</span></span>|<span data-ttu-id="3b52f-p103">Тип подчеркивания, применяемый для шрифта. Возможные значения: `None`, `Single`.</span><span class="sxs-lookup"><span data-stu-id="3b52f-p103">Type of underline applied to the font. Possible values are: `None`, `Single`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b52f-142">Связи</span><span class="sxs-lookup"><span data-stu-id="3b52f-142">Relationships</span></span>
<span data-ttu-id="3b52f-143">Нет</span><span class="sxs-lookup"><span data-stu-id="3b52f-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3b52f-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3b52f-144">JSON representation</span></span>

<span data-ttu-id="3b52f-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b52f-145">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartFont"
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
  "description": "ChartFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
