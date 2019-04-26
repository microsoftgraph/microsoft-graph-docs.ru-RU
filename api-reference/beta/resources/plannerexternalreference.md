---
title: Тип ресурса Планнерекстерналреференце
description: Ресурс **планнерекстерналреференце** представляет метаданные ссылки (например, файл, URL-адрес). Это значение пар "свойство-значение" в объекте Екстерналреференцес.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 6d2bce70afbeee3848f3055530daf732afe8a2b5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344825"
---
# <a name="plannerexternalreference-resource-type"></a><span data-ttu-id="c9785-104">Тип ресурса Планнерекстерналреференце</span><span class="sxs-lookup"><span data-stu-id="c9785-104">plannerExternalReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9785-105">Ресурс **планнерекстерналреференце** представляет метаданные ссылки (например, файл, URL-адрес).</span><span class="sxs-lookup"><span data-stu-id="c9785-105">The **plannerExternalReference** resource represents the metadata of a reference (attachments such as file, URL).</span></span> <span data-ttu-id="c9785-106">Это значение пар "свойство-значение" в [объекте екстерналреференцес](plannerexternalreferences.md).</span><span class="sxs-lookup"><span data-stu-id="c9785-106">It is the value of property-value pairs in the [externalReferences object](plannerexternalreferences.md).</span></span>



## <a name="properties"></a><span data-ttu-id="c9785-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c9785-107">Properties</span></span>
| <span data-ttu-id="c9785-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9785-108">Property</span></span>     | <span data-ttu-id="c9785-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c9785-109">Type</span></span>   |<span data-ttu-id="c9785-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c9785-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9785-111">alias</span><span class="sxs-lookup"><span data-stu-id="c9785-111">alias</span></span>|<span data-ttu-id="c9785-112">String</span><span class="sxs-lookup"><span data-stu-id="c9785-112">String</span></span>|<span data-ttu-id="c9785-113">Псевдоним имени для описания ссылки.</span><span class="sxs-lookup"><span data-stu-id="c9785-113">A name alias to describe the reference.</span></span>|
|<span data-ttu-id="c9785-114">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="c9785-114">lastModifiedBy</span></span>|[<span data-ttu-id="c9785-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="c9785-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="c9785-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c9785-116">Read-only.</span></span> <span data-ttu-id="c9785-117">Идентификатор пользователя, на который последний раз изменился.</span><span class="sxs-lookup"><span data-stu-id="c9785-117">User ID by which this is last modified.</span></span>|
|<span data-ttu-id="c9785-118">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9785-118">lastModifiedDateTime</span></span>|<span data-ttu-id="c9785-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9785-119">DateTimeOffset</span></span>|<span data-ttu-id="c9785-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c9785-120">Read-only.</span></span> <span data-ttu-id="c9785-121">Дата и время последнего изменения.</span><span class="sxs-lookup"><span data-stu-id="c9785-121">Date and time at which this is last modified.</span></span> <span data-ttu-id="c9785-122">Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="c9785-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c9785-123">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c9785-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c9785-124">Превиевприорити</span><span class="sxs-lookup"><span data-stu-id="c9785-124">previewPriority</span></span>|<span data-ttu-id="c9785-125">String</span><span class="sxs-lookup"><span data-stu-id="c9785-125">String</span></span>|<span data-ttu-id="c9785-126">Используется для задания относительного порядка приоритетов, в соответствии с которым ссылка будет отображаться в качестве предварительной версии для задачи.</span><span class="sxs-lookup"><span data-stu-id="c9785-126">Used to set the relative priority order in which the reference will be shown as a preview on the task.</span></span>|
|<span data-ttu-id="c9785-127">type</span><span class="sxs-lookup"><span data-stu-id="c9785-127">type</span></span>|<span data-ttu-id="c9785-128">String</span><span class="sxs-lookup"><span data-stu-id="c9785-128">String</span></span>|<span data-ttu-id="c9785-129">Используется для описания типа ссылки.</span><span class="sxs-lookup"><span data-stu-id="c9785-129">Used to describe the type of the reference.</span></span> <span data-ttu-id="c9785-130">Типы включают: `PowerPoint`, `Word`, `Excel`, `Other`.</span><span class="sxs-lookup"><span data-stu-id="c9785-130">Types include: `PowerPoint`, `Word`, `Excel`, `Other`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c9785-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c9785-131">JSON representation</span></span>
<span data-ttu-id="c9785-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c9785-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerExternalReference"
}-->

```json
{
  "alias": "String",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "previewPriority": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerExternalReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
