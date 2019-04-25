---
title: Тип ресурса Едукатионресаурце
description: Суперкласс для всех объектов ресурсов в системе. Ресурс связан с наЗначением **** и/или отправкой, представляющим обучающий объект, который ****
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 87b19f849e24f1780a1d13c7aa1b3eb83543fdec
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542879"
---
# <a name="educationresource-resource-type"></a><span data-ttu-id="1ac3c-104">Тип ресурса Едукатионресаурце</span><span class="sxs-lookup"><span data-stu-id="1ac3c-104">educationResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ac3c-105">Суперкласс для всех объектов ресурсов в системе.</span><span class="sxs-lookup"><span data-stu-id="1ac3c-105">A superclass for all resource objects in the system.</span></span> <span data-ttu-id="1ac3c-106">Ресурс связан с наЗначением \*\*\*\* и/или отправкой, представляющим обучающий объект, который передается или передается. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="1ac3c-106">A resource is associated with an **Assignment** and/or **Submission**, which represents the learning object that is being handed out or handed in.</span></span> <span data-ttu-id="1ac3c-107">Невозможно напрямую создать экземпляр ресурса; необходимо создать подкласс, который будет представлять тип используемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="1ac3c-107">You cannot instantiate a resource directly; you must make a subclass that will represent the type of resource being used.</span></span>

<span data-ttu-id="1ac3c-108">В этом ресурсе хранятся общие свойства для всех типов ресурсов.</span><span class="sxs-lookup"><span data-stu-id="1ac3c-108">This resource stores the common properties across all resource types.</span></span>


## <a name="properties"></a><span data-ttu-id="1ac3c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="1ac3c-109">Properties</span></span>
| <span data-ttu-id="1ac3c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="1ac3c-110">Property</span></span>     | <span data-ttu-id="1ac3c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="1ac3c-111">Type</span></span>   |<span data-ttu-id="1ac3c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1ac3c-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ac3c-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="1ac3c-113">createdBy</span></span>|[<span data-ttu-id="1ac3c-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="1ac3c-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="1ac3c-115">Кто создал ресурс.</span><span class="sxs-lookup"><span data-stu-id="1ac3c-115">Who created the resource.</span></span>|
|<span data-ttu-id="1ac3c-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1ac3c-116">createdDateTime</span></span>|<span data-ttu-id="1ac3c-117">Момент создания ресурса.</span><span class="sxs-lookup"><span data-stu-id="1ac3c-117">Moment in time when the resource was created.</span></span>  <span data-ttu-id="1ac3c-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ac3c-118">DateTimeOffset</span></span>|<span data-ttu-id="1ac3c-p104">Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601 (время всегда в формате UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="1ac3c-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="1ac3c-121">displayName</span><span class="sxs-lookup"><span data-stu-id="1ac3c-121">displayName</span></span>|<span data-ttu-id="1ac3c-122">String</span><span class="sxs-lookup"><span data-stu-id="1ac3c-122">String</span></span>|<span data-ttu-id="1ac3c-123">Отображаемое имя ресурса.</span><span class="sxs-lookup"><span data-stu-id="1ac3c-123">Display name of resource.</span></span>|
|<span data-ttu-id="1ac3c-124">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="1ac3c-124">lastModifiedBy</span></span>|[<span data-ttu-id="1ac3c-125">identitySet</span><span class="sxs-lookup"><span data-stu-id="1ac3c-125">identitySet</span></span>](identityset.md)|<span data-ttu-id="1ac3c-126">Кто последний пользователь изменил ресурс.</span><span class="sxs-lookup"><span data-stu-id="1ac3c-126">Who was the last user to modify the resource.</span></span>|
|<span data-ttu-id="1ac3c-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1ac3c-127">lastModifiedDateTime</span></span>|<span data-ttu-id="1ac3c-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ac3c-128">DateTimeOffset</span></span>|<span data-ttu-id="1ac3c-129">Момент времени последнего изменения ресурса.</span><span class="sxs-lookup"><span data-stu-id="1ac3c-129">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="1ac3c-130">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="1ac3c-130">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1ac3c-131">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="1ac3c-131">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1ac3c-132">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1ac3c-132">JSON representation</span></span>

<span data-ttu-id="1ac3c-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1ac3c-133">The following is a JSON representation of the resource.</span></span>

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
