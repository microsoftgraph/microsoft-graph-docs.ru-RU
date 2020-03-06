---
title: Тип ресурса SortField
description: Представляет условие в операции сортировки.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1c1d5a83323c28b8ec54543d4ee633861654991e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533638"
---
# <a name="sortfield-resource-type"></a><span data-ttu-id="36403-103">Тип ресурса SortField</span><span class="sxs-lookup"><span data-stu-id="36403-103">SortField resource type</span></span>

<span data-ttu-id="36403-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36403-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="36403-105">Представляет условие в операции сортировки.</span><span class="sxs-lookup"><span data-stu-id="36403-105">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="36403-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="36403-106">Properties</span></span>
| <span data-ttu-id="36403-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="36403-107">Property</span></span>     | <span data-ttu-id="36403-108">Тип</span><span class="sxs-lookup"><span data-stu-id="36403-108">Type</span></span>   |<span data-ttu-id="36403-109">Описание</span><span class="sxs-lookup"><span data-stu-id="36403-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36403-110">ascending</span><span class="sxs-lookup"><span data-stu-id="36403-110">ascending</span></span>|<span data-ttu-id="36403-111">boolean</span><span class="sxs-lookup"><span data-stu-id="36403-111">boolean</span></span>|<span data-ttu-id="36403-112">Указывает, выполняется ли сортировка по возрастанию.</span><span class="sxs-lookup"><span data-stu-id="36403-112">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="36403-113">color</span><span class="sxs-lookup"><span data-stu-id="36403-113">color</span></span>|<span data-ttu-id="36403-114">строка</span><span class="sxs-lookup"><span data-stu-id="36403-114">string</span></span>|<span data-ttu-id="36403-115">Представляет целевой цвет условия при сортировке по шрифту или цвету ячеек.</span><span class="sxs-lookup"><span data-stu-id="36403-115">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="36403-116">dataOption</span><span class="sxs-lookup"><span data-stu-id="36403-116">dataOption</span></span>|<span data-ttu-id="36403-117">string</span><span class="sxs-lookup"><span data-stu-id="36403-117">string</span></span>|<span data-ttu-id="36403-118">Представляет дополнительные параметры сортировки для этого поля.</span><span class="sxs-lookup"><span data-stu-id="36403-118">Represents additional sorting options for this field.</span></span> <span data-ttu-id="36403-119">Возможные значения: `Normal`, `TextAsNumber`.</span><span class="sxs-lookup"><span data-stu-id="36403-119">The possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="36403-120">key</span><span class="sxs-lookup"><span data-stu-id="36403-120">key</span></span>|<span data-ttu-id="36403-121">int</span><span class="sxs-lookup"><span data-stu-id="36403-121">int</span></span>|<span data-ttu-id="36403-p102">Представляет столбец (или строку в зависимости от ориентации сортировки), для которого задано условие. Представляется в виде расстояния от первого столбца (или строки).</span><span class="sxs-lookup"><span data-stu-id="36403-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="36403-124">sortOn</span><span class="sxs-lookup"><span data-stu-id="36403-124">sortOn</span></span>|<span data-ttu-id="36403-125">string</span><span class="sxs-lookup"><span data-stu-id="36403-125">string</span></span>|<span data-ttu-id="36403-126">Представляет тип сортировки этого условия.</span><span class="sxs-lookup"><span data-stu-id="36403-126">Represents the type of sorting of this condition.</span></span> <span data-ttu-id="36403-127">Допустимые значения: `Value`, `CellColor`, `FontColor`, `Icon`.</span><span class="sxs-lookup"><span data-stu-id="36403-127">The possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|
|<span data-ttu-id="36403-128">значок</span><span class="sxs-lookup"><span data-stu-id="36403-128">icon</span></span>|[<span data-ttu-id="36403-129">воркбукикон</span><span class="sxs-lookup"><span data-stu-id="36403-129">WorkbookIcon</span></span>](icon.md)|<span data-ttu-id="36403-130">Представляет значок, определенный условием, при сортировке по значку ячейки.</span><span class="sxs-lookup"><span data-stu-id="36403-130">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="36403-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="36403-131">JSON representation</span></span>

<span data-ttu-id="36403-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36403-132">Here is a JSON representation of the resource.</span></span>

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
