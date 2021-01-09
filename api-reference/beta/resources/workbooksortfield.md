---
title: Тип ресурса workbookSortField
description: Представляет условие в операции сортировки.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: ruoyingl
ms.openlocfilehash: a245591755542a0a9bcfefb3f220511bd1521118
ms.sourcegitcommit: de175a11806f9e9ba3c916384e897aee1cc7f75c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/09/2021
ms.locfileid: "49790673"
---
# <a name="workbooksortfield-resource-type"></a><span data-ttu-id="d7061-103">Тип ресурса workbookSortField</span><span class="sxs-lookup"><span data-stu-id="d7061-103">workbookSortField resource type</span></span>

<span data-ttu-id="d7061-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7061-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7061-105">Представляет условие в операции сортировки.</span><span class="sxs-lookup"><span data-stu-id="d7061-105">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="d7061-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d7061-106">Properties</span></span>
| <span data-ttu-id="d7061-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7061-107">Property</span></span>     | <span data-ttu-id="d7061-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d7061-108">Type</span></span>   |<span data-ttu-id="d7061-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d7061-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7061-110">ascending</span><span class="sxs-lookup"><span data-stu-id="d7061-110">ascending</span></span>|<span data-ttu-id="d7061-111">boolean</span><span class="sxs-lookup"><span data-stu-id="d7061-111">boolean</span></span>|<span data-ttu-id="d7061-112">Указывает, выполняется ли сортировка по возрастанию.</span><span class="sxs-lookup"><span data-stu-id="d7061-112">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="d7061-113">color</span><span class="sxs-lookup"><span data-stu-id="d7061-113">color</span></span>|<span data-ttu-id="d7061-114">string</span><span class="sxs-lookup"><span data-stu-id="d7061-114">string</span></span>|<span data-ttu-id="d7061-115">Представляет целевой цвет условия при сортировке по шрифту или цвету ячеек.</span><span class="sxs-lookup"><span data-stu-id="d7061-115">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="d7061-116">dataOption</span><span class="sxs-lookup"><span data-stu-id="d7061-116">dataOption</span></span>|<span data-ttu-id="d7061-117">string</span><span class="sxs-lookup"><span data-stu-id="d7061-117">string</span></span>|<span data-ttu-id="d7061-p101">Представляет дополнительные параметры сортировки для этого поля. Возможные значения: `Normal`, `TextAsNumber`.</span><span class="sxs-lookup"><span data-stu-id="d7061-p101">Represents additional sorting options for this field. Possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="d7061-120">значок</span><span class="sxs-lookup"><span data-stu-id="d7061-120">icon</span></span>|[<span data-ttu-id="d7061-121">workbookIcon</span><span class="sxs-lookup"><span data-stu-id="d7061-121">workbookIcon</span></span>](workbookicon.md)|<span data-ttu-id="d7061-122">Представляет значок, определенный условием, при сортировке по значку ячейки.</span><span class="sxs-lookup"><span data-stu-id="d7061-122">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|
|<span data-ttu-id="d7061-123">key</span><span class="sxs-lookup"><span data-stu-id="d7061-123">key</span></span>|<span data-ttu-id="d7061-124">int</span><span class="sxs-lookup"><span data-stu-id="d7061-124">int</span></span>|<span data-ttu-id="d7061-p102">Представляет столбец (или строку в зависимости от ориентации сортировки), для которого задано условие. Представляется в виде расстояния от первого столбца (или строки).</span><span class="sxs-lookup"><span data-stu-id="d7061-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="d7061-127">sortOn</span><span class="sxs-lookup"><span data-stu-id="d7061-127">sortOn</span></span>|<span data-ttu-id="d7061-128">string</span><span class="sxs-lookup"><span data-stu-id="d7061-128">string</span></span>|<span data-ttu-id="d7061-p103">Представляет тип сортировки этого условия. Возможные значения: `Value`, `CellColor`, `FontColor`, `Icon`.</span><span class="sxs-lookup"><span data-stu-id="d7061-p103">Represents the type of sorting of this condition. Possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d7061-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d7061-131">JSON representation</span></span>

<span data-ttu-id="d7061-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7061-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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


