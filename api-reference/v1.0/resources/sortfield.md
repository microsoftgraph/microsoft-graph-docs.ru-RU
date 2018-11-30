---
title: Тип ресурса SortField
description: Представляет условие в операции сортировки.
ms.openlocfilehash: b6fc87e03b63a3e1cc34beef61a7538a913a118a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027231"
---
# <a name="sortfield-resource-type"></a><span data-ttu-id="d42e2-103">Тип ресурса SortField</span><span class="sxs-lookup"><span data-stu-id="d42e2-103">SortField resource type</span></span>

<span data-ttu-id="d42e2-104">Представляет условие в операции сортировки.</span><span class="sxs-lookup"><span data-stu-id="d42e2-104">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="d42e2-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d42e2-105">Properties</span></span>
| <span data-ttu-id="d42e2-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d42e2-106">Property</span></span>     | <span data-ttu-id="d42e2-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d42e2-107">Type</span></span>   |<span data-ttu-id="d42e2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d42e2-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d42e2-109">ascending</span><span class="sxs-lookup"><span data-stu-id="d42e2-109">ascending</span></span>|<span data-ttu-id="d42e2-110">boolean</span><span class="sxs-lookup"><span data-stu-id="d42e2-110">boolean</span></span>|<span data-ttu-id="d42e2-111">Указывает, выполняется ли сортировка по возрастанию.</span><span class="sxs-lookup"><span data-stu-id="d42e2-111">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="d42e2-112">color</span><span class="sxs-lookup"><span data-stu-id="d42e2-112">color</span></span>|<span data-ttu-id="d42e2-113">строка</span><span class="sxs-lookup"><span data-stu-id="d42e2-113">string</span></span>|<span data-ttu-id="d42e2-114">Представляет целевой цвет условия при сортировке по шрифту или цвету ячеек.</span><span class="sxs-lookup"><span data-stu-id="d42e2-114">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="d42e2-115">dataOption</span><span class="sxs-lookup"><span data-stu-id="d42e2-115">dataOption</span></span>|<span data-ttu-id="d42e2-116">string</span><span class="sxs-lookup"><span data-stu-id="d42e2-116">string</span></span>|<span data-ttu-id="d42e2-117">Представляет Дополнительные параметры сортировки для этого поля.</span><span class="sxs-lookup"><span data-stu-id="d42e2-117">Represents additional sorting options for this field.</span></span> <span data-ttu-id="d42e2-118">Возможные значения: `Normal`, `TextAsNumber`.</span><span class="sxs-lookup"><span data-stu-id="d42e2-118">The possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="d42e2-119">key</span><span class="sxs-lookup"><span data-stu-id="d42e2-119">key</span></span>|<span data-ttu-id="d42e2-120">целое</span><span class="sxs-lookup"><span data-stu-id="d42e2-120">int</span></span>|<span data-ttu-id="d42e2-p102">Представляет столбец (или строку в зависимости от ориентации сортировки), для которого задано условие. Представляется в виде расстояния от первого столбца (или строки).</span><span class="sxs-lookup"><span data-stu-id="d42e2-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="d42e2-123">sortOn</span><span class="sxs-lookup"><span data-stu-id="d42e2-123">sortOn</span></span>|<span data-ttu-id="d42e2-124">строка</span><span class="sxs-lookup"><span data-stu-id="d42e2-124">string</span></span>|<span data-ttu-id="d42e2-125">Представляет тип сортировки этого условия.</span><span class="sxs-lookup"><span data-stu-id="d42e2-125">Represents the type of sorting of this condition.</span></span> <span data-ttu-id="d42e2-126">Возможные значения: `Value`, `CellColor`, `FontColor`, `Icon`.</span><span class="sxs-lookup"><span data-stu-id="d42e2-126">The possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|
|<span data-ttu-id="d42e2-127">icon</span><span class="sxs-lookup"><span data-stu-id="d42e2-127">icon</span></span>|[<span data-ttu-id="d42e2-128">WorkbookIcon</span><span class="sxs-lookup"><span data-stu-id="d42e2-128">WorkbookIcon</span></span>](icon.md)|<span data-ttu-id="d42e2-129">Представляет целевой значок условия при сортировке по значку ячейки.</span><span class="sxs-lookup"><span data-stu-id="d42e2-129">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d42e2-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d42e2-130">JSON representation</span></span>

<span data-ttu-id="d42e2-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d42e2-131">Here is a JSON representation of the resource.</span></span>

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