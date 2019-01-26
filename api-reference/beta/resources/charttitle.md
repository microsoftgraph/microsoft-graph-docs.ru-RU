---
title: Тип ресурса ChartTitle
description: Представляет объект заголовка диаграммы.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f0b669593bd9ca0768ad977ace8d54f5531301a4
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573097"
---
# <a name="charttitle-resource-type"></a><span data-ttu-id="27dbc-103">Тип ресурса ChartTitle</span><span class="sxs-lookup"><span data-stu-id="27dbc-103">ChartTitle resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27dbc-104">Представляет объект заголовка диаграммы.</span><span class="sxs-lookup"><span data-stu-id="27dbc-104">Represents a chart title object of a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="27dbc-105">Методы</span><span class="sxs-lookup"><span data-stu-id="27dbc-105">Methods</span></span>

| <span data-ttu-id="27dbc-106">Метод</span><span class="sxs-lookup"><span data-stu-id="27dbc-106">Method</span></span>           | <span data-ttu-id="27dbc-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="27dbc-107">Return Type</span></span>    |<span data-ttu-id="27dbc-108">Описание</span><span class="sxs-lookup"><span data-stu-id="27dbc-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="27dbc-109">Получение объекта ChartTitle</span><span class="sxs-lookup"><span data-stu-id="27dbc-109">Get ChartTitle</span></span>](../api/charttitle-get.md) | [<span data-ttu-id="27dbc-110">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="27dbc-110">WorkbookChartTitle</span></span>](charttitle.md) |<span data-ttu-id="27dbc-111">Чтение свойств и связей объекта chartTitle.</span><span class="sxs-lookup"><span data-stu-id="27dbc-111">Read properties and relationships of chartTitle object.</span></span>|
|[<span data-ttu-id="27dbc-112">Update</span><span class="sxs-lookup"><span data-stu-id="27dbc-112">Update</span></span>](../api/charttitle-update.md) | [<span data-ttu-id="27dbc-113">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="27dbc-113">WorkbookChartTitle</span></span>](charttitle.md)    |<span data-ttu-id="27dbc-114">Обновление объекта ChartTitle.</span><span class="sxs-lookup"><span data-stu-id="27dbc-114">Update ChartTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="27dbc-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="27dbc-115">Properties</span></span>
| <span data-ttu-id="27dbc-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="27dbc-116">Property</span></span>     | <span data-ttu-id="27dbc-117">Тип</span><span class="sxs-lookup"><span data-stu-id="27dbc-117">Type</span></span>   |<span data-ttu-id="27dbc-118">Описание</span><span class="sxs-lookup"><span data-stu-id="27dbc-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27dbc-119">overlay</span><span class="sxs-lookup"><span data-stu-id="27dbc-119">overlay</span></span>|<span data-ttu-id="27dbc-120">boolean</span><span class="sxs-lookup"><span data-stu-id="27dbc-120">boolean</span></span>|<span data-ttu-id="27dbc-121">Логическое значение, указывающее, отображается ли заголовок диаграммы поверх нее.</span><span class="sxs-lookup"><span data-stu-id="27dbc-121">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="27dbc-122">text</span><span class="sxs-lookup"><span data-stu-id="27dbc-122">text</span></span>|<span data-ttu-id="27dbc-123">строка</span><span class="sxs-lookup"><span data-stu-id="27dbc-123">string</span></span>|<span data-ttu-id="27dbc-124">Представляет текст заголовка диаграммы.</span><span class="sxs-lookup"><span data-stu-id="27dbc-124">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="27dbc-125">visible</span><span class="sxs-lookup"><span data-stu-id="27dbc-125">visible</span></span>|<span data-ttu-id="27dbc-126">boolean</span><span class="sxs-lookup"><span data-stu-id="27dbc-126">boolean</span></span>|<span data-ttu-id="27dbc-127">Логическое значение, представляющее видимость объекта заголовка диаграммы.</span><span class="sxs-lookup"><span data-stu-id="27dbc-127">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="27dbc-128">Связи</span><span class="sxs-lookup"><span data-stu-id="27dbc-128">Relationships</span></span>
| <span data-ttu-id="27dbc-129">Связь</span><span class="sxs-lookup"><span data-stu-id="27dbc-129">Relationship</span></span> | <span data-ttu-id="27dbc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="27dbc-130">Type</span></span>   |<span data-ttu-id="27dbc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="27dbc-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27dbc-132">format</span><span class="sxs-lookup"><span data-stu-id="27dbc-132">format</span></span>|[<span data-ttu-id="27dbc-133">WorkbookChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="27dbc-133">WorkbookChartTitleFormat</span></span>](charttitleformat.md)|<span data-ttu-id="27dbc-p101">Представляет форматирование названия диаграммы, включая формат заливки и шрифта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27dbc-p101">Represents the formatting of a chart title, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="27dbc-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="27dbc-136">JSON representation</span></span>

<span data-ttu-id="27dbc-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27dbc-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartTitle"
}-->

```json
{
  "overlay": true,
  "text": "string",
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/charttitle.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
