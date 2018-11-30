---
title: Тип ресурса plannerExternalReference
description: Ресурс **plannerExternalReference** представляет метаданные ссылки (вложениях, например файл, URL-адрес). Это значение пары значение свойства в объекте externalReferences.
ms.openlocfilehash: a9d53b487fd2ca6584af934c55388ee66b2071d2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024800"
---
# <a name="plannerexternalreference-resource-type"></a><span data-ttu-id="db486-104">Тип ресурса plannerExternalReference</span><span class="sxs-lookup"><span data-stu-id="db486-104">plannerExternalReference resource type</span></span>

<span data-ttu-id="db486-p102">Ресурс **plannerExternalReference** представляет метаданные справочных материалов (такие вложения, как файл, URL-адрес). Это значение пар "свойство-значение" в объекте [externalReferences](plannerexternalreferences.md).</span><span class="sxs-lookup"><span data-stu-id="db486-p102">The **plannerExternalReference** resource represents the metadata of a reference (attachments such as file, URL). It is the value of property-value pairs in the [externalReferences object](plannerexternalreferences.md).</span></span>



## <a name="properties"></a><span data-ttu-id="db486-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="db486-107">Properties</span></span>
| <span data-ttu-id="db486-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="db486-108">Property</span></span>     | <span data-ttu-id="db486-109">Тип</span><span class="sxs-lookup"><span data-stu-id="db486-109">Type</span></span>   |<span data-ttu-id="db486-110">Описание</span><span class="sxs-lookup"><span data-stu-id="db486-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db486-111">alias</span><span class="sxs-lookup"><span data-stu-id="db486-111">alias</span></span>|<span data-ttu-id="db486-112">String</span><span class="sxs-lookup"><span data-stu-id="db486-112">String</span></span>|<span data-ttu-id="db486-113">Псевдоним имени для описания справочных материалов.</span><span class="sxs-lookup"><span data-stu-id="db486-113">A name alias to describe the reference.</span></span>|
|<span data-ttu-id="db486-114">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="db486-114">lastModifiedBy</span></span>|[<span data-ttu-id="db486-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="db486-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="db486-p103">Только для чтения. Идентификатор автора последних изменений.</span><span class="sxs-lookup"><span data-stu-id="db486-p103">Read-only. User ID by which this is last modified.</span></span>|
|<span data-ttu-id="db486-118">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="db486-118">lastModifiedDateTime</span></span>|<span data-ttu-id="db486-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db486-119">DateTimeOffset</span></span>|<span data-ttu-id="db486-p104">Только для чтения. Дата и время последнего изменения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="db486-p104">Read-only. Date and time at which this is last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="db486-124">previewPriority</span><span class="sxs-lookup"><span data-stu-id="db486-124">previewPriority</span></span>|<span data-ttu-id="db486-125">String</span><span class="sxs-lookup"><span data-stu-id="db486-125">String</span></span>|<span data-ttu-id="db486-126">Позволяет задать порядок относительного приоритета, согласно которому справочные материалы будут отображаться при предварительном просмотре для задачи.</span><span class="sxs-lookup"><span data-stu-id="db486-126">Used to set the relative priority order in which the reference will be shown as a preview on the task.</span></span>|
|<span data-ttu-id="db486-127">type</span><span class="sxs-lookup"><span data-stu-id="db486-127">type</span></span>|<span data-ttu-id="db486-128">String</span><span class="sxs-lookup"><span data-stu-id="db486-128">String</span></span>|<span data-ttu-id="db486-p105">Используется для описания типа справочных материалов. Типы: `PowerPoint`, `Word`, `Excel`, `Other`.</span><span class="sxs-lookup"><span data-stu-id="db486-p105">Used to describe the type of the reference. Types include: `PowerPoint`, `Word`, `Excel`, `Other`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="db486-131">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="db486-131">JSON representation</span></span>
<span data-ttu-id="db486-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db486-132">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerExternalReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->