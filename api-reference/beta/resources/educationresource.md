---
title: тип ресурсов educationResource
description: Суперкласс для всех объектов ресурса в системе. Ресурс связан с  назначением и/или **отправкой,** представляюще обучающий объект, который находится в настоящее время
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: df2e9b0c49085503e76d56643a755e74e2f0cfaa
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722407"
---
# <a name="educationresource-resource-type"></a><span data-ttu-id="8571c-104">тип ресурсов educationResource</span><span class="sxs-lookup"><span data-stu-id="8571c-104">educationResource resource type</span></span>

<span data-ttu-id="8571c-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8571c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8571c-106">Суперкласс для всех объектов ресурса в системе.</span><span class="sxs-lookup"><span data-stu-id="8571c-106">A superclass for all resource objects in the system.</span></span> <span data-ttu-id="8571c-107">Ресурс связан с  назначением и/или отправкой, представляюще обучающий объект, который передается или передается.</span><span class="sxs-lookup"><span data-stu-id="8571c-107">A resource is associated with an **Assignment** and/or **Submission**, which represents the learning object that is being handed out or handed in.</span></span> <span data-ttu-id="8571c-108">Вы не можете мгновенно получить ресурс напрямую; необходимо сделать подкласс, который будет представлять тип используемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="8571c-108">You cannot instantiate a resource directly; you must make a subclass that will represent the type of resource being used.</span></span>

<span data-ttu-id="8571c-109">Этот ресурс сохраняет общие свойства для всех типов ресурсов.</span><span class="sxs-lookup"><span data-stu-id="8571c-109">This resource stores the common properties across all resource types.</span></span>


## <a name="properties"></a><span data-ttu-id="8571c-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="8571c-110">Properties</span></span>
| <span data-ttu-id="8571c-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="8571c-111">Property</span></span>     | <span data-ttu-id="8571c-112">Тип</span><span class="sxs-lookup"><span data-stu-id="8571c-112">Type</span></span>   |<span data-ttu-id="8571c-113">Описание</span><span class="sxs-lookup"><span data-stu-id="8571c-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8571c-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="8571c-114">createdBy</span></span>|[<span data-ttu-id="8571c-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="8571c-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="8571c-116">Кто создал ресурс.</span><span class="sxs-lookup"><span data-stu-id="8571c-116">Who created the resource.</span></span>|
|<span data-ttu-id="8571c-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8571c-117">createdDateTime</span></span>|<span data-ttu-id="8571c-118">Момент создания ресурса.</span><span class="sxs-lookup"><span data-stu-id="8571c-118">Moment in time when the resource was created.</span></span>  <span data-ttu-id="8571c-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8571c-119">DateTimeOffset</span></span>|<span data-ttu-id="8571c-120">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="8571c-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8571c-121">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="8571c-121">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="8571c-122">displayName</span><span class="sxs-lookup"><span data-stu-id="8571c-122">displayName</span></span>|<span data-ttu-id="8571c-123">String</span><span class="sxs-lookup"><span data-stu-id="8571c-123">String</span></span>|<span data-ttu-id="8571c-124">Отображение имени ресурса.</span><span class="sxs-lookup"><span data-stu-id="8571c-124">Display name of resource.</span></span>|
|<span data-ttu-id="8571c-125">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="8571c-125">lastModifiedBy</span></span>|[<span data-ttu-id="8571c-126">identitySet</span><span class="sxs-lookup"><span data-stu-id="8571c-126">identitySet</span></span>](identityset.md)|<span data-ttu-id="8571c-127">Кто был последним пользователем, который модифицировать ресурс.</span><span class="sxs-lookup"><span data-stu-id="8571c-127">Who was the last user to modify the resource.</span></span>|
|<span data-ttu-id="8571c-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8571c-128">lastModifiedDateTime</span></span>|<span data-ttu-id="8571c-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8571c-129">DateTimeOffset</span></span>|<span data-ttu-id="8571c-130">Время последнего изменения ресурса.</span><span class="sxs-lookup"><span data-stu-id="8571c-130">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="8571c-131">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="8571c-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8571c-132">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="8571c-132">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8571c-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8571c-133">JSON representation</span></span>

<span data-ttu-id="8571c-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8571c-134">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->


