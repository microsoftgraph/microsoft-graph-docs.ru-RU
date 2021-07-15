---
title: тип ресурсов educationResource
description: Суперкласс для всех объектов ресурса в системе. Ресурс связан с  назначением и/или **отправкой,** представляюще обучающий объект, который находится в настоящее время
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f82274782f84204be288c67365288891f64fedf6
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440948"
---
# <a name="educationresource-resource-type"></a><span data-ttu-id="ea230-104">тип ресурсов educationResource</span><span class="sxs-lookup"><span data-stu-id="ea230-104">educationResource resource type</span></span>

<span data-ttu-id="ea230-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea230-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea230-106">Суперкласс для всех объектов ресурса в системе.</span><span class="sxs-lookup"><span data-stu-id="ea230-106">A superclass for all resource objects in the system.</span></span> <span data-ttu-id="ea230-107">Ресурс связан с  назначением и/или отправкой, представляюще обучающий объект, который передается или передается.</span><span class="sxs-lookup"><span data-stu-id="ea230-107">A resource is associated with an **Assignment** and/or **Submission**, which represents the learning object that is being handed out or handed in.</span></span> <span data-ttu-id="ea230-108">Вы не можете мгновенно получить ресурс напрямую; необходимо сделать подкласс, который будет представлять тип используемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="ea230-108">You cannot instantiate a resource directly; you must make a subclass that will represent the type of resource being used.</span></span>

<span data-ttu-id="ea230-109">Этот ресурс сохраняет общие свойства для всех типов ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ea230-109">This resource stores the common properties across all resource types.</span></span>


## <a name="properties"></a><span data-ttu-id="ea230-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="ea230-110">Properties</span></span>
| <span data-ttu-id="ea230-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea230-111">Property</span></span>     | <span data-ttu-id="ea230-112">Тип</span><span class="sxs-lookup"><span data-stu-id="ea230-112">Type</span></span>   |<span data-ttu-id="ea230-113">Описание</span><span class="sxs-lookup"><span data-stu-id="ea230-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea230-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="ea230-114">createdBy</span></span>|[<span data-ttu-id="ea230-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="ea230-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="ea230-116">Кто создал ресурс.</span><span class="sxs-lookup"><span data-stu-id="ea230-116">Who created the resource.</span></span>|
|<span data-ttu-id="ea230-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ea230-117">createdDateTime</span></span>|<span data-ttu-id="ea230-118">Момент создания ресурса.</span><span class="sxs-lookup"><span data-stu-id="ea230-118">Moment in time when the resource was created.</span></span>  <span data-ttu-id="ea230-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea230-119">DateTimeOffset</span></span>|<span data-ttu-id="ea230-120">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="ea230-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ea230-121">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="ea230-121">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="ea230-122">displayName</span><span class="sxs-lookup"><span data-stu-id="ea230-122">displayName</span></span>|<span data-ttu-id="ea230-123">String</span><span class="sxs-lookup"><span data-stu-id="ea230-123">String</span></span>|<span data-ttu-id="ea230-124">Отображение имени ресурса.</span><span class="sxs-lookup"><span data-stu-id="ea230-124">Display name of resource.</span></span>|
|<span data-ttu-id="ea230-125">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ea230-125">lastModifiedBy</span></span>|[<span data-ttu-id="ea230-126">identitySet</span><span class="sxs-lookup"><span data-stu-id="ea230-126">identitySet</span></span>](identityset.md)|<span data-ttu-id="ea230-127">Кто был последним пользователем, который модифицировать ресурс.</span><span class="sxs-lookup"><span data-stu-id="ea230-127">Who was the last user to modify the resource.</span></span>|
|<span data-ttu-id="ea230-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ea230-128">lastModifiedDateTime</span></span>|<span data-ttu-id="ea230-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea230-129">DateTimeOffset</span></span>|<span data-ttu-id="ea230-130">Время последнего изменения ресурса.</span><span class="sxs-lookup"><span data-stu-id="ea230-130">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="ea230-131">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="ea230-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ea230-132">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="ea230-132">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ea230-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ea230-133">JSON representation</span></span>

<span data-ttu-id="ea230-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea230-134">The following is a JSON representation of the resource.</span></span>

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


