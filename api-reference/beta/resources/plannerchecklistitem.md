---
title: тип ресурса plannerChecklistItem
description: Ресурс **plannerChecklistItem** представляет элемент в списке задач. Контрольный список задачи представлен объектом checklistItems.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 5702e7a8c34c9ca0b996f437a65409371e8f3c98
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721007"
---
# <a name="plannerchecklistitem-resource-type"></a><span data-ttu-id="a8a73-104">тип ресурса plannerChecklistItem</span><span class="sxs-lookup"><span data-stu-id="a8a73-104">plannerChecklistItem resource type</span></span>

<span data-ttu-id="a8a73-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8a73-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8a73-106">Ресурс **plannerChecklistItem** представляет элемент в списке задач.</span><span class="sxs-lookup"><span data-stu-id="a8a73-106">The **plannerChecklistItem** resource represents an item in the checklist of a task.</span></span> <span data-ttu-id="a8a73-107">Контрольный список задачи представлен [объектом checklistItems.](plannerchecklistitems.md)</span><span class="sxs-lookup"><span data-stu-id="a8a73-107">The checklist on a task is represented by the [checklistItems object](plannerchecklistitems.md).</span></span>


## <a name="properties"></a><span data-ttu-id="a8a73-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a8a73-108">Properties</span></span>
| <span data-ttu-id="a8a73-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8a73-109">Property</span></span>     | <span data-ttu-id="a8a73-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a8a73-110">Type</span></span>   |<span data-ttu-id="a8a73-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a8a73-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8a73-112">isChecked</span><span class="sxs-lookup"><span data-stu-id="a8a73-112">isChecked</span></span>|<span data-ttu-id="a8a73-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8a73-113">Boolean</span></span>|<span data-ttu-id="a8a73-114">Значение, `true` если элемент проверяется и в `false` противном случае.</span><span class="sxs-lookup"><span data-stu-id="a8a73-114">Value is `true` if the item is checked and `false` otherwise.</span></span>|
|<span data-ttu-id="a8a73-115">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="a8a73-115">lastModifiedBy</span></span>|[<span data-ttu-id="a8a73-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="a8a73-116">identitySet</span></span>](identityset.md)| <span data-ttu-id="a8a73-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a8a73-117">Read-only.</span></span> <span data-ttu-id="a8a73-118">Пользовательский ID, с помощью которого он был изменен в последний раз.</span><span class="sxs-lookup"><span data-stu-id="a8a73-118">User ID by which this is last modified.</span></span>|
|<span data-ttu-id="a8a73-119">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8a73-119">lastModifiedDateTime</span></span>|<span data-ttu-id="a8a73-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8a73-120">DateTimeOffset</span></span>|<span data-ttu-id="a8a73-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a8a73-121">Read-only.</span></span> <span data-ttu-id="a8a73-122">Дата и время последнего изменения.</span><span class="sxs-lookup"><span data-stu-id="a8a73-122">Date and time at which this is last modified.</span></span> <span data-ttu-id="a8a73-123">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="a8a73-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a8a73-124">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="a8a73-124">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="a8a73-125">orderHint</span><span class="sxs-lookup"><span data-stu-id="a8a73-125">orderHint</span></span>|<span data-ttu-id="a8a73-126">String</span><span class="sxs-lookup"><span data-stu-id="a8a73-126">String</span></span>|<span data-ttu-id="a8a73-127">Используется для набора относительного порядка элементов в списке.</span><span class="sxs-lookup"><span data-stu-id="a8a73-127">Used to set the relative order of items in the checklist.</span></span> <span data-ttu-id="a8a73-128">Формат определяется как описанный [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="a8a73-128">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="a8a73-129">title</span><span class="sxs-lookup"><span data-stu-id="a8a73-129">title</span></span>|<span data-ttu-id="a8a73-130">String</span><span class="sxs-lookup"><span data-stu-id="a8a73-130">String</span></span>|<span data-ttu-id="a8a73-131">Название элемента контрольного списка</span><span class="sxs-lookup"><span data-stu-id="a8a73-131">Title of the checklist item</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a8a73-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a8a73-132">JSON representation</span></span>
<span data-ttu-id="a8a73-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8a73-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerChecklistItem"
}-->

```json
{
  "isChecked": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "orderHint": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerChecklistItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


