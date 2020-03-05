---
title: Тип ресурса Планнерчекклиститем
description: Ресурс **планнерчекклиститем** представляет элемент в контрольном списке задачи. Контрольный список для задачи представлен объектом Чекклиститемс.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 0ca5116b83d3d61fda27f1469573c9a9ab971522
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521771"
---
# <a name="plannerchecklistitem-resource-type"></a><span data-ttu-id="303cd-104">Тип ресурса Планнерчекклиститем</span><span class="sxs-lookup"><span data-stu-id="303cd-104">plannerChecklistItem resource type</span></span>

<span data-ttu-id="303cd-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="303cd-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="303cd-106">Ресурс **планнерчекклиститем** представляет элемент в контрольном списке задачи.</span><span class="sxs-lookup"><span data-stu-id="303cd-106">The **plannerChecklistItem** resource represents an item in the checklist of a task.</span></span> <span data-ttu-id="303cd-107">Контрольный список для задачи представлен [объектом чекклиститемс](plannerchecklistitems.md).</span><span class="sxs-lookup"><span data-stu-id="303cd-107">The checklist on a task is represented by the [checklistItems object](plannerchecklistitems.md).</span></span>


## <a name="properties"></a><span data-ttu-id="303cd-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="303cd-108">Properties</span></span>
| <span data-ttu-id="303cd-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="303cd-109">Property</span></span>     | <span data-ttu-id="303cd-110">Тип</span><span class="sxs-lookup"><span data-stu-id="303cd-110">Type</span></span>   |<span data-ttu-id="303cd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="303cd-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="303cd-112">с возвратом</span><span class="sxs-lookup"><span data-stu-id="303cd-112">isChecked</span></span>|<span data-ttu-id="303cd-113">Логический</span><span class="sxs-lookup"><span data-stu-id="303cd-113">Boolean</span></span>|<span data-ttu-id="303cd-114">Значение, `true` если элемент отмечен флажком и `false` в противном случае.</span><span class="sxs-lookup"><span data-stu-id="303cd-114">Value is `true` if the item is checked and `false` otherwise.</span></span>|
|<span data-ttu-id="303cd-115">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="303cd-115">lastModifiedBy</span></span>|[<span data-ttu-id="303cd-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="303cd-116">identitySet</span></span>](identityset.md)| <span data-ttu-id="303cd-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="303cd-117">Read-only.</span></span> <span data-ttu-id="303cd-118">Идентификатор пользователя, на который последний раз изменился.</span><span class="sxs-lookup"><span data-stu-id="303cd-118">User ID by which this is last modified.</span></span>|
|<span data-ttu-id="303cd-119">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="303cd-119">lastModifiedDateTime</span></span>|<span data-ttu-id="303cd-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="303cd-120">DateTimeOffset</span></span>|<span data-ttu-id="303cd-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="303cd-121">Read-only.</span></span> <span data-ttu-id="303cd-122">Дата и время последнего изменения.</span><span class="sxs-lookup"><span data-stu-id="303cd-122">Date and time at which this is last modified.</span></span> <span data-ttu-id="303cd-123">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="303cd-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="303cd-124">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="303cd-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="303cd-125">orderHint</span><span class="sxs-lookup"><span data-stu-id="303cd-125">orderHint</span></span>|<span data-ttu-id="303cd-126">String</span><span class="sxs-lookup"><span data-stu-id="303cd-126">String</span></span>|<span data-ttu-id="303cd-127">Используется для задания относительного порядка элементов в контрольном списке.</span><span class="sxs-lookup"><span data-stu-id="303cd-127">Used to set the relative order of items in the checklist.</span></span> <span data-ttu-id="303cd-128">Формат определяется, как описано [ниже](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="303cd-128">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="303cd-129">title</span><span class="sxs-lookup"><span data-stu-id="303cd-129">title</span></span>|<span data-ttu-id="303cd-130">String</span><span class="sxs-lookup"><span data-stu-id="303cd-130">String</span></span>|<span data-ttu-id="303cd-131">Название элемента контрольного списка</span><span class="sxs-lookup"><span data-stu-id="303cd-131">Title of the checklist item</span></span>|

## <a name="json-representation"></a><span data-ttu-id="303cd-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="303cd-132">JSON representation</span></span>
<span data-ttu-id="303cd-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="303cd-133">Here is a JSON representation of the resource.</span></span>

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
