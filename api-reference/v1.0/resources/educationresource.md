---
title: тип ресурсов educationResource
description: Суперкласс для всех объектов ресурса в системе.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f817740ff7879d20788b46debad0824499f56498
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442439"
---
# <a name="educationresource-resource-type"></a><span data-ttu-id="6c15d-103">тип ресурсов educationResource</span><span class="sxs-lookup"><span data-stu-id="6c15d-103">educationResource resource type</span></span>

<span data-ttu-id="6c15d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c15d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6c15d-105">Суперкласс для всех объектов ресурса в системе.</span><span class="sxs-lookup"><span data-stu-id="6c15d-105">A superclass for all resource objects in the system.</span></span> <span data-ttu-id="6c15d-106">Ресурс связан с  назначением и/или отправкой, представляюще обучающий объект, который передается или передается.</span><span class="sxs-lookup"><span data-stu-id="6c15d-106">A resource is associated with an **Assignment** and/or **Submission**, which represents the learning object that is being handed out or handed in.</span></span> <span data-ttu-id="6c15d-107">Вы не можете мгновенно получить ресурс напрямую; необходимо сделать подкласс, который будет представлять тип используемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="6c15d-107">You cannot instantiate a resource directly; you must make a subclass that will represent the type of resource being used.</span></span>

<span data-ttu-id="6c15d-108">Этот ресурс сохраняет общие свойства для всех типов ресурсов.</span><span class="sxs-lookup"><span data-stu-id="6c15d-108">This resource stores the common properties across all resource types.</span></span>


## <a name="properties"></a><span data-ttu-id="6c15d-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="6c15d-109">Properties</span></span>
| <span data-ttu-id="6c15d-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c15d-110">Property</span></span>     | <span data-ttu-id="6c15d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="6c15d-111">Type</span></span>   |<span data-ttu-id="6c15d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="6c15d-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c15d-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="6c15d-113">createdBy</span></span>|[<span data-ttu-id="6c15d-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="6c15d-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="6c15d-115">Человек, создавший ресурс.</span><span class="sxs-lookup"><span data-stu-id="6c15d-115">The individual who created the resource.</span></span>|
|<span data-ttu-id="6c15d-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c15d-116">createdDateTime</span></span>|<span data-ttu-id="6c15d-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c15d-117">DateTimeOffset</span></span>|<span data-ttu-id="6c15d-118">Момент создания ресурса.</span><span class="sxs-lookup"><span data-stu-id="6c15d-118">Moment in time when the resource was created.</span></span> <span data-ttu-id="6c15d-119">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="6c15d-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6c15d-120">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="6c15d-120">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="6c15d-121">displayName</span><span class="sxs-lookup"><span data-stu-id="6c15d-121">displayName</span></span>|<span data-ttu-id="6c15d-122">String</span><span class="sxs-lookup"><span data-stu-id="6c15d-122">String</span></span>|<span data-ttu-id="6c15d-123">Отображение имени ресурса.</span><span class="sxs-lookup"><span data-stu-id="6c15d-123">Display name of resource.</span></span>|
|<span data-ttu-id="6c15d-124">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="6c15d-124">lastModifiedBy</span></span>|[<span data-ttu-id="6c15d-125">identitySet</span><span class="sxs-lookup"><span data-stu-id="6c15d-125">identitySet</span></span>](identityset.md)|<span data-ttu-id="6c15d-126">Последний пользователь, который изменит ресурс.</span><span class="sxs-lookup"><span data-stu-id="6c15d-126">The last user to modify the resource.</span></span>|
|<span data-ttu-id="6c15d-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c15d-127">lastModifiedDateTime</span></span>|<span data-ttu-id="6c15d-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c15d-128">DateTimeOffset</span></span>|<span data-ttu-id="6c15d-129">Время последнего изменения ресурса.</span><span class="sxs-lookup"><span data-stu-id="6c15d-129">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="6c15d-130">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="6c15d-130">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6c15d-131">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="6c15d-131">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6c15d-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6c15d-132">JSON representation</span></span>

<span data-ttu-id="6c15d-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6c15d-133">The following is a JSON representation of the resource.</span></span>

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


