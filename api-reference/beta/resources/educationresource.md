---
title: Тип ресурса Едукатионресаурце
description: Суперкласс для всех объектов ресурсов в системе. Ресурс связан с **назначением** и/или **отправкой**, представляющим обучающий объект, который
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: dc2c1c4ecd6ce7b57992637bfdcf9a1523265f90
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501096"
---
# <a name="educationresource-resource-type"></a><span data-ttu-id="52c7f-104">Тип ресурса Едукатионресаурце</span><span class="sxs-lookup"><span data-stu-id="52c7f-104">educationResource resource type</span></span>

<span data-ttu-id="52c7f-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="52c7f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52c7f-106">Суперкласс для всех объектов ресурсов в системе.</span><span class="sxs-lookup"><span data-stu-id="52c7f-106">A superclass for all resource objects in the system.</span></span> <span data-ttu-id="52c7f-107">Ресурс связан с **назначением** и/или **отправкой**, представляющим обучающий объект, который передается или передается.</span><span class="sxs-lookup"><span data-stu-id="52c7f-107">A resource is associated with an **Assignment** and/or **Submission**, which represents the learning object that is being handed out or handed in.</span></span> <span data-ttu-id="52c7f-108">Невозможно напрямую создать экземпляр ресурса; необходимо создать подкласс, который будет представлять тип используемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="52c7f-108">You cannot instantiate a resource directly; you must make a subclass that will represent the type of resource being used.</span></span>

<span data-ttu-id="52c7f-109">В этом ресурсе хранятся общие свойства для всех типов ресурсов.</span><span class="sxs-lookup"><span data-stu-id="52c7f-109">This resource stores the common properties across all resource types.</span></span>


## <a name="properties"></a><span data-ttu-id="52c7f-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="52c7f-110">Properties</span></span>
| <span data-ttu-id="52c7f-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="52c7f-111">Property</span></span>     | <span data-ttu-id="52c7f-112">Тип</span><span class="sxs-lookup"><span data-stu-id="52c7f-112">Type</span></span>   |<span data-ttu-id="52c7f-113">Описание</span><span class="sxs-lookup"><span data-stu-id="52c7f-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52c7f-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="52c7f-114">createdBy</span></span>|[<span data-ttu-id="52c7f-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="52c7f-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="52c7f-116">Кто создал ресурс.</span><span class="sxs-lookup"><span data-stu-id="52c7f-116">Who created the resource.</span></span>|
|<span data-ttu-id="52c7f-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="52c7f-117">createdDateTime</span></span>|<span data-ttu-id="52c7f-118">Момент создания ресурса.</span><span class="sxs-lookup"><span data-stu-id="52c7f-118">Moment in time when the resource was created.</span></span>  <span data-ttu-id="52c7f-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52c7f-119">DateTimeOffset</span></span>|<span data-ttu-id="52c7f-p104">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="52c7f-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="52c7f-122">displayName</span><span class="sxs-lookup"><span data-stu-id="52c7f-122">displayName</span></span>|<span data-ttu-id="52c7f-123">String</span><span class="sxs-lookup"><span data-stu-id="52c7f-123">String</span></span>|<span data-ttu-id="52c7f-124">Отображаемое имя ресурса.</span><span class="sxs-lookup"><span data-stu-id="52c7f-124">Display name of resource.</span></span>|
|<span data-ttu-id="52c7f-125">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="52c7f-125">lastModifiedBy</span></span>|[<span data-ttu-id="52c7f-126">identitySet</span><span class="sxs-lookup"><span data-stu-id="52c7f-126">identitySet</span></span>](identityset.md)|<span data-ttu-id="52c7f-127">Кто последний пользователь изменил ресурс.</span><span class="sxs-lookup"><span data-stu-id="52c7f-127">Who was the last user to modify the resource.</span></span>|
|<span data-ttu-id="52c7f-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="52c7f-128">lastModifiedDateTime</span></span>|<span data-ttu-id="52c7f-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52c7f-129">DateTimeOffset</span></span>|<span data-ttu-id="52c7f-130">Момент времени последнего изменения ресурса.</span><span class="sxs-lookup"><span data-stu-id="52c7f-130">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="52c7f-131">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="52c7f-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="52c7f-132">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="52c7f-132">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="52c7f-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="52c7f-133">JSON representation</span></span>

<span data-ttu-id="52c7f-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52c7f-134">The following is a JSON representation of the resource.</span></span>

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
