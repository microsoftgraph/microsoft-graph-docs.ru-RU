---
title: Тип ресурса ChartFont
description: Этот объект представляет атрибуты шрифта (название, размер, цвет и т. д.) для объекта диаграммы.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 1768e40edde1d02c109e77c7e7ca3c2dd0ffdafa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531855"
---
# <a name="chartfont-resource-type"></a><span data-ttu-id="6939a-103">Тип ресурса ChartFont</span><span class="sxs-lookup"><span data-stu-id="6939a-103">ChartFont resource type</span></span>

<span data-ttu-id="6939a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6939a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6939a-105">Этот объект представляет атрибуты шрифта (название, размер, цвет и т. д.) для объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="6939a-105">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="6939a-106">Методы</span><span class="sxs-lookup"><span data-stu-id="6939a-106">Methods</span></span>

| <span data-ttu-id="6939a-107">Метод</span><span class="sxs-lookup"><span data-stu-id="6939a-107">Method</span></span>           | <span data-ttu-id="6939a-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6939a-108">Return Type</span></span>    |<span data-ttu-id="6939a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6939a-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6939a-110">Получение объекта ChartFont</span><span class="sxs-lookup"><span data-stu-id="6939a-110">Get ChartFont</span></span>](../api/chartfont-get.md) | [<span data-ttu-id="6939a-111">воркбукчартфонт</span><span class="sxs-lookup"><span data-stu-id="6939a-111">WorkbookChartFont</span></span>](chartfont.md) |<span data-ttu-id="6939a-112">Чтение свойств и связей объекта chartFont.</span><span class="sxs-lookup"><span data-stu-id="6939a-112">Read properties and relationships of chartFont object.</span></span>|
|[<span data-ttu-id="6939a-113">Обновление</span><span class="sxs-lookup"><span data-stu-id="6939a-113">Update</span></span>](../api/chartfont-update.md) | [<span data-ttu-id="6939a-114">воркбукчартфонт</span><span class="sxs-lookup"><span data-stu-id="6939a-114">WorkbookChartFont</span></span>](chartfont.md)   |<span data-ttu-id="6939a-115">Обновление объекта ChartFont.</span><span class="sxs-lookup"><span data-stu-id="6939a-115">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6939a-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="6939a-116">Properties</span></span>
| <span data-ttu-id="6939a-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="6939a-117">Property</span></span>     | <span data-ttu-id="6939a-118">Тип</span><span class="sxs-lookup"><span data-stu-id="6939a-118">Type</span></span>   |<span data-ttu-id="6939a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="6939a-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6939a-120">bold</span><span class="sxs-lookup"><span data-stu-id="6939a-120">bold</span></span>|<span data-ttu-id="6939a-121">boolean</span><span class="sxs-lookup"><span data-stu-id="6939a-121">boolean</span></span>|<span data-ttu-id="6939a-122">Указывает, является ли шрифт полужирным.</span><span class="sxs-lookup"><span data-stu-id="6939a-122">Represents the bold status of font.</span></span>|
|<span data-ttu-id="6939a-123">color</span><span class="sxs-lookup"><span data-stu-id="6939a-123">color</span></span>|<span data-ttu-id="6939a-124">строка</span><span class="sxs-lookup"><span data-stu-id="6939a-124">string</span></span>|<span data-ttu-id="6939a-p101">HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.</span><span class="sxs-lookup"><span data-stu-id="6939a-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="6939a-128">italic</span><span class="sxs-lookup"><span data-stu-id="6939a-128">italic</span></span>|<span data-ttu-id="6939a-129">boolean</span><span class="sxs-lookup"><span data-stu-id="6939a-129">boolean</span></span>|<span data-ttu-id="6939a-130">Указывает, применяется ли курсив.</span><span class="sxs-lookup"><span data-stu-id="6939a-130">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="6939a-131">name</span><span class="sxs-lookup"><span data-stu-id="6939a-131">name</span></span>|<span data-ttu-id="6939a-132">string</span><span class="sxs-lookup"><span data-stu-id="6939a-132">string</span></span>|<span data-ttu-id="6939a-133">Имя шрифта (например, Calibri)</span><span class="sxs-lookup"><span data-stu-id="6939a-133">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="6939a-134">size</span><span class="sxs-lookup"><span data-stu-id="6939a-134">size</span></span>|<span data-ttu-id="6939a-135">Double</span><span class="sxs-lookup"><span data-stu-id="6939a-135">double</span></span>|<span data-ttu-id="6939a-136">Размер шрифта (например, 11)</span><span class="sxs-lookup"><span data-stu-id="6939a-136">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="6939a-137">underline</span><span class="sxs-lookup"><span data-stu-id="6939a-137">underline</span></span>|<span data-ttu-id="6939a-138">string</span><span class="sxs-lookup"><span data-stu-id="6939a-138">string</span></span>|<span data-ttu-id="6939a-139">Тип подчеркивания, применяемый для шрифта.</span><span class="sxs-lookup"><span data-stu-id="6939a-139">Type of underline applied to the font.</span></span> <span data-ttu-id="6939a-140">Возможные значения: `None`, `Single`.</span><span class="sxs-lookup"><span data-stu-id="6939a-140">The possible values are: `None`, `Single`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6939a-141">Связи</span><span class="sxs-lookup"><span data-stu-id="6939a-141">Relationships</span></span>
<span data-ttu-id="6939a-142">Нет</span><span class="sxs-lookup"><span data-stu-id="6939a-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6939a-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6939a-143">JSON representation</span></span>

<span data-ttu-id="6939a-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6939a-144">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartFont"
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
