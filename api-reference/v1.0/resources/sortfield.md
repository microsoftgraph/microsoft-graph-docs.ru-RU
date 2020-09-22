---
title: Тип ресурса SortField
description: Представляет условие в операции сортировки.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6bc2a983fe5b27759a0944975876c2c0a0b1ca41
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086411"
---
# <a name="sortfield-resource-type"></a><span data-ttu-id="11831-103">Тип ресурса SortField</span><span class="sxs-lookup"><span data-stu-id="11831-103">SortField resource type</span></span>

<span data-ttu-id="11831-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11831-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="11831-105">Представляет условие в операции сортировки.</span><span class="sxs-lookup"><span data-stu-id="11831-105">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="11831-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="11831-106">Properties</span></span>
| <span data-ttu-id="11831-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="11831-107">Property</span></span>     | <span data-ttu-id="11831-108">Тип</span><span class="sxs-lookup"><span data-stu-id="11831-108">Type</span></span>   |<span data-ttu-id="11831-109">Описание</span><span class="sxs-lookup"><span data-stu-id="11831-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11831-110">ascending</span><span class="sxs-lookup"><span data-stu-id="11831-110">ascending</span></span>|<span data-ttu-id="11831-111">boolean</span><span class="sxs-lookup"><span data-stu-id="11831-111">boolean</span></span>|<span data-ttu-id="11831-112">Указывает, выполняется ли сортировка по возрастанию.</span><span class="sxs-lookup"><span data-stu-id="11831-112">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="11831-113">color</span><span class="sxs-lookup"><span data-stu-id="11831-113">color</span></span>|<span data-ttu-id="11831-114">string</span><span class="sxs-lookup"><span data-stu-id="11831-114">string</span></span>|<span data-ttu-id="11831-115">Представляет целевой цвет условия при сортировке по шрифту или цвету ячеек.</span><span class="sxs-lookup"><span data-stu-id="11831-115">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="11831-116">dataOption</span><span class="sxs-lookup"><span data-stu-id="11831-116">dataOption</span></span>|<span data-ttu-id="11831-117">string</span><span class="sxs-lookup"><span data-stu-id="11831-117">string</span></span>|<span data-ttu-id="11831-118">Представляет дополнительные параметры сортировки для этого поля.</span><span class="sxs-lookup"><span data-stu-id="11831-118">Represents additional sorting options for this field.</span></span> <span data-ttu-id="11831-119">Возможные значения: `Normal` , `TextAsNumber` .</span><span class="sxs-lookup"><span data-stu-id="11831-119">The possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="11831-120">key</span><span class="sxs-lookup"><span data-stu-id="11831-120">key</span></span>|<span data-ttu-id="11831-121">int</span><span class="sxs-lookup"><span data-stu-id="11831-121">int</span></span>|<span data-ttu-id="11831-p102">Представляет столбец (или строку в зависимости от ориентации сортировки), для которого задано условие. Представляется в виде расстояния от первого столбца (или строки).</span><span class="sxs-lookup"><span data-stu-id="11831-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="11831-124">sortOn</span><span class="sxs-lookup"><span data-stu-id="11831-124">sortOn</span></span>|<span data-ttu-id="11831-125">string</span><span class="sxs-lookup"><span data-stu-id="11831-125">string</span></span>|<span data-ttu-id="11831-126">Представляет тип сортировки этого условия.</span><span class="sxs-lookup"><span data-stu-id="11831-126">Represents the type of sorting of this condition.</span></span> <span data-ttu-id="11831-127">Допустимые значения: `Value`, `CellColor`, `FontColor`, `Icon`.</span><span class="sxs-lookup"><span data-stu-id="11831-127">The possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|
|<span data-ttu-id="11831-128">значок</span><span class="sxs-lookup"><span data-stu-id="11831-128">icon</span></span>|[<span data-ttu-id="11831-129">воркбукикон</span><span class="sxs-lookup"><span data-stu-id="11831-129">WorkbookIcon</span></span>](icon.md)|<span data-ttu-id="11831-130">Представляет значок, определенный условием, при сортировке по значку ячейки.</span><span class="sxs-lookup"><span data-stu-id="11831-130">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11831-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="11831-131">JSON representation</span></span>

<span data-ttu-id="11831-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11831-132">Here is a JSON representation of the resource.</span></span>

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

