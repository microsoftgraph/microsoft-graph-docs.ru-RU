---
title: Тип ресурса plannerExternalReference
description: Ресурс **plannerExternalReference** представляет метаданные справочных материалов (такие вложения, как файл, URL-адрес). Это значение пар "свойство-значение" в объекте externalReferences.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 95084e8a4d2d1b117fc627902b2bd8163fcc82f6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518711"
---
# <a name="plannerexternalreference-resource-type"></a><span data-ttu-id="2cb2c-104">Тип ресурса plannerExternalReference</span><span class="sxs-lookup"><span data-stu-id="2cb2c-104">plannerExternalReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2cb2c-p102">Ресурс **plannerExternalReference** представляет метаданные справочных материалов (такие вложения, как файл, URL-адрес). Это значение пар "свойство-значение" в объекте [externalReferences](plannerexternalreferences.md).</span><span class="sxs-lookup"><span data-stu-id="2cb2c-p102">The **plannerExternalReference** resource represents the metadata of a reference (attachments such as file, URL). It is the value of property-value pairs in the [externalReferences object](plannerexternalreferences.md).</span></span>



## <a name="properties"></a><span data-ttu-id="2cb2c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2cb2c-107">Properties</span></span>
| <span data-ttu-id="2cb2c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2cb2c-108">Property</span></span>     | <span data-ttu-id="2cb2c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2cb2c-109">Type</span></span>   |<span data-ttu-id="2cb2c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2cb2c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2cb2c-111">alias</span><span class="sxs-lookup"><span data-stu-id="2cb2c-111">alias</span></span>|<span data-ttu-id="2cb2c-112">String</span><span class="sxs-lookup"><span data-stu-id="2cb2c-112">String</span></span>|<span data-ttu-id="2cb2c-113">Псевдоним имени для описания справочных материалов.</span><span class="sxs-lookup"><span data-stu-id="2cb2c-113">A name alias to describe the reference.</span></span>|
|<span data-ttu-id="2cb2c-114">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="2cb2c-114">lastModifiedBy</span></span>|[<span data-ttu-id="2cb2c-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="2cb2c-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="2cb2c-p103">Только для чтения. Идентификатор автора последних изменений.</span><span class="sxs-lookup"><span data-stu-id="2cb2c-p103">Read-only. User ID by which this is last modified.</span></span>|
|<span data-ttu-id="2cb2c-118">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2cb2c-118">lastModifiedDateTime</span></span>|<span data-ttu-id="2cb2c-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2cb2c-119">DateTimeOffset</span></span>|<span data-ttu-id="2cb2c-p104">Только для чтения. Дата и время последнего изменения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="2cb2c-p104">Read-only. Date and time at which this is last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="2cb2c-124">previewPriority</span><span class="sxs-lookup"><span data-stu-id="2cb2c-124">previewPriority</span></span>|<span data-ttu-id="2cb2c-125">String</span><span class="sxs-lookup"><span data-stu-id="2cb2c-125">String</span></span>|<span data-ttu-id="2cb2c-126">Позволяет задать порядок относительного приоритета, согласно которому справочные материалы будут отображаться при предварительном просмотре для задачи.</span><span class="sxs-lookup"><span data-stu-id="2cb2c-126">Used to set the relative priority order in which the reference will be shown as a preview on the task.</span></span>|
|<span data-ttu-id="2cb2c-127">type</span><span class="sxs-lookup"><span data-stu-id="2cb2c-127">type</span></span>|<span data-ttu-id="2cb2c-128">String</span><span class="sxs-lookup"><span data-stu-id="2cb2c-128">String</span></span>|<span data-ttu-id="2cb2c-p105">Используется для описания типа справочных материалов. Типы: `PowerPoint`, `Word`, `Excel`, `Other`.</span><span class="sxs-lookup"><span data-stu-id="2cb2c-p105">Used to describe the type of the reference. Types include: `PowerPoint`, `Word`, `Excel`, `Other`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2cb2c-131">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2cb2c-131">JSON representation</span></span>
<span data-ttu-id="2cb2c-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2cb2c-132">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerexternalreference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
