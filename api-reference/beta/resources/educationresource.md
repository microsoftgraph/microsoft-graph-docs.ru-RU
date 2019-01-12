---
title: Тип ресурса educationResource
description: Суперкласса для всех объектов ресурсов в системе. Ресурс связан с **назначения** и/или **отправки**, который представляет объект обучения, который
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9ac84fd9d661f31186ea65e95c680456cdabe221
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982122"
---
# <a name="educationresource-resource-type"></a><span data-ttu-id="e9a01-104">Тип ресурса educationResource</span><span class="sxs-lookup"><span data-stu-id="e9a01-104">educationResource resource type</span></span>

> <span data-ttu-id="e9a01-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e9a01-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e9a01-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9a01-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e9a01-107">Суперкласса для всех объектов ресурсов в системе.</span><span class="sxs-lookup"><span data-stu-id="e9a01-107">A superclass for all resource objects in the system.</span></span> <span data-ttu-id="e9a01-108">Ресурс связан с **назначения** и/или **отправки**, который представляет объект обучения, который раздать или передачи.</span><span class="sxs-lookup"><span data-stu-id="e9a01-108">A resource is associated with an **Assignment** and/or **Submission**, which represents the learning object that is being handed out or handed in.</span></span> <span data-ttu-id="e9a01-109">Ресурс не могут создаваться напрямую; необходимо включить для подкласса, представляющий тип использования ресурсов.</span><span class="sxs-lookup"><span data-stu-id="e9a01-109">You cannot instantiate a resource directly; you must make a subclass that will represent the type of resource being used.</span></span>

<span data-ttu-id="e9a01-110">Этот ресурс сохраняет общие свойства для всех типов ресурсов.</span><span class="sxs-lookup"><span data-stu-id="e9a01-110">This resource stores the common properties across all resource types.</span></span>


## <a name="properties"></a><span data-ttu-id="e9a01-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="e9a01-111">Properties</span></span>
| <span data-ttu-id="e9a01-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9a01-112">Property</span></span>     | <span data-ttu-id="e9a01-113">Тип</span><span class="sxs-lookup"><span data-stu-id="e9a01-113">Type</span></span>   |<span data-ttu-id="e9a01-114">Описание</span><span class="sxs-lookup"><span data-stu-id="e9a01-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9a01-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="e9a01-115">createdBy</span></span>|[<span data-ttu-id="e9a01-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="e9a01-116">identitySet</span></span>](identityset.md)|<span data-ttu-id="e9a01-117">Создатель ресурса.</span><span class="sxs-lookup"><span data-stu-id="e9a01-117">Who created the resource.</span></span>|
|<span data-ttu-id="e9a01-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e9a01-118">createdDateTime</span></span>|<span data-ttu-id="e9a01-119">Момент времени, когда был создан ресурса.</span><span class="sxs-lookup"><span data-stu-id="e9a01-119">Moment in time when the resource was created.</span></span>  <span data-ttu-id="e9a01-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9a01-120">DateTimeOffset</span></span>|<span data-ttu-id="e9a01-p105">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e9a01-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e9a01-123">displayName</span><span class="sxs-lookup"><span data-stu-id="e9a01-123">displayName</span></span>|<span data-ttu-id="e9a01-124">Строка</span><span class="sxs-lookup"><span data-stu-id="e9a01-124">String</span></span>|<span data-ttu-id="e9a01-125">Отображаемое имя ресурса.</span><span class="sxs-lookup"><span data-stu-id="e9a01-125">Display name of resource.</span></span>|
|<span data-ttu-id="e9a01-126">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="e9a01-126">lastModifiedBy</span></span>|[<span data-ttu-id="e9a01-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="e9a01-127">identitySet</span></span>](identityset.md)|<span data-ttu-id="e9a01-128">Кто был последний пользователям изменять ресурса.</span><span class="sxs-lookup"><span data-stu-id="e9a01-128">Who was the last user to modify the resource.</span></span>|
|<span data-ttu-id="e9a01-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e9a01-129">lastModifiedDateTime</span></span>|<span data-ttu-id="e9a01-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9a01-130">DateTimeOffset</span></span>|<span data-ttu-id="e9a01-131">Момент времени, время последнего изменения ресурса.</span><span class="sxs-lookup"><span data-stu-id="e9a01-131">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="e9a01-132">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="e9a01-132">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e9a01-133">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e9a01-133">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e9a01-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e9a01-134">JSON representation</span></span>

<span data-ttu-id="e9a01-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9a01-135">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
