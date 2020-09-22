---
title: Тип ресурса Воркбуксортфиелд
description: Представляет условие в операции сортировки.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: ruoyingl
ms.openlocfilehash: 5f296d7d2d748213c24f1d49f6363f86d2b1af84
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046106"
---
# <a name="workbooksortfield-resource-type"></a><span data-ttu-id="d71dd-103">Тип ресурса Воркбуксортфиелд</span><span class="sxs-lookup"><span data-stu-id="d71dd-103">workbookSortField resource type</span></span>

<span data-ttu-id="d71dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d71dd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d71dd-105">Представляет условие в операции сортировки.</span><span class="sxs-lookup"><span data-stu-id="d71dd-105">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="d71dd-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d71dd-106">Properties</span></span>
| <span data-ttu-id="d71dd-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d71dd-107">Property</span></span>     | <span data-ttu-id="d71dd-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d71dd-108">Type</span></span>   |<span data-ttu-id="d71dd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d71dd-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d71dd-110">ascending</span><span class="sxs-lookup"><span data-stu-id="d71dd-110">ascending</span></span>|<span data-ttu-id="d71dd-111">boolean</span><span class="sxs-lookup"><span data-stu-id="d71dd-111">boolean</span></span>|<span data-ttu-id="d71dd-112">Указывает, выполняется ли сортировка по возрастанию.</span><span class="sxs-lookup"><span data-stu-id="d71dd-112">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="d71dd-113">color</span><span class="sxs-lookup"><span data-stu-id="d71dd-113">color</span></span>|<span data-ttu-id="d71dd-114">string</span><span class="sxs-lookup"><span data-stu-id="d71dd-114">string</span></span>|<span data-ttu-id="d71dd-115">Представляет целевой цвет условия при сортировке по шрифту или цвету ячеек.</span><span class="sxs-lookup"><span data-stu-id="d71dd-115">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="d71dd-116">dataOption</span><span class="sxs-lookup"><span data-stu-id="d71dd-116">dataOption</span></span>|<span data-ttu-id="d71dd-117">string</span><span class="sxs-lookup"><span data-stu-id="d71dd-117">string</span></span>|<span data-ttu-id="d71dd-p101">Представляет дополнительные параметры сортировки для этого поля. Возможные значения: `Normal`, `TextAsNumber`.</span><span class="sxs-lookup"><span data-stu-id="d71dd-p101">Represents additional sorting options for this field. Possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="d71dd-120">key</span><span class="sxs-lookup"><span data-stu-id="d71dd-120">key</span></span>|<span data-ttu-id="d71dd-121">int</span><span class="sxs-lookup"><span data-stu-id="d71dd-121">int</span></span>|<span data-ttu-id="d71dd-p102">Представляет столбец (или строку в зависимости от ориентации сортировки), для которого задано условие. Представляется в виде расстояния от первого столбца (или строки).</span><span class="sxs-lookup"><span data-stu-id="d71dd-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="d71dd-124">sortOn</span><span class="sxs-lookup"><span data-stu-id="d71dd-124">sortOn</span></span>|<span data-ttu-id="d71dd-125">string</span><span class="sxs-lookup"><span data-stu-id="d71dd-125">string</span></span>|<span data-ttu-id="d71dd-p103">Представляет тип сортировки этого условия. Возможные значения: `Value`, `CellColor`, `FontColor`, `Icon`.</span><span class="sxs-lookup"><span data-stu-id="d71dd-p103">Represents the type of sorting of this condition. Possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d71dd-128">Связи</span><span class="sxs-lookup"><span data-stu-id="d71dd-128">Relationships</span></span>
| <span data-ttu-id="d71dd-129">Связь</span><span class="sxs-lookup"><span data-stu-id="d71dd-129">Relationship</span></span> | <span data-ttu-id="d71dd-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d71dd-130">Type</span></span>   |<span data-ttu-id="d71dd-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d71dd-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d71dd-132">icon</span><span class="sxs-lookup"><span data-stu-id="d71dd-132">icon</span></span>|[<span data-ttu-id="d71dd-133">воркбукикон</span><span class="sxs-lookup"><span data-stu-id="d71dd-133">workbookIcon</span></span>](workbookicon.md)|<span data-ttu-id="d71dd-134">Представляет значок, определенный условием, при сортировке по значку ячейки.</span><span class="sxs-lookup"><span data-stu-id="d71dd-134">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d71dd-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d71dd-135">JSON representation</span></span>

<span data-ttu-id="d71dd-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d71dd-136">Here is a JSON representation of the resource.</span></span>

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


