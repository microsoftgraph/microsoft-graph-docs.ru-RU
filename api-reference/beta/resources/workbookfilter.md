---
title: Тип ресурса Воркбукфилтер
description: Управляет фильтрацией столбца таблицы.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: ''
ms.openlocfilehash: 4a6255f522955e7e2041a8b9b2b23e39c5379ea1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519234"
---
# <a name="workbookfilter-resource-type"></a><span data-ttu-id="d930c-103">Тип ресурса Воркбукфилтер</span><span class="sxs-lookup"><span data-stu-id="d930c-103">workbookFilter resource type</span></span>

<span data-ttu-id="d930c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d930c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d930c-105">Управляет фильтрацией столбца таблицы.</span><span class="sxs-lookup"><span data-stu-id="d930c-105">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="d930c-106">Методы</span><span class="sxs-lookup"><span data-stu-id="d930c-106">Methods</span></span>

| <span data-ttu-id="d930c-107">Метод</span><span class="sxs-lookup"><span data-stu-id="d930c-107">Method</span></span>           | <span data-ttu-id="d930c-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d930c-108">Return Type</span></span>    |<span data-ttu-id="d930c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d930c-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d930c-110">Apply</span><span class="sxs-lookup"><span data-stu-id="d930c-110">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="d930c-111">Нет</span><span class="sxs-lookup"><span data-stu-id="d930c-111">None</span></span>|<span data-ttu-id="d930c-112">Применяет заданные условия фильтра для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="d930c-112">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="d930c-113">Clear</span><span class="sxs-lookup"><span data-stu-id="d930c-113">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="d930c-114">Нет</span><span class="sxs-lookup"><span data-stu-id="d930c-114">None</span></span>|<span data-ttu-id="d930c-115">Сбрасывает фильтр для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="d930c-115">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="d930c-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="d930c-116">Properties</span></span>
<span data-ttu-id="d930c-117">Нет</span><span class="sxs-lookup"><span data-stu-id="d930c-117">None</span></span>

## <a name="relationships"></a><span data-ttu-id="d930c-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="d930c-118">Relationships</span></span>
| <span data-ttu-id="d930c-119">Связь</span><span class="sxs-lookup"><span data-stu-id="d930c-119">Relationship</span></span> | <span data-ttu-id="d930c-120">Тип</span><span class="sxs-lookup"><span data-stu-id="d930c-120">Type</span></span>   |<span data-ttu-id="d930c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d930c-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d930c-122">criteria</span><span class="sxs-lookup"><span data-stu-id="d930c-122">criteria</span></span>|[<span data-ttu-id="d930c-123">воркбукфилтеркритериа</span><span class="sxs-lookup"><span data-stu-id="d930c-123">workbookFilterCriteria</span></span>](workbookfiltercriteria.md)|<span data-ttu-id="d930c-124">Текущий фильтр, заданный для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="d930c-124">The currently applied filter on the given column.</span></span> <span data-ttu-id="d930c-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d930c-125">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="d930c-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d930c-126">JSON representation</span></span>

<span data-ttu-id="d930c-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d930c-127">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
     "legacyId"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookFilter"
}-->

```json
{
    "criteria": {"@odata.type": "microsoft.graph.workbookFilterCriteria"}
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
