---
title: Тип ресурса ChartFont
description: Этот объект представляет атрибуты шрифта (название, размер, цвет и т. д.) для объекта диаграммы.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: c507a966dc6b29e46935c5c77a85b557a84cc69c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543733"
---
# <a name="chartfont-resource-type"></a><span data-ttu-id="4fd4d-103">Тип ресурса ChartFont</span><span class="sxs-lookup"><span data-stu-id="4fd4d-103">ChartFont resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4fd4d-104">Этот объект представляет атрибуты шрифта (название, размер, цвет и т. д.) для объекта диаграммы.</span><span class="sxs-lookup"><span data-stu-id="4fd4d-104">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="4fd4d-105">Методы</span><span class="sxs-lookup"><span data-stu-id="4fd4d-105">Methods</span></span>

| <span data-ttu-id="4fd4d-106">Метод</span><span class="sxs-lookup"><span data-stu-id="4fd4d-106">Method</span></span>           | <span data-ttu-id="4fd4d-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4fd4d-107">Return Type</span></span>    |<span data-ttu-id="4fd4d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4fd4d-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4fd4d-109">Получение объекта ChartFont</span><span class="sxs-lookup"><span data-stu-id="4fd4d-109">Get ChartFont</span></span>](../api/chartfont-get.md) | [<span data-ttu-id="4fd4d-110">ChartFont</span><span class="sxs-lookup"><span data-stu-id="4fd4d-110">ChartFont</span></span>](chartfont.md) |<span data-ttu-id="4fd4d-111">Чтение свойств и связей объекта chartFont.</span><span class="sxs-lookup"><span data-stu-id="4fd4d-111">Read properties and relationships of chartFont object.</span></span>|
|[<span data-ttu-id="4fd4d-112">Обновление</span><span class="sxs-lookup"><span data-stu-id="4fd4d-112">Update</span></span>](../api/chartfont-update.md) | [<span data-ttu-id="4fd4d-113">ChartFont</span><span class="sxs-lookup"><span data-stu-id="4fd4d-113">ChartFont</span></span>](chartfont.md)   |<span data-ttu-id="4fd4d-114">Обновление объекта ChartFont.</span><span class="sxs-lookup"><span data-stu-id="4fd4d-114">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4fd4d-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="4fd4d-115">Properties</span></span>
| <span data-ttu-id="4fd4d-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="4fd4d-116">Property</span></span>     | <span data-ttu-id="4fd4d-117">Тип</span><span class="sxs-lookup"><span data-stu-id="4fd4d-117">Type</span></span>   |<span data-ttu-id="4fd4d-118">Описание</span><span class="sxs-lookup"><span data-stu-id="4fd4d-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4fd4d-119">bold</span><span class="sxs-lookup"><span data-stu-id="4fd4d-119">bold</span></span>|<span data-ttu-id="4fd4d-120">логический</span><span class="sxs-lookup"><span data-stu-id="4fd4d-120">boolean</span></span>|<span data-ttu-id="4fd4d-121">Указывает, является ли шрифт полужирным.</span><span class="sxs-lookup"><span data-stu-id="4fd4d-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="4fd4d-122">color</span><span class="sxs-lookup"><span data-stu-id="4fd4d-122">color</span></span>|<span data-ttu-id="4fd4d-123">строка</span><span class="sxs-lookup"><span data-stu-id="4fd4d-123">string</span></span>|<span data-ttu-id="4fd4d-p101">HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.</span><span class="sxs-lookup"><span data-stu-id="4fd4d-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="4fd4d-127">italic</span><span class="sxs-lookup"><span data-stu-id="4fd4d-127">italic</span></span>|<span data-ttu-id="4fd4d-128">boolean</span><span class="sxs-lookup"><span data-stu-id="4fd4d-128">boolean</span></span>|<span data-ttu-id="4fd4d-129">Указывает, применяется ли курсив.</span><span class="sxs-lookup"><span data-stu-id="4fd4d-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="4fd4d-130">name</span><span class="sxs-lookup"><span data-stu-id="4fd4d-130">name</span></span>|<span data-ttu-id="4fd4d-131">string</span><span class="sxs-lookup"><span data-stu-id="4fd4d-131">string</span></span>|<span data-ttu-id="4fd4d-132">Имя шрифта (например, Calibri)</span><span class="sxs-lookup"><span data-stu-id="4fd4d-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="4fd4d-133">size</span><span class="sxs-lookup"><span data-stu-id="4fd4d-133">size</span></span>|<span data-ttu-id="4fd4d-134">Double</span><span class="sxs-lookup"><span data-stu-id="4fd4d-134">double</span></span>|<span data-ttu-id="4fd4d-135">Размер шрифта (например, 11)</span><span class="sxs-lookup"><span data-stu-id="4fd4d-135">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="4fd4d-136">underline</span><span class="sxs-lookup"><span data-stu-id="4fd4d-136">underline</span></span>|<span data-ttu-id="4fd4d-137">string</span><span class="sxs-lookup"><span data-stu-id="4fd4d-137">string</span></span>|<span data-ttu-id="4fd4d-p102">Тип подчеркивания, применяемый для шрифта. Возможные значения: `None`, `Single`.</span><span class="sxs-lookup"><span data-stu-id="4fd4d-p102">Type of underline applied to the font. Possible values are: `None`, `Single`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4fd4d-140">Отношения</span><span class="sxs-lookup"><span data-stu-id="4fd4d-140">Relationships</span></span>
<span data-ttu-id="4fd4d-141">Нет</span><span class="sxs-lookup"><span data-stu-id="4fd4d-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="4fd4d-142">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4fd4d-142">JSON representation</span></span>

<span data-ttu-id="4fd4d-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4fd4d-143">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "ChartFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartfont.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
