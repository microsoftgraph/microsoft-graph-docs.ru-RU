---
title: Тип ресурса Filter
description: Управляет фильтрацией столбца таблицы.
ms.openlocfilehash: df896d10b1e8734015d38b92b5824e3e3652e3a6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079404"
---
# <a name="filter-resource-type"></a><span data-ttu-id="e80c0-103">Тип ресурса Filter</span><span class="sxs-lookup"><span data-stu-id="e80c0-103">Filter resource type</span></span>

> <span data-ttu-id="e80c0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e80c0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e80c0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e80c0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e80c0-106">Управляет фильтрацией столбца таблицы.</span><span class="sxs-lookup"><span data-stu-id="e80c0-106">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="e80c0-107">Методы</span><span class="sxs-lookup"><span data-stu-id="e80c0-107">Methods</span></span>

| <span data-ttu-id="e80c0-108">Метод</span><span class="sxs-lookup"><span data-stu-id="e80c0-108">Method</span></span>           | <span data-ttu-id="e80c0-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e80c0-109">Return Type</span></span>    |<span data-ttu-id="e80c0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e80c0-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e80c0-111">Apply</span><span class="sxs-lookup"><span data-stu-id="e80c0-111">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="e80c0-112">Нет</span><span class="sxs-lookup"><span data-stu-id="e80c0-112">None</span></span>|<span data-ttu-id="e80c0-113">Применяет заданные условия фильтра для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="e80c0-113">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="e80c0-114">Clear</span><span class="sxs-lookup"><span data-stu-id="e80c0-114">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="e80c0-115">Нет</span><span class="sxs-lookup"><span data-stu-id="e80c0-115">None</span></span>|<span data-ttu-id="e80c0-116">Сбрасывает фильтр для определенного столбца.</span><span class="sxs-lookup"><span data-stu-id="e80c0-116">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="e80c0-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="e80c0-117">Properties</span></span>
<span data-ttu-id="e80c0-118">Нет</span><span class="sxs-lookup"><span data-stu-id="e80c0-118">None</span></span>

## <a name="relationships"></a><span data-ttu-id="e80c0-119">Связи</span><span class="sxs-lookup"><span data-stu-id="e80c0-119">Relationships</span></span>
| <span data-ttu-id="e80c0-120">Связь</span><span class="sxs-lookup"><span data-stu-id="e80c0-120">Relationship</span></span> | <span data-ttu-id="e80c0-121">Тип</span><span class="sxs-lookup"><span data-stu-id="e80c0-121">Type</span></span>   |<span data-ttu-id="e80c0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e80c0-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e80c0-123">criteria</span><span class="sxs-lookup"><span data-stu-id="e80c0-123">criteria</span></span>|[<span data-ttu-id="e80c0-124">FilterCriteria</span><span class="sxs-lookup"><span data-stu-id="e80c0-124">FilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="e80c0-p102">Текущий фильтр, заданный для определенного столбца. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e80c0-p102">The currently applied filter on the given column. Read-only.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->