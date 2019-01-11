---
title: Тип ресурса Filter
description: Управляет фильтрацией столбца таблицы.
localization_priority: Normal
ms.openlocfilehash: cc4b1b105c2049b36fa27cb88b41102366648fa8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834666"
---
# <a name="filter-resource-type"></a><span data-ttu-id="989f5-103">Тип ресурса Filter</span><span class="sxs-lookup"><span data-stu-id="989f5-103">Filter resource type</span></span>

<span data-ttu-id="989f5-104">Управляет фильтрацией столбца таблицы.</span><span class="sxs-lookup"><span data-stu-id="989f5-104">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="989f5-105">Методы</span><span class="sxs-lookup"><span data-stu-id="989f5-105">Methods</span></span>

| <span data-ttu-id="989f5-106">Метод</span><span class="sxs-lookup"><span data-stu-id="989f5-106">Method</span></span>           | <span data-ttu-id="989f5-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="989f5-107">Return Type</span></span>    |<span data-ttu-id="989f5-108">Описание</span><span class="sxs-lookup"><span data-stu-id="989f5-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="989f5-109">Apply</span><span class="sxs-lookup"><span data-stu-id="989f5-109">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="989f5-110">Нет</span><span class="sxs-lookup"><span data-stu-id="989f5-110">None</span></span>|<span data-ttu-id="989f5-111">Применяет заданные условия фильтра для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="989f5-111">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="989f5-112">Clear</span><span class="sxs-lookup"><span data-stu-id="989f5-112">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="989f5-113">Нет</span><span class="sxs-lookup"><span data-stu-id="989f5-113">None</span></span>|<span data-ttu-id="989f5-114">Сбрасывает фильтр для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="989f5-114">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="989f5-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="989f5-115">Properties</span></span>

| <span data-ttu-id="989f5-116">Имя</span><span class="sxs-lookup"><span data-stu-id="989f5-116">Name</span></span> | <span data-ttu-id="989f5-117">Тип</span><span class="sxs-lookup"><span data-stu-id="989f5-117">Type</span></span>   |<span data-ttu-id="989f5-118">Описание</span><span class="sxs-lookup"><span data-stu-id="989f5-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="989f5-119">criteria</span><span class="sxs-lookup"><span data-stu-id="989f5-119">criteria</span></span>|[<span data-ttu-id="989f5-120">WorkbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="989f5-120">WorkbookFilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="989f5-p101">Текущий фильтр, заданный для определенного столбца. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="989f5-p101">The currently applied filter on the given column. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="989f5-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="989f5-123">JSON representation</span></span>

<span data-ttu-id="989f5-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="989f5-124">Here is a JSON representation of the resource.</span></span>

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
