---
title: Тип ресурса educationResource
description: Суперкласса для всех объектов ресурсов в системе. Ресурс связан с **назначения** и/или **отправки**, который представляет объект обучения, который
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 87b19f849e24f1780a1d13c7aa1b3eb83543fdec
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523220"
---
# <a name="educationresource-resource-type"></a><span data-ttu-id="1b012-104">Тип ресурса educationResource</span><span class="sxs-lookup"><span data-stu-id="1b012-104">educationResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b012-105">Суперкласса для всех объектов ресурсов в системе.</span><span class="sxs-lookup"><span data-stu-id="1b012-105">A superclass for all resource objects in the system.</span></span> <span data-ttu-id="1b012-106">Ресурс связан с **назначения** и/или **отправки**, который представляет объект обучения, который раздать или передачи.</span><span class="sxs-lookup"><span data-stu-id="1b012-106">A resource is associated with an **Assignment** and/or **Submission**, which represents the learning object that is being handed out or handed in.</span></span> <span data-ttu-id="1b012-107">Ресурс не могут создаваться напрямую; необходимо включить для подкласса, представляющий тип использования ресурсов.</span><span class="sxs-lookup"><span data-stu-id="1b012-107">You cannot instantiate a resource directly; you must make a subclass that will represent the type of resource being used.</span></span>

<span data-ttu-id="1b012-108">Этот ресурс сохраняет общие свойства для всех типов ресурсов.</span><span class="sxs-lookup"><span data-stu-id="1b012-108">This resource stores the common properties across all resource types.</span></span>


## <a name="properties"></a><span data-ttu-id="1b012-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="1b012-109">Properties</span></span>
| <span data-ttu-id="1b012-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b012-110">Property</span></span>     | <span data-ttu-id="1b012-111">Тип</span><span class="sxs-lookup"><span data-stu-id="1b012-111">Type</span></span>   |<span data-ttu-id="1b012-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1b012-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b012-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="1b012-113">createdBy</span></span>|[<span data-ttu-id="1b012-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="1b012-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="1b012-115">Создатель ресурса.</span><span class="sxs-lookup"><span data-stu-id="1b012-115">Who created the resource.</span></span>|
|<span data-ttu-id="1b012-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1b012-116">createdDateTime</span></span>|<span data-ttu-id="1b012-117">Момент времени, когда был создан ресурса.</span><span class="sxs-lookup"><span data-stu-id="1b012-117">Moment in time when the resource was created.</span></span>  <span data-ttu-id="1b012-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b012-118">DateTimeOffset</span></span>|<span data-ttu-id="1b012-p104">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="1b012-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="1b012-121">displayName</span><span class="sxs-lookup"><span data-stu-id="1b012-121">displayName</span></span>|<span data-ttu-id="1b012-122">String</span><span class="sxs-lookup"><span data-stu-id="1b012-122">String</span></span>|<span data-ttu-id="1b012-123">Отображаемое имя ресурса.</span><span class="sxs-lookup"><span data-stu-id="1b012-123">Display name of resource.</span></span>|
|<span data-ttu-id="1b012-124">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="1b012-124">lastModifiedBy</span></span>|[<span data-ttu-id="1b012-125">identitySet</span><span class="sxs-lookup"><span data-stu-id="1b012-125">identitySet</span></span>](identityset.md)|<span data-ttu-id="1b012-126">Кто был последний пользователям изменять ресурса.</span><span class="sxs-lookup"><span data-stu-id="1b012-126">Who was the last user to modify the resource.</span></span>|
|<span data-ttu-id="1b012-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b012-127">lastModifiedDateTime</span></span>|<span data-ttu-id="1b012-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b012-128">DateTimeOffset</span></span>|<span data-ttu-id="1b012-129">Момент времени, время последнего изменения ресурса.</span><span class="sxs-lookup"><span data-stu-id="1b012-129">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="1b012-130">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="1b012-130">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1b012-131">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="1b012-131">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1b012-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1b012-132">JSON representation</span></span>

<span data-ttu-id="1b012-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b012-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationResource"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
