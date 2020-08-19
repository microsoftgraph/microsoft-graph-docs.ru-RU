---
title: Тип ресурса Воркбукфилтер
description: Управляет фильтрацией столбца таблицы.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: ruoyingl
ms.openlocfilehash: 39ebe2f59e5741e4580ef5300400a0b7e480ffad
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808521"
---
# <a name="workbookfilter-resource-type"></a><span data-ttu-id="77f90-103">Тип ресурса Воркбукфилтер</span><span class="sxs-lookup"><span data-stu-id="77f90-103">workbookFilter resource type</span></span>

<span data-ttu-id="77f90-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77f90-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77f90-105">Управляет фильтрацией столбца таблицы.</span><span class="sxs-lookup"><span data-stu-id="77f90-105">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="77f90-106">Методы</span><span class="sxs-lookup"><span data-stu-id="77f90-106">Methods</span></span>

| <span data-ttu-id="77f90-107">Метод</span><span class="sxs-lookup"><span data-stu-id="77f90-107">Method</span></span>           | <span data-ttu-id="77f90-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="77f90-108">Return Type</span></span>    |<span data-ttu-id="77f90-109">Описание</span><span class="sxs-lookup"><span data-stu-id="77f90-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="77f90-110">Apply</span><span class="sxs-lookup"><span data-stu-id="77f90-110">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="77f90-111">Нет</span><span class="sxs-lookup"><span data-stu-id="77f90-111">None</span></span>|<span data-ttu-id="77f90-112">Применяет заданные условия фильтра для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="77f90-112">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="77f90-113">Clear</span><span class="sxs-lookup"><span data-stu-id="77f90-113">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="77f90-114">Нет</span><span class="sxs-lookup"><span data-stu-id="77f90-114">None</span></span>|<span data-ttu-id="77f90-115">Сбрасывает фильтр для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="77f90-115">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="77f90-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="77f90-116">Properties</span></span>
<span data-ttu-id="77f90-117">Нет</span><span class="sxs-lookup"><span data-stu-id="77f90-117">None</span></span>

## <a name="relationships"></a><span data-ttu-id="77f90-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="77f90-118">Relationships</span></span>
| <span data-ttu-id="77f90-119">Связь</span><span class="sxs-lookup"><span data-stu-id="77f90-119">Relationship</span></span> | <span data-ttu-id="77f90-120">Тип</span><span class="sxs-lookup"><span data-stu-id="77f90-120">Type</span></span>   |<span data-ttu-id="77f90-121">Описание</span><span class="sxs-lookup"><span data-stu-id="77f90-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77f90-122">criteria</span><span class="sxs-lookup"><span data-stu-id="77f90-122">criteria</span></span>|[<span data-ttu-id="77f90-123">воркбукфилтеркритериа</span><span class="sxs-lookup"><span data-stu-id="77f90-123">workbookFilterCriteria</span></span>](workbookfiltercriteria.md)|<span data-ttu-id="77f90-124">Текущий фильтр, заданный для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="77f90-124">The currently applied filter on the given column.</span></span> <span data-ttu-id="77f90-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="77f90-125">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="77f90-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="77f90-126">JSON representation</span></span>

<span data-ttu-id="77f90-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77f90-127">Here is a JSON representation of the resource.</span></span>

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
