---
title: Тип ресурса plannerChecklistItem
description: Ресурс **plannerChecklistItem** представляет элемент в контрольном списке задачи. Контрольный список задачи представлен объектом checklistItems.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 87f7349e20245068a0a29a179ddb5505cd3be0ec
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522541"
---
# <a name="plannerchecklistitem-resource-type"></a><span data-ttu-id="08b50-104">Тип ресурса plannerChecklistItem</span><span class="sxs-lookup"><span data-stu-id="08b50-104">plannerChecklistItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08b50-p102">Ресурс **plannerChecklistItem** представляет элемент в контрольном списке задачи. Контрольный список задачи представлен [объектом checklistItems](plannerchecklistitems.md).</span><span class="sxs-lookup"><span data-stu-id="08b50-p102">The **plannerChecklistItem** resource represents an item in the checklist of a task. The checklist on a task is represented by the [checklistItems object](plannerchecklistitems.md).</span></span>


## <a name="properties"></a><span data-ttu-id="08b50-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="08b50-107">Properties</span></span>
| <span data-ttu-id="08b50-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="08b50-108">Property</span></span>     | <span data-ttu-id="08b50-109">Тип</span><span class="sxs-lookup"><span data-stu-id="08b50-109">Type</span></span>   |<span data-ttu-id="08b50-110">Описание</span><span class="sxs-lookup"><span data-stu-id="08b50-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08b50-111">isChecked</span><span class="sxs-lookup"><span data-stu-id="08b50-111">isChecked</span></span>|<span data-ttu-id="08b50-112">Логический</span><span class="sxs-lookup"><span data-stu-id="08b50-112">Boolean</span></span>|<span data-ttu-id="08b50-113">Значение — `true`, если элемент проверен, в противном случае — `false`.</span><span class="sxs-lookup"><span data-stu-id="08b50-113">Value is `true` if the item is checked and `false` otherwise.</span></span>|
|<span data-ttu-id="08b50-114">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="08b50-114">lastModifiedBy</span></span>|[<span data-ttu-id="08b50-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="08b50-115">identitySet</span></span>](identityset.md)| <span data-ttu-id="08b50-p103">Только для чтения. Идентификатор автора последних изменений.</span><span class="sxs-lookup"><span data-stu-id="08b50-p103">Read-only. User ID by which this is last modified.</span></span>|
|<span data-ttu-id="08b50-118">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="08b50-118">lastModifiedDateTime</span></span>|<span data-ttu-id="08b50-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08b50-119">DateTimeOffset</span></span>|<span data-ttu-id="08b50-p104">Только для чтения. Дата и время последнего изменения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="08b50-p104">Read-only. Date and time at which this is last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="08b50-124">orderHint</span><span class="sxs-lookup"><span data-stu-id="08b50-124">orderHint</span></span>|<span data-ttu-id="08b50-125">Строка</span><span class="sxs-lookup"><span data-stu-id="08b50-125">String</span></span>|<span data-ttu-id="08b50-p105">Используется для указания относительного порядка элементов в списке. Используемый формат описан [здесь](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="08b50-p105">Used to set the relative order of items in the checklist. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="08b50-128">title</span><span class="sxs-lookup"><span data-stu-id="08b50-128">title</span></span>|<span data-ttu-id="08b50-129">String</span><span class="sxs-lookup"><span data-stu-id="08b50-129">String</span></span>|<span data-ttu-id="08b50-130">Название элемента списка</span><span class="sxs-lookup"><span data-stu-id="08b50-130">Title of the checklist item</span></span>|

## <a name="json-representation"></a><span data-ttu-id="08b50-131">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="08b50-131">JSON representation</span></span>
<span data-ttu-id="08b50-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08b50-132">Here is a JSON representation of the resource.</span></span>

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
