---
title: Тип ресурса SortField
description: Представляет условие в операции сортировки.
localization_priority: Normal
ms.openlocfilehash: fc93f33f7e1c6f366986cd5d1ca82ea186ad44b9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894280"
---
# <a name="sortfield-resource-type"></a><span data-ttu-id="aa80c-103">Тип ресурса SortField</span><span class="sxs-lookup"><span data-stu-id="aa80c-103">SortField resource type</span></span>

> <span data-ttu-id="aa80c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="aa80c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa80c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa80c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aa80c-106">Представляет условие в операции сортировки.</span><span class="sxs-lookup"><span data-stu-id="aa80c-106">Represents a condition in a sorting operation.</span></span>

## <a name="properties"></a><span data-ttu-id="aa80c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="aa80c-107">Properties</span></span>
| <span data-ttu-id="aa80c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa80c-108">Property</span></span>     | <span data-ttu-id="aa80c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="aa80c-109">Type</span></span>   |<span data-ttu-id="aa80c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="aa80c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa80c-111">ascending</span><span class="sxs-lookup"><span data-stu-id="aa80c-111">ascending</span></span>|<span data-ttu-id="aa80c-112">boolean</span><span class="sxs-lookup"><span data-stu-id="aa80c-112">boolean</span></span>|<span data-ttu-id="aa80c-113">Указывает, выполняется ли сортировка по возрастанию.</span><span class="sxs-lookup"><span data-stu-id="aa80c-113">Represents whether the sorting is done in an ascending fashion.</span></span>|
|<span data-ttu-id="aa80c-114">color</span><span class="sxs-lookup"><span data-stu-id="aa80c-114">color</span></span>|<span data-ttu-id="aa80c-115">строка</span><span class="sxs-lookup"><span data-stu-id="aa80c-115">string</span></span>|<span data-ttu-id="aa80c-116">Представляет целевой цвет условия при сортировке по шрифту или цвету ячеек.</span><span class="sxs-lookup"><span data-stu-id="aa80c-116">Represents the color that is the target of the condition if the sorting is on font or cell color.</span></span>|
|<span data-ttu-id="aa80c-117">dataOption</span><span class="sxs-lookup"><span data-stu-id="aa80c-117">dataOption</span></span>|<span data-ttu-id="aa80c-118">string</span><span class="sxs-lookup"><span data-stu-id="aa80c-118">string</span></span>|<span data-ttu-id="aa80c-p102">Представляет дополнительные параметры сортировки для этого поля. Возможные значения: `Normal`, `TextAsNumber`.</span><span class="sxs-lookup"><span data-stu-id="aa80c-p102">Represents additional sorting options for this field. Possible values are: `Normal`, `TextAsNumber`.</span></span>|
|<span data-ttu-id="aa80c-121">key</span><span class="sxs-lookup"><span data-stu-id="aa80c-121">key</span></span>|<span data-ttu-id="aa80c-122">int</span><span class="sxs-lookup"><span data-stu-id="aa80c-122">int</span></span>|<span data-ttu-id="aa80c-p103">Представляет столбец (или строку в зависимости от ориентации сортировки), для которого задано условие. Представляется в виде расстояния от первого столбца (или строки).</span><span class="sxs-lookup"><span data-stu-id="aa80c-p103">Represents the column (or row, depending on the sort orientation) that the condition is on. Represented as an offset from the first column (or row).</span></span>|
|<span data-ttu-id="aa80c-125">sortOn</span><span class="sxs-lookup"><span data-stu-id="aa80c-125">sortOn</span></span>|<span data-ttu-id="aa80c-126">строка</span><span class="sxs-lookup"><span data-stu-id="aa80c-126">string</span></span>|<span data-ttu-id="aa80c-p104">Представляет тип сортировки этого условия. Возможные значения: `Value`, `CellColor`, `FontColor`, `Icon`.</span><span class="sxs-lookup"><span data-stu-id="aa80c-p104">Represents the type of sorting of this condition. Possible values are: `Value`, `CellColor`, `FontColor`, `Icon`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa80c-129">Связи</span><span class="sxs-lookup"><span data-stu-id="aa80c-129">Relationships</span></span>
| <span data-ttu-id="aa80c-130">Связь</span><span class="sxs-lookup"><span data-stu-id="aa80c-130">Relationship</span></span> | <span data-ttu-id="aa80c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="aa80c-131">Type</span></span>   |<span data-ttu-id="aa80c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="aa80c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa80c-133">icon</span><span class="sxs-lookup"><span data-stu-id="aa80c-133">icon</span></span>|[<span data-ttu-id="aa80c-134">Icon</span><span class="sxs-lookup"><span data-stu-id="aa80c-134">Icon</span></span>](icon.md)|<span data-ttu-id="aa80c-135">Представляет целевой значок условия при сортировке по значку ячейки.</span><span class="sxs-lookup"><span data-stu-id="aa80c-135">Represents the icon that is the target of the condition if the sorting is on the cell's icon.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aa80c-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aa80c-136">JSON representation</span></span>

<span data-ttu-id="aa80c-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa80c-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sortField"
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
<!-- {
  "type": "#page.annotation",
  "description": "SortField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
