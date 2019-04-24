---
title: Тип ресурса Планнерчекклиститем
description: Ресурс **планнерчекклиститем** представляет элемент в контрольном списке задачи. Контрольный список для задачи представлен объектом Чекклиститемс.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 554391577fb0d48c2e0fd9fe265298e1dc1dd4fb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462482"
---
# <a name="plannerchecklistitem-resource-type"></a><span data-ttu-id="c1e9b-104">Тип ресурса Планнерчекклиститем</span><span class="sxs-lookup"><span data-stu-id="c1e9b-104">plannerChecklistItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1e9b-105">Ресурс **планнерчекклиститем** представляет элемент в контрольном списке задачи.</span><span class="sxs-lookup"><span data-stu-id="c1e9b-105">The **plannerChecklistItem** resource represents an item in the checklist of a task.</span></span> <span data-ttu-id="c1e9b-106">Контрольный список для задачи представлен [объектом чекклиститемс](plannerchecklistitems.md).</span><span class="sxs-lookup"><span data-stu-id="c1e9b-106">The checklist on a task is represented by the [checklistItems object](plannerchecklistitems.md).</span></span>


## <a name="properties"></a><span data-ttu-id="c1e9b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c1e9b-107">Properties</span></span>
| <span data-ttu-id="c1e9b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1e9b-108">Property</span></span>     | <span data-ttu-id="c1e9b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c1e9b-109">Type</span></span>   |<span data-ttu-id="c1e9b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c1e9b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1e9b-111">с возвратом</span><span class="sxs-lookup"><span data-stu-id="c1e9b-111">isChecked</span></span>|<span data-ttu-id="c1e9b-112">Логический</span><span class="sxs-lookup"><span data-stu-id="c1e9b-112">Boolean</span></span>|<span data-ttu-id="c1e9b-113">Значение, `true` если элемент отмечен флажком и `false` в противном случае.</span><span class="sxs-lookup"><span data-stu-id="c1e9b-113">Value is `true` if the item is checked and `false` otherwise.</span></span>|
|<span data-ttu-id="c1e9b-114">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="c1e9b-114">lastModifiedBy</span></span>|[<span data-ttu-id="c1e9b-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="c1e9b-115">identitySet</span></span>](identityset.md)| <span data-ttu-id="c1e9b-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c1e9b-116">Read-only.</span></span> <span data-ttu-id="c1e9b-117">Идентификатор пользователя, на который последний раз изменился.</span><span class="sxs-lookup"><span data-stu-id="c1e9b-117">User ID by which this is last modified.</span></span>|
|<span data-ttu-id="c1e9b-118">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1e9b-118">lastModifiedDateTime</span></span>|<span data-ttu-id="c1e9b-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1e9b-119">DateTimeOffset</span></span>|<span data-ttu-id="c1e9b-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c1e9b-120">Read-only.</span></span> <span data-ttu-id="c1e9b-121">Дата и время последнего изменения.</span><span class="sxs-lookup"><span data-stu-id="c1e9b-121">Date and time at which this is last modified.</span></span> <span data-ttu-id="c1e9b-122">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="c1e9b-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c1e9b-123">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c1e9b-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c1e9b-124">orderHint</span><span class="sxs-lookup"><span data-stu-id="c1e9b-124">orderHint</span></span>|<span data-ttu-id="c1e9b-125">String</span><span class="sxs-lookup"><span data-stu-id="c1e9b-125">String</span></span>|<span data-ttu-id="c1e9b-126">Используется для задания относительного порядка элементов в контрольном списке.</span><span class="sxs-lookup"><span data-stu-id="c1e9b-126">Used to set the relative order of items in the checklist.</span></span> <span data-ttu-id="c1e9b-127">Формат определяется, как описано [ниже](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="c1e9b-127">The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="c1e9b-128">title</span><span class="sxs-lookup"><span data-stu-id="c1e9b-128">title</span></span>|<span data-ttu-id="c1e9b-129">Строка</span><span class="sxs-lookup"><span data-stu-id="c1e9b-129">String</span></span>|<span data-ttu-id="c1e9b-130">Название элемента контрольного списка</span><span class="sxs-lookup"><span data-stu-id="c1e9b-130">Title of the checklist item</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c1e9b-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c1e9b-131">JSON representation</span></span>
<span data-ttu-id="c1e9b-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1e9b-132">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerchecklistitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
