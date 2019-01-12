---
title: Тип ресурса plannerChecklistItem
description: Ресурс **plannerChecklistItem** представляет элемент в контрольном списке задачи. Контрольный список для задачи представлен объектом пункты памятки.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: fef935dfc2683e04b0ccec9ab5a7885927f8a13c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962984"
---
# <a name="plannerchecklistitem-resource-type"></a><span data-ttu-id="b214f-104">Тип ресурса plannerChecklistItem</span><span class="sxs-lookup"><span data-stu-id="b214f-104">plannerChecklistItem resource type</span></span>

> <span data-ttu-id="b214f-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b214f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b214f-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b214f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b214f-p103">Ресурс **plannerChecklistItem** представляет элемент в контрольном списке задачи. Контрольный список задачи представлен [объектом checklistItems](plannerchecklistitems.md).</span><span class="sxs-lookup"><span data-stu-id="b214f-p103">The **plannerChecklistItem** resource represents an item in the checklist of a task. The checklist on a task is represented by the [checklistItems object](plannerchecklistitems.md).</span></span>


## <a name="properties"></a><span data-ttu-id="b214f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="b214f-109">Properties</span></span>
| <span data-ttu-id="b214f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="b214f-110">Property</span></span>     | <span data-ttu-id="b214f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="b214f-111">Type</span></span>   |<span data-ttu-id="b214f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b214f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b214f-113">isChecked</span><span class="sxs-lookup"><span data-stu-id="b214f-113">isChecked</span></span>|<span data-ttu-id="b214f-114">Логический</span><span class="sxs-lookup"><span data-stu-id="b214f-114">Boolean</span></span>|<span data-ttu-id="b214f-115">Значение — `true`, если элемент проверен, в противном случае — `false`.</span><span class="sxs-lookup"><span data-stu-id="b214f-115">Value is `true` if the item is checked and `false` otherwise.</span></span>|
|<span data-ttu-id="b214f-116">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="b214f-116">lastModifiedBy</span></span>|[<span data-ttu-id="b214f-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="b214f-117">identitySet</span></span>](identityset.md)| <span data-ttu-id="b214f-p104">Только для чтения. Идентификатор автора последних изменений.</span><span class="sxs-lookup"><span data-stu-id="b214f-p104">Read-only. User ID by which this is last modified.</span></span>|
|<span data-ttu-id="b214f-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b214f-120">lastModifiedDateTime</span></span>|<span data-ttu-id="b214f-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b214f-121">DateTimeOffset</span></span>|<span data-ttu-id="b214f-p105">Только для чтения. Дата и время последнего изменения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b214f-p105">Read-only. Date and time at which this is last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b214f-126">orderHint</span><span class="sxs-lookup"><span data-stu-id="b214f-126">orderHint</span></span>|<span data-ttu-id="b214f-127">Строка</span><span class="sxs-lookup"><span data-stu-id="b214f-127">String</span></span>|<span data-ttu-id="b214f-p106">Используется для указания относительного порядка элементов в списке. Используемый формат описан [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="b214f-p106">Used to set the relative order of items in the checklist. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="b214f-130">title</span><span class="sxs-lookup"><span data-stu-id="b214f-130">title</span></span>|<span data-ttu-id="b214f-131">Строка</span><span class="sxs-lookup"><span data-stu-id="b214f-131">String</span></span>|<span data-ttu-id="b214f-132">Название элемента списка</span><span class="sxs-lookup"><span data-stu-id="b214f-132">Title of the checklist item</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b214f-133">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b214f-133">JSON representation</span></span>
<span data-ttu-id="b214f-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b214f-134">Here is a JSON representation of the resource.</span></span>

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
