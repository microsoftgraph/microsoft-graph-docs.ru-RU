---
title: Тип ресурса Воркбукфилтер
description: Управляет фильтрацией столбца таблицы.
localization_priority: Normal
ms.openlocfilehash: 79ded0bfca0ace3b2d7c1bcdb4cd8dd2696802a4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33349002"
---
# <a name="workbookfilter-resource-type"></a><span data-ttu-id="f59f1-103">Тип ресурса Воркбукфилтер</span><span class="sxs-lookup"><span data-stu-id="f59f1-103">workbookFilter resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f59f1-104">Управляет фильтрацией столбца таблицы.</span><span class="sxs-lookup"><span data-stu-id="f59f1-104">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="f59f1-105">Методы</span><span class="sxs-lookup"><span data-stu-id="f59f1-105">Methods</span></span>

| <span data-ttu-id="f59f1-106">Метод</span><span class="sxs-lookup"><span data-stu-id="f59f1-106">Method</span></span>           | <span data-ttu-id="f59f1-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f59f1-107">Return Type</span></span>    |<span data-ttu-id="f59f1-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f59f1-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f59f1-109">Apply</span><span class="sxs-lookup"><span data-stu-id="f59f1-109">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="f59f1-110">Нет</span><span class="sxs-lookup"><span data-stu-id="f59f1-110">None</span></span>|<span data-ttu-id="f59f1-111">Применяет заданные условия фильтра для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="f59f1-111">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="f59f1-112">Clear</span><span class="sxs-lookup"><span data-stu-id="f59f1-112">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="f59f1-113">Нет</span><span class="sxs-lookup"><span data-stu-id="f59f1-113">None</span></span>|<span data-ttu-id="f59f1-114">Сбрасывает фильтр для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="f59f1-114">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="f59f1-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="f59f1-115">Properties</span></span>
<span data-ttu-id="f59f1-116">Нет</span><span class="sxs-lookup"><span data-stu-id="f59f1-116">None</span></span>

## <a name="relationships"></a><span data-ttu-id="f59f1-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="f59f1-117">Relationships</span></span>
| <span data-ttu-id="f59f1-118">Отношение</span><span class="sxs-lookup"><span data-stu-id="f59f1-118">Relationship</span></span> | <span data-ttu-id="f59f1-119">Тип</span><span class="sxs-lookup"><span data-stu-id="f59f1-119">Type</span></span>   |<span data-ttu-id="f59f1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f59f1-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f59f1-121">criteria</span><span class="sxs-lookup"><span data-stu-id="f59f1-121">criteria</span></span>|[<span data-ttu-id="f59f1-122">Воркбукфилтеркритериа</span><span class="sxs-lookup"><span data-stu-id="f59f1-122">workbookFilterCriteria</span></span>](workbookfiltercriteria.md)|<span data-ttu-id="f59f1-123">Текущий фильтр, заданный для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="f59f1-123">The currently applied filter on the given column.</span></span> <span data-ttu-id="f59f1-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f59f1-124">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f59f1-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f59f1-125">JSON representation</span></span>

<span data-ttu-id="f59f1-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f59f1-126">Here is a JSON representation of the resource.</span></span>

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
