---
title: Тип ресурса Filter
description: Управляет фильтрацией столбца таблицы.
ms.openlocfilehash: 272b4ea0ee91c25ea845217512a12e33b08ed7b8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026046"
---
# <a name="filter-resource-type"></a><span data-ttu-id="eb677-103">Тип ресурса Filter</span><span class="sxs-lookup"><span data-stu-id="eb677-103">Filter resource type</span></span>

<span data-ttu-id="eb677-104">Управляет фильтрацией столбца таблицы.</span><span class="sxs-lookup"><span data-stu-id="eb677-104">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="eb677-105">Методы</span><span class="sxs-lookup"><span data-stu-id="eb677-105">Methods</span></span>

| <span data-ttu-id="eb677-106">Метод</span><span class="sxs-lookup"><span data-stu-id="eb677-106">Method</span></span>           | <span data-ttu-id="eb677-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="eb677-107">Return Type</span></span>    |<span data-ttu-id="eb677-108">Описание</span><span class="sxs-lookup"><span data-stu-id="eb677-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="eb677-109">Apply</span><span class="sxs-lookup"><span data-stu-id="eb677-109">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="eb677-110">Нет</span><span class="sxs-lookup"><span data-stu-id="eb677-110">None</span></span>|<span data-ttu-id="eb677-111">Применяет заданные условия фильтра для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="eb677-111">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="eb677-112">Clear</span><span class="sxs-lookup"><span data-stu-id="eb677-112">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="eb677-113">Нет</span><span class="sxs-lookup"><span data-stu-id="eb677-113">None</span></span>|<span data-ttu-id="eb677-114">Сбрасывает фильтр для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="eb677-114">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="eb677-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="eb677-115">Properties</span></span>

| <span data-ttu-id="eb677-116">Имя</span><span class="sxs-lookup"><span data-stu-id="eb677-116">Name</span></span> | <span data-ttu-id="eb677-117">Тип</span><span class="sxs-lookup"><span data-stu-id="eb677-117">Type</span></span>   |<span data-ttu-id="eb677-118">Описание</span><span class="sxs-lookup"><span data-stu-id="eb677-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb677-119">criteria</span><span class="sxs-lookup"><span data-stu-id="eb677-119">criteria</span></span>|[<span data-ttu-id="eb677-120">WorkbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="eb677-120">WorkbookFilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="eb677-p101">Текущий фильтр, заданный для определенного столбца. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eb677-p101">The currently applied filter on the given column. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eb677-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eb677-123">JSON representation</span></span>

<span data-ttu-id="eb677-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb677-124">Here is a JSON representation of the resource.</span></span>

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