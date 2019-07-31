---
title: Тип ресурса Планнерчекклиститем
description: Ресурс **планнерчекклиститем** представляет элемент в контрольном списке задачи. Контрольный список для задачи представлен объектом Чекклиститемс.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 9bce6b0089f9e713e66e0354ce58d68cfd17fa7c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009078"
---
# <a name="plannerchecklistitem-resource-type"></a><span data-ttu-id="c9385-104">Тип ресурса Планнерчекклиститем</span><span class="sxs-lookup"><span data-stu-id="c9385-104">plannerChecklistItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9385-105">Ресурс **планнерчекклиститем** представляет элемент в контрольном списке задачи.</span><span class="sxs-lookup"><span data-stu-id="c9385-105">The **plannerChecklistItem** resource represents an item in the checklist of a task.</span></span> <span data-ttu-id="c9385-106">Контрольный список для задачи представлен [объектом чекклиститемс](plannerchecklistitems.md).</span><span class="sxs-lookup"><span data-stu-id="c9385-106">The checklist on a task is represented by the [checklistItems object](plannerchecklistitems.md).</span></span>


## <a name="properties"></a><span data-ttu-id="c9385-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c9385-107">Properties</span></span>
| <span data-ttu-id="c9385-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9385-108">Property</span></span>     | <span data-ttu-id="c9385-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c9385-109">Type</span></span>   |<span data-ttu-id="c9385-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c9385-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9385-111">с возвратом</span><span class="sxs-lookup"><span data-stu-id="c9385-111">isChecked</span></span>|<span data-ttu-id="c9385-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9385-112">Boolean</span></span>|<span data-ttu-id="c9385-113">Значение, `true` если элемент отмечен флажком и `false` в противном случае.</span><span class="sxs-lookup"><span data-stu-id="c9385-113">Value is `true` if the item is checked and `false` otherwise.</span></span>|
|<span data-ttu-id="c9385-114">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="c9385-114">lastModifiedBy</span></span>|[<span data-ttu-id="c9385-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="c9385-115">identitySet</span></span>](identityset.md)| <span data-ttu-id="c9385-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c9385-116">Read-only.</span></span> <span data-ttu-id="c9385-117">Идентификатор пользователя, на который последний раз изменился.</span><span class="sxs-lookup"><span data-stu-id="c9385-117">User ID by which this is last modified.</span></span>|
|<span data-ttu-id="c9385-118">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9385-118">lastModifiedDateTime</span></span>|<span data-ttu-id="c9385-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9385-119">DateTimeOffset</span></span>|<span data-ttu-id="c9385-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c9385-120">Read-only.</span></span> <span data-ttu-id="c9385-121">Дата и время последнего изменения.</span><span class="sxs-lookup"><span data-stu-id="c9385-121">Date and time at which this is last modified.</span></span> <span data-ttu-id="c9385-122">Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="c9385-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c9385-123">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c9385-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c9385-124">orderHint</span><span class="sxs-lookup"><span data-stu-id="c9385-124">orderHint</span></span>|<span data-ttu-id="c9385-125">String</span><span class="sxs-lookup"><span data-stu-id="c9385-125">String</span></span>|<span data-ttu-id="c9385-126">Используется для задания относительного порядка элементов в контрольном списке.</span><span class="sxs-lookup"><span data-stu-id="c9385-126">Used to set the relative order of items in the checklist.</span></span> <span data-ttu-id="c9385-127">Формат определяется, как описано [ниже](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="c9385-127">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="c9385-128">title</span><span class="sxs-lookup"><span data-stu-id="c9385-128">title</span></span>|<span data-ttu-id="c9385-129">String</span><span class="sxs-lookup"><span data-stu-id="c9385-129">String</span></span>|<span data-ttu-id="c9385-130">Название элемента контрольного списка</span><span class="sxs-lookup"><span data-stu-id="c9385-130">Title of the checklist item</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c9385-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c9385-131">JSON representation</span></span>
<span data-ttu-id="c9385-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c9385-132">Here is a JSON representation of the resource.</span></span>

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
