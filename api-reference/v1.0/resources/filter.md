---
title: Тип ресурса Filter
description: Управляет фильтрацией столбца таблицы.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ecaa61bde452d13e7e8e7fe0c79e3b75eeaa591a
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807810"
---
# <a name="filter-resource-type"></a><span data-ttu-id="1d031-103">Тип ресурса Filter</span><span class="sxs-lookup"><span data-stu-id="1d031-103">Filter resource type</span></span>

<span data-ttu-id="1d031-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d031-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1d031-105">Управляет фильтрацией столбца таблицы.</span><span class="sxs-lookup"><span data-stu-id="1d031-105">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="1d031-106">Методы</span><span class="sxs-lookup"><span data-stu-id="1d031-106">Methods</span></span>

| <span data-ttu-id="1d031-107">Метод</span><span class="sxs-lookup"><span data-stu-id="1d031-107">Method</span></span>           | <span data-ttu-id="1d031-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1d031-108">Return Type</span></span>    |<span data-ttu-id="1d031-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1d031-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1d031-110">Apply</span><span class="sxs-lookup"><span data-stu-id="1d031-110">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="1d031-111">Нет</span><span class="sxs-lookup"><span data-stu-id="1d031-111">None</span></span>|<span data-ttu-id="1d031-112">Применяет заданные условия фильтра для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="1d031-112">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="1d031-113">Clear</span><span class="sxs-lookup"><span data-stu-id="1d031-113">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="1d031-114">Нет</span><span class="sxs-lookup"><span data-stu-id="1d031-114">None</span></span>|<span data-ttu-id="1d031-115">Сбрасывает фильтр для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="1d031-115">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="1d031-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="1d031-116">Properties</span></span>

| <span data-ttu-id="1d031-117">Имя</span><span class="sxs-lookup"><span data-stu-id="1d031-117">Name</span></span> | <span data-ttu-id="1d031-118">Тип</span><span class="sxs-lookup"><span data-stu-id="1d031-118">Type</span></span>   |<span data-ttu-id="1d031-119">Описание</span><span class="sxs-lookup"><span data-stu-id="1d031-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d031-120">criteria</span><span class="sxs-lookup"><span data-stu-id="1d031-120">criteria</span></span>|[<span data-ttu-id="1d031-121">воркбукфилтеркритериа</span><span class="sxs-lookup"><span data-stu-id="1d031-121">WorkbookFilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="1d031-122">Текущий фильтр, заданный для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="1d031-122">The currently applied filter on the given column.</span></span> <span data-ttu-id="1d031-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1d031-123">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1d031-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1d031-124">JSON representation</span></span>

<span data-ttu-id="1d031-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1d031-125">Here is a JSON representation of the resource.</span></span>

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
