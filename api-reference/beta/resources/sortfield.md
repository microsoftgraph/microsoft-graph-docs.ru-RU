---
title: Тип ресурса SortField
description: Представляет условие в операции сортировки.
localization_priority: Normal
ms.openlocfilehash: 52817df89ed130b6984ae3a76da775e0e000dee5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521637"
---
# <a name="sortfield-resource-type"></a><span data-ttu-id="f931e-103">Тип ресурса SortField</span><span class="sxs-lookup"><span data-stu-id="f931e-103">SortField resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f931e-104">Представляет условие в операции сортировки.</span><span class="sxs-lookup"><span data-stu-id="f931e-104">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="f931e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f931e-105">Properties</span></span>
| <span data-ttu-id="f931e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f931e-106">Property</span></span>     | <span data-ttu-id="f931e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f931e-107">Type</span></span>   |<span data-ttu-id="f931e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f931e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f931e-109">ascending</span><span class="sxs-lookup"><span data-stu-id="f931e-109">ascending</span></span>|<span data-ttu-id="f931e-110">boolean</span><span class="sxs-lookup"><span data-stu-id="f931e-110">boolean</span></span>|<span data-ttu-id="f931e-111">Указывает, выполняется ли сортировка по возрастанию.</span><span class="sxs-lookup"><span data-stu-id="f931e-111">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="f931e-112">color</span><span class="sxs-lookup"><span data-stu-id="f931e-112">color</span></span>|<span data-ttu-id="f931e-113">строка</span><span class="sxs-lookup"><span data-stu-id="f931e-113">string</span></span>|<span data-ttu-id="f931e-114">Представляет целевой цвет условия при сортировке по шрифту или цвету ячеек.</span><span class="sxs-lookup"><span data-stu-id="f931e-114">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="f931e-115">dataOption</span><span class="sxs-lookup"><span data-stu-id="f931e-115">dataOption</span></span>|<span data-ttu-id="f931e-116">string</span><span class="sxs-lookup"><span data-stu-id="f931e-116">string</span></span>|<span data-ttu-id="f931e-p101">Представляет дополнительные параметры сортировки для этого поля. Возможные значения: `Normal`, `TextAsNumber`.</span><span class="sxs-lookup"><span data-stu-id="f931e-p101">Represents additional sorting options for this field. Possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="f931e-119">key</span><span class="sxs-lookup"><span data-stu-id="f931e-119">key</span></span>|<span data-ttu-id="f931e-120">int</span><span class="sxs-lookup"><span data-stu-id="f931e-120">int</span></span>|<span data-ttu-id="f931e-p102">Представляет столбец (или строку в зависимости от ориентации сортировки), для которого задано условие. Представляется в виде расстояния от первого столбца (или строки).</span><span class="sxs-lookup"><span data-stu-id="f931e-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="f931e-123">sortOn</span><span class="sxs-lookup"><span data-stu-id="f931e-123">sortOn</span></span>|<span data-ttu-id="f931e-124">string</span><span class="sxs-lookup"><span data-stu-id="f931e-124">string</span></span>|<span data-ttu-id="f931e-p103">Представляет тип сортировки этого условия. Возможные значения: `Value`, `CellColor`, `FontColor`, `Icon`.</span><span class="sxs-lookup"><span data-stu-id="f931e-p103">Represents the type of sorting of this condition. Possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f931e-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="f931e-127">Relationships</span></span>
| <span data-ttu-id="f931e-128">Связь</span><span class="sxs-lookup"><span data-stu-id="f931e-128">Relationship</span></span> | <span data-ttu-id="f931e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="f931e-129">Type</span></span>   |<span data-ttu-id="f931e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="f931e-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f931e-131">icon</span><span class="sxs-lookup"><span data-stu-id="f931e-131">icon</span></span>|[<span data-ttu-id="f931e-132">Icon</span><span class="sxs-lookup"><span data-stu-id="f931e-132">Icon</span></span>](icon.md)|<span data-ttu-id="f931e-133">Представляет целевой значок условия при сортировке по значку ячейки.</span><span class="sxs-lookup"><span data-stu-id="f931e-133">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f931e-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f931e-134">JSON representation</span></span>

<span data-ttu-id="f931e-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f931e-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sortField"
}-->

```json
{
  "ascending": true,
  "color": "string",
  "dataOption": "string",
  "key": 1024,
  "sortOn": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "SortField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sortfield.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
