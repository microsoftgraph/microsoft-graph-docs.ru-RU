---
title: Тип ресурса SortField
description: Представляет условие в операции сортировки.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: debc1f860e2e24306d6261444a29e126037aa3ae
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806746"
---
# <a name="sortfield-resource-type"></a><span data-ttu-id="cb907-103">Тип ресурса SortField</span><span class="sxs-lookup"><span data-stu-id="cb907-103">SortField resource type</span></span>

<span data-ttu-id="cb907-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb907-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cb907-105">Представляет условие в операции сортировки.</span><span class="sxs-lookup"><span data-stu-id="cb907-105">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="cb907-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="cb907-106">Properties</span></span>
| <span data-ttu-id="cb907-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb907-107">Property</span></span>     | <span data-ttu-id="cb907-108">Тип</span><span class="sxs-lookup"><span data-stu-id="cb907-108">Type</span></span>   |<span data-ttu-id="cb907-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cb907-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cb907-110">ascending</span><span class="sxs-lookup"><span data-stu-id="cb907-110">ascending</span></span>|<span data-ttu-id="cb907-111">boolean</span><span class="sxs-lookup"><span data-stu-id="cb907-111">boolean</span></span>|<span data-ttu-id="cb907-112">Указывает, выполняется ли сортировка по возрастанию.</span><span class="sxs-lookup"><span data-stu-id="cb907-112">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="cb907-113">color</span><span class="sxs-lookup"><span data-stu-id="cb907-113">color</span></span>|<span data-ttu-id="cb907-114">string</span><span class="sxs-lookup"><span data-stu-id="cb907-114">string</span></span>|<span data-ttu-id="cb907-115">Представляет целевой цвет условия при сортировке по шрифту или цвету ячеек.</span><span class="sxs-lookup"><span data-stu-id="cb907-115">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="cb907-116">dataOption</span><span class="sxs-lookup"><span data-stu-id="cb907-116">dataOption</span></span>|<span data-ttu-id="cb907-117">string</span><span class="sxs-lookup"><span data-stu-id="cb907-117">string</span></span>|<span data-ttu-id="cb907-118">Представляет дополнительные параметры сортировки для этого поля.</span><span class="sxs-lookup"><span data-stu-id="cb907-118">Represents additional sorting options for this field.</span></span> <span data-ttu-id="cb907-119">Возможные значения: `Normal` , `TextAsNumber` .</span><span class="sxs-lookup"><span data-stu-id="cb907-119">The possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="cb907-120">key</span><span class="sxs-lookup"><span data-stu-id="cb907-120">key</span></span>|<span data-ttu-id="cb907-121">int</span><span class="sxs-lookup"><span data-stu-id="cb907-121">int</span></span>|<span data-ttu-id="cb907-p102">Представляет столбец (или строку в зависимости от ориентации сортировки), для которого задано условие. Представляется в виде расстояния от первого столбца (или строки).</span><span class="sxs-lookup"><span data-stu-id="cb907-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="cb907-124">sortOn</span><span class="sxs-lookup"><span data-stu-id="cb907-124">sortOn</span></span>|<span data-ttu-id="cb907-125">string</span><span class="sxs-lookup"><span data-stu-id="cb907-125">string</span></span>|<span data-ttu-id="cb907-126">Представляет тип сортировки этого условия.</span><span class="sxs-lookup"><span data-stu-id="cb907-126">Represents the type of sorting of this condition.</span></span> <span data-ttu-id="cb907-127">Допустимые значения: `Value`, `CellColor`, `FontColor`, `Icon`.</span><span class="sxs-lookup"><span data-stu-id="cb907-127">The possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|
|<span data-ttu-id="cb907-128">значок</span><span class="sxs-lookup"><span data-stu-id="cb907-128">icon</span></span>|[<span data-ttu-id="cb907-129">воркбукикон</span><span class="sxs-lookup"><span data-stu-id="cb907-129">WorkbookIcon</span></span>](icon.md)|<span data-ttu-id="cb907-130">Представляет значок, определенный условием, при сортировке по значку ячейки.</span><span class="sxs-lookup"><span data-stu-id="cb907-130">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cb907-131">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="cb907-131">JSON representation</span></span>

<span data-ttu-id="cb907-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb907-132">Here is a JSON representation of the resource.</span></span>

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
