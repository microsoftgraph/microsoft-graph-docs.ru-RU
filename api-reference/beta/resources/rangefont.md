---
title: Тип ресурса RangeFont
description: Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 2dee07b7d2573081650bdd15799e4884c774e171
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563419"
---
# <a name="rangefont-resource-type"></a><span data-ttu-id="17240-103">Тип ресурса RangeFont</span><span class="sxs-lookup"><span data-stu-id="17240-103">RangeFont resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17240-104">Этот объект представляет атрибуты шрифта (имя, размер, цвет и т. д.) для объекта.</span><span class="sxs-lookup"><span data-stu-id="17240-104">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="17240-105">Методы</span><span class="sxs-lookup"><span data-stu-id="17240-105">Methods</span></span>

| <span data-ttu-id="17240-106">Метод</span><span class="sxs-lookup"><span data-stu-id="17240-106">Method</span></span>           | <span data-ttu-id="17240-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="17240-107">Return Type</span></span>    |<span data-ttu-id="17240-108">Описание</span><span class="sxs-lookup"><span data-stu-id="17240-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="17240-109">Получение объекта RangeFont</span><span class="sxs-lookup"><span data-stu-id="17240-109">Get RangeFont</span></span>](../api/rangefont-get.md) | [<span data-ttu-id="17240-110">RangeFont</span><span class="sxs-lookup"><span data-stu-id="17240-110">RangeFont</span></span>](rangefont.md) |<span data-ttu-id="17240-111">Чтение свойств и связей объекта rangeFont.</span><span class="sxs-lookup"><span data-stu-id="17240-111">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="17240-112">Обновление</span><span class="sxs-lookup"><span data-stu-id="17240-112">Update</span></span>](../api/rangefont-update.md) | [<span data-ttu-id="17240-113">RangeFont</span><span class="sxs-lookup"><span data-stu-id="17240-113">RangeFont</span></span>](rangefont.md)   |<span data-ttu-id="17240-114">Обновление объекта RangeFont.</span><span class="sxs-lookup"><span data-stu-id="17240-114">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="17240-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="17240-115">Properties</span></span>
| <span data-ttu-id="17240-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="17240-116">Property</span></span>     | <span data-ttu-id="17240-117">Тип</span><span class="sxs-lookup"><span data-stu-id="17240-117">Type</span></span>   |<span data-ttu-id="17240-118">Описание</span><span class="sxs-lookup"><span data-stu-id="17240-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17240-119">bold</span><span class="sxs-lookup"><span data-stu-id="17240-119">bold</span></span>|<span data-ttu-id="17240-120">boolean</span><span class="sxs-lookup"><span data-stu-id="17240-120">boolean</span></span>|<span data-ttu-id="17240-121">Указывает, является ли шрифт полужирным.</span><span class="sxs-lookup"><span data-stu-id="17240-121">Represents the bold status of font.</span></span>|
|<span data-ttu-id="17240-122">color</span><span class="sxs-lookup"><span data-stu-id="17240-122">color</span></span>|<span data-ttu-id="17240-123">строка</span><span class="sxs-lookup"><span data-stu-id="17240-123">string</span></span>|<span data-ttu-id="17240-p101">HTML-код цвета текста. Например, значение #FF0000 обозначает красный цвет.</span><span class="sxs-lookup"><span data-stu-id="17240-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="17240-127">italic</span><span class="sxs-lookup"><span data-stu-id="17240-127">italic</span></span>|<span data-ttu-id="17240-128">boolean</span><span class="sxs-lookup"><span data-stu-id="17240-128">boolean</span></span>|<span data-ttu-id="17240-129">Указывает, применяется ли курсив.</span><span class="sxs-lookup"><span data-stu-id="17240-129">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="17240-130">name</span><span class="sxs-lookup"><span data-stu-id="17240-130">name</span></span>|<span data-ttu-id="17240-131">string</span><span class="sxs-lookup"><span data-stu-id="17240-131">string</span></span>|<span data-ttu-id="17240-132">Имя шрифта (например, Calibri)</span><span class="sxs-lookup"><span data-stu-id="17240-132">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="17240-133">size</span><span class="sxs-lookup"><span data-stu-id="17240-133">size</span></span>|<span data-ttu-id="17240-134">double</span><span class="sxs-lookup"><span data-stu-id="17240-134">double</span></span>|<span data-ttu-id="17240-135">размер шрифта</span><span class="sxs-lookup"><span data-stu-id="17240-135">Font size.</span></span>|
|<span data-ttu-id="17240-136">underline</span><span class="sxs-lookup"><span data-stu-id="17240-136">underline</span></span>|<span data-ttu-id="17240-137">string</span><span class="sxs-lookup"><span data-stu-id="17240-137">string</span></span>|<span data-ttu-id="17240-p102">Тип подчеркивания, применяемый для шрифта. Возможные значения: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="17240-p102">Type of underline applied to the font. Possible values are: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="17240-140">Отношения</span><span class="sxs-lookup"><span data-stu-id="17240-140">Relationships</span></span>
<span data-ttu-id="17240-141">Нет</span><span class="sxs-lookup"><span data-stu-id="17240-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="17240-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="17240-142">JSON representation</span></span>

<span data-ttu-id="17240-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="17240-143">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "RangeFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/rangefont.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
