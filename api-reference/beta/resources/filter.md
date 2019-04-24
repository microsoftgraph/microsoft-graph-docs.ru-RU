---
title: Тип ресурса Filter
description: Управляет фильтрацией столбца таблицы.
localization_priority: Normal
ms.openlocfilehash: 6adc4e378b47bcb134a640e77bf54c32a35b3be2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506422"
---
# <a name="filter-resource-type"></a><span data-ttu-id="1cb63-103">Тип ресурса Filter</span><span class="sxs-lookup"><span data-stu-id="1cb63-103">Filter resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1cb63-104">Управляет фильтрацией столбца таблицы.</span><span class="sxs-lookup"><span data-stu-id="1cb63-104">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="1cb63-105">Методы</span><span class="sxs-lookup"><span data-stu-id="1cb63-105">Methods</span></span>

| <span data-ttu-id="1cb63-106">Метод</span><span class="sxs-lookup"><span data-stu-id="1cb63-106">Method</span></span>           | <span data-ttu-id="1cb63-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1cb63-107">Return Type</span></span>    |<span data-ttu-id="1cb63-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1cb63-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1cb63-109">Apply</span><span class="sxs-lookup"><span data-stu-id="1cb63-109">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="1cb63-110">Нет</span><span class="sxs-lookup"><span data-stu-id="1cb63-110">None</span></span>|<span data-ttu-id="1cb63-111">Применяет заданные условия фильтра для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="1cb63-111">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="1cb63-112">Clear</span><span class="sxs-lookup"><span data-stu-id="1cb63-112">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="1cb63-113">Нет</span><span class="sxs-lookup"><span data-stu-id="1cb63-113">None</span></span>|<span data-ttu-id="1cb63-114">Сбрасывает фильтр для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="1cb63-114">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="1cb63-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="1cb63-115">Properties</span></span>
<span data-ttu-id="1cb63-116">Отсутствует</span><span class="sxs-lookup"><span data-stu-id="1cb63-116">None</span></span>

## <a name="relationships"></a><span data-ttu-id="1cb63-117">Связи</span><span class="sxs-lookup"><span data-stu-id="1cb63-117">Relationships</span></span>
| <span data-ttu-id="1cb63-118">Отношение</span><span class="sxs-lookup"><span data-stu-id="1cb63-118">Relationship</span></span> | <span data-ttu-id="1cb63-119">Тип</span><span class="sxs-lookup"><span data-stu-id="1cb63-119">Type</span></span>   |<span data-ttu-id="1cb63-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1cb63-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1cb63-121">criteria</span><span class="sxs-lookup"><span data-stu-id="1cb63-121">criteria</span></span>|[<span data-ttu-id="1cb63-122">FilterCriteria</span><span class="sxs-lookup"><span data-stu-id="1cb63-122">FilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="1cb63-p101">Текущий фильтр, заданный для определенного столбца. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1cb63-p101">The currently applied filter on the given column. Read-only.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/filter.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
