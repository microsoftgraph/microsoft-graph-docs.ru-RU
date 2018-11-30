---
title: Тип ресурса plannerChecklistItem
description: Ресурс **plannerChecklistItem** представляет элемент в контрольном списке задачи. Контрольный список для задачи представлен объектом пункты памятки.
ms.openlocfilehash: 846c1877fb421c9070eff7c041983367a7beb29b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078096"
---
# <a name="plannerchecklistitem-resource-type"></a><span data-ttu-id="31f54-104">Тип ресурса plannerChecklistItem</span><span class="sxs-lookup"><span data-stu-id="31f54-104">plannerChecklistItem resource type</span></span>

> <span data-ttu-id="31f54-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="31f54-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31f54-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31f54-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="31f54-p103">Ресурс **plannerChecklistItem** представляет элемент в контрольном списке задачи. Контрольный список задачи представлен [объектом checklistItems](plannerchecklistitems.md).</span><span class="sxs-lookup"><span data-stu-id="31f54-p103">The **plannerChecklistItem** resource represents an item in the checklist of a task. The checklist on a task is represented by the [checklistItems object](plannerchecklistitems.md).</span></span>


## <a name="properties"></a><span data-ttu-id="31f54-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="31f54-109">Properties</span></span>
| <span data-ttu-id="31f54-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="31f54-110">Property</span></span>     | <span data-ttu-id="31f54-111">Тип</span><span class="sxs-lookup"><span data-stu-id="31f54-111">Type</span></span>   |<span data-ttu-id="31f54-112">Описание</span><span class="sxs-lookup"><span data-stu-id="31f54-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31f54-113">isChecked</span><span class="sxs-lookup"><span data-stu-id="31f54-113">isChecked</span></span>|<span data-ttu-id="31f54-114">Логический</span><span class="sxs-lookup"><span data-stu-id="31f54-114">Boolean</span></span>|<span data-ttu-id="31f54-115">Значение — `true`, если элемент проверен, в противном случае — `false`.</span><span class="sxs-lookup"><span data-stu-id="31f54-115">Value is `true` if the item is checked and `false` otherwise.</span></span>|
|<span data-ttu-id="31f54-116">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="31f54-116">lastModifiedBy</span></span>|[<span data-ttu-id="31f54-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="31f54-117">identitySet</span></span>](identityset.md)| <span data-ttu-id="31f54-p104">Только для чтения. Идентификатор автора последних изменений.</span><span class="sxs-lookup"><span data-stu-id="31f54-p104">Read-only. User ID by which this is last modified.</span></span>|
|<span data-ttu-id="31f54-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="31f54-120">lastModifiedDateTime</span></span>|<span data-ttu-id="31f54-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31f54-121">DateTimeOffset</span></span>|<span data-ttu-id="31f54-p105">Только для чтения. Дата и время последнего изменения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="31f54-p105">Read-only. Date and time at which this is last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="31f54-126">orderHint</span><span class="sxs-lookup"><span data-stu-id="31f54-126">orderHint</span></span>|<span data-ttu-id="31f54-127">Строка</span><span class="sxs-lookup"><span data-stu-id="31f54-127">String</span></span>|<span data-ttu-id="31f54-p106">Используется для указания относительного порядка элементов в списке. Используемый формат описан [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="31f54-p106">Used to set the relative order of items in the checklist. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="31f54-130">title</span><span class="sxs-lookup"><span data-stu-id="31f54-130">title</span></span>|<span data-ttu-id="31f54-131">Строка</span><span class="sxs-lookup"><span data-stu-id="31f54-131">String</span></span>|<span data-ttu-id="31f54-132">Название элемента списка</span><span class="sxs-lookup"><span data-stu-id="31f54-132">Title of the checklist item</span></span>|

## <a name="json-representation"></a><span data-ttu-id="31f54-133">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="31f54-133">JSON representation</span></span>
<span data-ttu-id="31f54-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31f54-134">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerChecklistItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->