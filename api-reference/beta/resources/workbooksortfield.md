---
title: Тип ресурса Воркбуксортфиелд
description: Представляет условие в операции сортировки.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: ruoyingl
ms.openlocfilehash: d5622a727ed084f7dc8e991dd76b166527988549
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807369"
---
# <a name="workbooksortfield-resource-type"></a><span data-ttu-id="40526-103">Тип ресурса Воркбуксортфиелд</span><span class="sxs-lookup"><span data-stu-id="40526-103">workbookSortField resource type</span></span>

<span data-ttu-id="40526-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40526-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40526-105">Представляет условие в операции сортировки.</span><span class="sxs-lookup"><span data-stu-id="40526-105">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="40526-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="40526-106">Properties</span></span>
| <span data-ttu-id="40526-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="40526-107">Property</span></span>     | <span data-ttu-id="40526-108">Тип</span><span class="sxs-lookup"><span data-stu-id="40526-108">Type</span></span>   |<span data-ttu-id="40526-109">Описание</span><span class="sxs-lookup"><span data-stu-id="40526-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40526-110">ascending</span><span class="sxs-lookup"><span data-stu-id="40526-110">ascending</span></span>|<span data-ttu-id="40526-111">boolean</span><span class="sxs-lookup"><span data-stu-id="40526-111">boolean</span></span>|<span data-ttu-id="40526-112">Указывает, выполняется ли сортировка по возрастанию.</span><span class="sxs-lookup"><span data-stu-id="40526-112">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="40526-113">color</span><span class="sxs-lookup"><span data-stu-id="40526-113">color</span></span>|<span data-ttu-id="40526-114">string</span><span class="sxs-lookup"><span data-stu-id="40526-114">string</span></span>|<span data-ttu-id="40526-115">Представляет целевой цвет условия при сортировке по шрифту или цвету ячеек.</span><span class="sxs-lookup"><span data-stu-id="40526-115">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="40526-116">dataOption</span><span class="sxs-lookup"><span data-stu-id="40526-116">dataOption</span></span>|<span data-ttu-id="40526-117">string</span><span class="sxs-lookup"><span data-stu-id="40526-117">string</span></span>|<span data-ttu-id="40526-p101">Представляет дополнительные параметры сортировки для этого поля. Возможные значения: `Normal`, `TextAsNumber`.</span><span class="sxs-lookup"><span data-stu-id="40526-p101">Represents additional sorting options for this field. Possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="40526-120">key</span><span class="sxs-lookup"><span data-stu-id="40526-120">key</span></span>|<span data-ttu-id="40526-121">int</span><span class="sxs-lookup"><span data-stu-id="40526-121">int</span></span>|<span data-ttu-id="40526-p102">Представляет столбец (или строку в зависимости от ориентации сортировки), для которого задано условие. Представляется в виде расстояния от первого столбца (или строки).</span><span class="sxs-lookup"><span data-stu-id="40526-p102">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="40526-124">sortOn</span><span class="sxs-lookup"><span data-stu-id="40526-124">sortOn</span></span>|<span data-ttu-id="40526-125">string</span><span class="sxs-lookup"><span data-stu-id="40526-125">string</span></span>|<span data-ttu-id="40526-p103">Представляет тип сортировки этого условия. Возможные значения: `Value`, `CellColor`, `FontColor`, `Icon`.</span><span class="sxs-lookup"><span data-stu-id="40526-p103">Represents the type of sorting of this condition. Possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="40526-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="40526-128">Relationships</span></span>
| <span data-ttu-id="40526-129">Связь</span><span class="sxs-lookup"><span data-stu-id="40526-129">Relationship</span></span> | <span data-ttu-id="40526-130">Тип</span><span class="sxs-lookup"><span data-stu-id="40526-130">Type</span></span>   |<span data-ttu-id="40526-131">Описание</span><span class="sxs-lookup"><span data-stu-id="40526-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40526-132">icon</span><span class="sxs-lookup"><span data-stu-id="40526-132">icon</span></span>|[<span data-ttu-id="40526-133">воркбукикон</span><span class="sxs-lookup"><span data-stu-id="40526-133">workbookIcon</span></span>](workbookicon.md)|<span data-ttu-id="40526-134">Представляет значок, определенный условием, при сортировке по значку ячейки.</span><span class="sxs-lookup"><span data-stu-id="40526-134">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="40526-135">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="40526-135">JSON representation</span></span>

<span data-ttu-id="40526-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40526-136">Here is a JSON representation of the resource.</span></span>

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
