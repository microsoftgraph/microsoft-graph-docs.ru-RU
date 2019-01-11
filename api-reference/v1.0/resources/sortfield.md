---
title: Тип ресурса SortField
description: Представляет условие в операции сортировки.
localization_priority: Normal
ms.openlocfilehash: 2c1b9a272fd024455d1297c5f59ca7684283e1a1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825972"
---
# <a name="sortfield-resource-type"></a><span data-ttu-id="7aee7-103">Тип ресурса SortField</span><span class="sxs-lookup"><span data-stu-id="7aee7-103">SortField resource type</span></span>

<span data-ttu-id="7aee7-104">Представляет условие в операции сортировки.</span><span class="sxs-lookup"><span data-stu-id="7aee7-104">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="7aee7-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="7aee7-105">Properties</span></span>
| <span data-ttu-id="7aee7-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="7aee7-106">Property</span></span>     | <span data-ttu-id="7aee7-107">Тип</span><span class="sxs-lookup"><span data-stu-id="7aee7-107">Type</span></span>   |<span data-ttu-id="7aee7-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7aee7-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7aee7-109">ascending</span><span class="sxs-lookup"><span data-stu-id="7aee7-109">ascending</span></span>|<span data-ttu-id="7aee7-110">boolean</span><span class="sxs-lookup"><span data-stu-id="7aee7-110">boolean</span></span>|<span data-ttu-id="7aee7-111">Указывает, выполняется ли сортировка по возрастанию.</span><span class="sxs-lookup"><span data-stu-id="7aee7-111">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="7aee7-112">color</span><span class="sxs-lookup"><span data-stu-id="7aee7-112">color</span></span>|<span data-ttu-id="7aee7-113">строка</span><span class="sxs-lookup"><span data-stu-id="7aee7-113">string</span></span>|<span data-ttu-id="7aee7-114">Представляет целевой цвет условия при сортировке по шрифту или цвету ячеек.</span><span class="sxs-lookup"><span data-stu-id="7aee7-114">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="7aee7-115">dataOption</span><span class="sxs-lookup"><span data-stu-id="7aee7-115">dataOption</span></span>|<span data-ttu-id="7aee7-116">string</span><span class="sxs-lookup"><span data-stu-id="7aee7-116">string</span></span>|<span data-ttu-id="7aee7-117">Представляет Дополнительные параметры сортировки для этого поля.</span><span class="sxs-lookup"><span data-stu-id="7aee7-117">Represents additional sorting options for this field.</span></span> <span data-ttu-id="7aee7-118">Возможные значения: `Normal`, `TextAsNumber`.</span><span class="sxs-lookup"><span data-stu-id="7aee7-118">The possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="7aee7-119">key</span><span class="sxs-lookup"><span data-stu-id="7aee7-119">key</span></span>|<span data-ttu-id="7aee7-120">int</span><span class="sxs-lookup"><span data-stu-id="7aee7-120">int</span></span>|<span data-ttu-id="7aee7-p102">Представляет столбец (или строку в зависимости от ориентации сортировки), для которого задано условие. Представляется в виде расстояния от первого столбца (или строки).</span><span class="sxs-lookup"><span data-stu-id="7aee7-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="7aee7-123">sortOn</span><span class="sxs-lookup"><span data-stu-id="7aee7-123">sortOn</span></span>|<span data-ttu-id="7aee7-124">строка</span><span class="sxs-lookup"><span data-stu-id="7aee7-124">string</span></span>|<span data-ttu-id="7aee7-125">Представляет тип сортировки этого условия.</span><span class="sxs-lookup"><span data-stu-id="7aee7-125">Represents the type of sorting of this condition.</span></span> <span data-ttu-id="7aee7-126">Возможные значения: `Value`, `CellColor`, `FontColor`, `Icon`.</span><span class="sxs-lookup"><span data-stu-id="7aee7-126">The possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|
|<span data-ttu-id="7aee7-127">icon</span><span class="sxs-lookup"><span data-stu-id="7aee7-127">icon</span></span>|[<span data-ttu-id="7aee7-128">WorkbookIcon</span><span class="sxs-lookup"><span data-stu-id="7aee7-128">WorkbookIcon</span></span>](icon.md)|<span data-ttu-id="7aee7-129">Представляет целевой значок условия при сортировке по значку ячейки.</span><span class="sxs-lookup"><span data-stu-id="7aee7-129">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7aee7-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7aee7-130">JSON representation</span></span>

<span data-ttu-id="7aee7-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7aee7-131">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookSortField"
}-->

```json
{
  "ascending": true,
  "color": "string",
  "dataOption": "string",
  "key": 1024,
  "sortOn": "string",
  "icon": { "@odata.type": "microsoft.graph.workbookIcon" }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "SortField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
