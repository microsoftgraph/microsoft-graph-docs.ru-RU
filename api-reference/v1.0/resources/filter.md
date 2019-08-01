---
title: Тип ресурса Filter
description: Управляет фильтрацией столбца таблицы.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3f58e1f5207fc3b4aebe2fdfb780735c0c5d209d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032482"
---
# <a name="filter-resource-type"></a><span data-ttu-id="b8000-103">Тип ресурса Filter</span><span class="sxs-lookup"><span data-stu-id="b8000-103">Filter resource type</span></span>

<span data-ttu-id="b8000-104">Управляет фильтрацией столбца таблицы.</span><span class="sxs-lookup"><span data-stu-id="b8000-104">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="b8000-105">Методы</span><span class="sxs-lookup"><span data-stu-id="b8000-105">Methods</span></span>

| <span data-ttu-id="b8000-106">Метод</span><span class="sxs-lookup"><span data-stu-id="b8000-106">Method</span></span>           | <span data-ttu-id="b8000-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b8000-107">Return Type</span></span>    |<span data-ttu-id="b8000-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b8000-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b8000-109">Apply</span><span class="sxs-lookup"><span data-stu-id="b8000-109">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="b8000-110">Нет</span><span class="sxs-lookup"><span data-stu-id="b8000-110">None</span></span>|<span data-ttu-id="b8000-111">Применяет заданные условия фильтра для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="b8000-111">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="b8000-112">Clear</span><span class="sxs-lookup"><span data-stu-id="b8000-112">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="b8000-113">Нет</span><span class="sxs-lookup"><span data-stu-id="b8000-113">None</span></span>|<span data-ttu-id="b8000-114">Сбрасывает фильтр для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="b8000-114">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="b8000-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="b8000-115">Properties</span></span>

| <span data-ttu-id="b8000-116">Имя</span><span class="sxs-lookup"><span data-stu-id="b8000-116">Name</span></span> | <span data-ttu-id="b8000-117">Тип</span><span class="sxs-lookup"><span data-stu-id="b8000-117">Type</span></span>   |<span data-ttu-id="b8000-118">Описание</span><span class="sxs-lookup"><span data-stu-id="b8000-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8000-119">criteria</span><span class="sxs-lookup"><span data-stu-id="b8000-119">criteria</span></span>|[<span data-ttu-id="b8000-120">Воркбукфилтеркритериа</span><span class="sxs-lookup"><span data-stu-id="b8000-120">WorkbookFilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="b8000-121">Текущий фильтр, заданный для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="b8000-121">The currently applied filter on the given column.</span></span> <span data-ttu-id="b8000-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8000-122">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b8000-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b8000-123">JSON representation</span></span>

<span data-ttu-id="b8000-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8000-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilter"
}-->

```json
{
  "criteria": {"@odata.type": "microsoft.graph.workbookFilterCriteria" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
