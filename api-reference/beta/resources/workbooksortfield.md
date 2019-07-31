---
title: Тип ресурса Воркбуксортфиелд
description: Представляет условие в операции сортировки.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: ''
ms.openlocfilehash: 55a1f822e080f786b588837dd6d9120cea546d4b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963908"
---
# <a name="workbooksortfield-resource-type"></a><span data-ttu-id="13aff-103">Тип ресурса Воркбуксортфиелд</span><span class="sxs-lookup"><span data-stu-id="13aff-103">workbookSortField resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13aff-104">Представляет условие в операции сортировки.</span><span class="sxs-lookup"><span data-stu-id="13aff-104">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="13aff-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="13aff-105">Properties</span></span>
| <span data-ttu-id="13aff-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="13aff-106">Property</span></span>     | <span data-ttu-id="13aff-107">Тип</span><span class="sxs-lookup"><span data-stu-id="13aff-107">Type</span></span>   |<span data-ttu-id="13aff-108">Описание</span><span class="sxs-lookup"><span data-stu-id="13aff-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13aff-109">ascending</span><span class="sxs-lookup"><span data-stu-id="13aff-109">ascending</span></span>|<span data-ttu-id="13aff-110">boolean</span><span class="sxs-lookup"><span data-stu-id="13aff-110">boolean</span></span>|<span data-ttu-id="13aff-111">Указывает, выполняется ли сортировка по возрастанию.</span><span class="sxs-lookup"><span data-stu-id="13aff-111">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="13aff-112">color</span><span class="sxs-lookup"><span data-stu-id="13aff-112">color</span></span>|<span data-ttu-id="13aff-113">строка</span><span class="sxs-lookup"><span data-stu-id="13aff-113">string</span></span>|<span data-ttu-id="13aff-114">Представляет целевой цвет условия при сортировке по шрифту или цвету ячеек.</span><span class="sxs-lookup"><span data-stu-id="13aff-114">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="13aff-115">dataOption</span><span class="sxs-lookup"><span data-stu-id="13aff-115">dataOption</span></span>|<span data-ttu-id="13aff-116">string</span><span class="sxs-lookup"><span data-stu-id="13aff-116">string</span></span>|<span data-ttu-id="13aff-p101">Представляет дополнительные параметры сортировки для этого поля. Возможные значения: `Normal`, `TextAsNumber`.</span><span class="sxs-lookup"><span data-stu-id="13aff-p101">Represents additional sorting options for this field. Possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="13aff-119">key</span><span class="sxs-lookup"><span data-stu-id="13aff-119">key</span></span>|<span data-ttu-id="13aff-120">int</span><span class="sxs-lookup"><span data-stu-id="13aff-120">int</span></span>|<span data-ttu-id="13aff-p102">Представляет столбец (или строку в зависимости от ориентации сортировки), для которого задано условие. Представляется в виде расстояния от первого столбца (или строки).</span><span class="sxs-lookup"><span data-stu-id="13aff-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="13aff-123">sortOn</span><span class="sxs-lookup"><span data-stu-id="13aff-123">sortOn</span></span>|<span data-ttu-id="13aff-124">string</span><span class="sxs-lookup"><span data-stu-id="13aff-124">string</span></span>|<span data-ttu-id="13aff-p103">Представляет тип сортировки этого условия. Возможные значения: `Value`, `CellColor`, `FontColor`, `Icon`.</span><span class="sxs-lookup"><span data-stu-id="13aff-p103">Represents the type of sorting of this condition. Possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13aff-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="13aff-127">Relationships</span></span>
| <span data-ttu-id="13aff-128">Отношение</span><span class="sxs-lookup"><span data-stu-id="13aff-128">Relationship</span></span> | <span data-ttu-id="13aff-129">Тип</span><span class="sxs-lookup"><span data-stu-id="13aff-129">Type</span></span>   |<span data-ttu-id="13aff-130">Описание</span><span class="sxs-lookup"><span data-stu-id="13aff-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13aff-131">icon</span><span class="sxs-lookup"><span data-stu-id="13aff-131">icon</span></span>|[<span data-ttu-id="13aff-132">Воркбукикон</span><span class="sxs-lookup"><span data-stu-id="13aff-132">workbookIcon</span></span>](workbookicon.md)|<span data-ttu-id="13aff-133">Представляет значок, определенный условием, при сортировке по значку ячейки.</span><span class="sxs-lookup"><span data-stu-id="13aff-133">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13aff-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="13aff-134">JSON representation</span></span>

<span data-ttu-id="13aff-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13aff-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookSortField"
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
  "suppressions": []
}
-->
