---
title: Тип ресурса SortField
description: Представляет условие в операции сортировки.
localization_priority: Normal
ms.openlocfilehash: 2c1b9a272fd024455d1297c5f59ca7684283e1a1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561301"
---
# <a name="sortfield-resource-type"></a><span data-ttu-id="c283a-103">Тип ресурса SortField</span><span class="sxs-lookup"><span data-stu-id="c283a-103">SortField resource type</span></span>

<span data-ttu-id="c283a-104">Представляет условие в операции сортировки.</span><span class="sxs-lookup"><span data-stu-id="c283a-104">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="c283a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c283a-105">Properties</span></span>
| <span data-ttu-id="c283a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c283a-106">Property</span></span>     | <span data-ttu-id="c283a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c283a-107">Type</span></span>   |<span data-ttu-id="c283a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c283a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c283a-109">ascending</span><span class="sxs-lookup"><span data-stu-id="c283a-109">ascending</span></span>|<span data-ttu-id="c283a-110">boolean</span><span class="sxs-lookup"><span data-stu-id="c283a-110">boolean</span></span>|<span data-ttu-id="c283a-111">Указывает, выполняется ли сортировка по возрастанию.</span><span class="sxs-lookup"><span data-stu-id="c283a-111">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="c283a-112">color</span><span class="sxs-lookup"><span data-stu-id="c283a-112">color</span></span>|<span data-ttu-id="c283a-113">строка</span><span class="sxs-lookup"><span data-stu-id="c283a-113">string</span></span>|<span data-ttu-id="c283a-114">Представляет целевой цвет условия при сортировке по шрифту или цвету ячеек.</span><span class="sxs-lookup"><span data-stu-id="c283a-114">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="c283a-115">dataOption</span><span class="sxs-lookup"><span data-stu-id="c283a-115">dataOption</span></span>|<span data-ttu-id="c283a-116">string</span><span class="sxs-lookup"><span data-stu-id="c283a-116">string</span></span>|<span data-ttu-id="c283a-117">Представляет дополнительные параметры сортировки для этого поля.</span><span class="sxs-lookup"><span data-stu-id="c283a-117">Represents additional sorting options for this field.</span></span> <span data-ttu-id="c283a-118">Возможные значения: `Normal`, `TextAsNumber`.</span><span class="sxs-lookup"><span data-stu-id="c283a-118">The possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="c283a-119">key</span><span class="sxs-lookup"><span data-stu-id="c283a-119">key</span></span>|<span data-ttu-id="c283a-120">int</span><span class="sxs-lookup"><span data-stu-id="c283a-120">int</span></span>|<span data-ttu-id="c283a-p102">Представляет столбец (или строку в зависимости от ориентации сортировки), для которого задано условие. Представляется в виде расстояния от первого столбца (или строки).</span><span class="sxs-lookup"><span data-stu-id="c283a-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="c283a-123">sortOn</span><span class="sxs-lookup"><span data-stu-id="c283a-123">sortOn</span></span>|<span data-ttu-id="c283a-124">string</span><span class="sxs-lookup"><span data-stu-id="c283a-124">string</span></span>|<span data-ttu-id="c283a-125">Представляет тип сортировки этого условия.</span><span class="sxs-lookup"><span data-stu-id="c283a-125">Represents the type of sorting of this condition.</span></span> <span data-ttu-id="c283a-126">`Value`Возможные значения: `CellColor`,, `FontColor`,. `Icon`</span><span class="sxs-lookup"><span data-stu-id="c283a-126">The possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|
|<span data-ttu-id="c283a-127">значок</span><span class="sxs-lookup"><span data-stu-id="c283a-127">icon</span></span>|[<span data-ttu-id="c283a-128">Воркбукикон</span><span class="sxs-lookup"><span data-stu-id="c283a-128">WorkbookIcon</span></span>](icon.md)|<span data-ttu-id="c283a-129">Представляет значок, определенный условием, при сортировке по значку ячейки.</span><span class="sxs-lookup"><span data-stu-id="c283a-129">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c283a-130">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c283a-130">JSON representation</span></span>

<span data-ttu-id="c283a-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c283a-131">Here is a JSON representation of the resource.</span></span>

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
