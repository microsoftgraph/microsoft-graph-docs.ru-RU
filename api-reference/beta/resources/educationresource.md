---
title: Тип ресурса Едукатионресаурце
description: Суперкласс для всех объектов ресурсов в системе. Ресурс связан с назначением **** и/или отправкой, представляющим обучающий объект, который ****
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 8dfb996c863e3b2aa5e319fcd2b4dc6dd246751a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972609"
---
# <a name="educationresource-resource-type"></a><span data-ttu-id="c42a9-104">Тип ресурса Едукатионресаурце</span><span class="sxs-lookup"><span data-stu-id="c42a9-104">educationResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c42a9-105">Суперкласс для всех объектов ресурсов в системе.</span><span class="sxs-lookup"><span data-stu-id="c42a9-105">A superclass for all resource objects in the system.</span></span> <span data-ttu-id="c42a9-106">Ресурс связан с назначением \*\*\*\* и/или отправкой, представляющим обучающий объект, который передается или передается. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="c42a9-106">A resource is associated with an **Assignment** and/or **Submission**, which represents the learning object that is being handed out or handed in.</span></span> <span data-ttu-id="c42a9-107">Невозможно напрямую создать экземпляр ресурса; необходимо создать подкласс, который будет представлять тип используемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="c42a9-107">You cannot instantiate a resource directly; you must make a subclass that will represent the type of resource being used.</span></span>

<span data-ttu-id="c42a9-108">В этом ресурсе хранятся общие свойства для всех типов ресурсов.</span><span class="sxs-lookup"><span data-stu-id="c42a9-108">This resource stores the common properties across all resource types.</span></span>


## <a name="properties"></a><span data-ttu-id="c42a9-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c42a9-109">Properties</span></span>
| <span data-ttu-id="c42a9-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c42a9-110">Property</span></span>     | <span data-ttu-id="c42a9-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c42a9-111">Type</span></span>   |<span data-ttu-id="c42a9-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c42a9-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c42a9-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="c42a9-113">createdBy</span></span>|[<span data-ttu-id="c42a9-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="c42a9-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="c42a9-115">Кто создал ресурс.</span><span class="sxs-lookup"><span data-stu-id="c42a9-115">Who created the resource.</span></span>|
|<span data-ttu-id="c42a9-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c42a9-116">createdDateTime</span></span>|<span data-ttu-id="c42a9-117">Момент создания ресурса.</span><span class="sxs-lookup"><span data-stu-id="c42a9-117">Moment in time when the resource was created.</span></span>  <span data-ttu-id="c42a9-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c42a9-118">DateTimeOffset</span></span>|<span data-ttu-id="c42a9-p104">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c42a9-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c42a9-121">displayName</span><span class="sxs-lookup"><span data-stu-id="c42a9-121">displayName</span></span>|<span data-ttu-id="c42a9-122">String</span><span class="sxs-lookup"><span data-stu-id="c42a9-122">String</span></span>|<span data-ttu-id="c42a9-123">Отображаемое имя ресурса.</span><span class="sxs-lookup"><span data-stu-id="c42a9-123">Display name of resource.</span></span>|
|<span data-ttu-id="c42a9-124">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="c42a9-124">lastModifiedBy</span></span>|[<span data-ttu-id="c42a9-125">identitySet</span><span class="sxs-lookup"><span data-stu-id="c42a9-125">identitySet</span></span>](identityset.md)|<span data-ttu-id="c42a9-126">Кто последний пользователь изменил ресурс.</span><span class="sxs-lookup"><span data-stu-id="c42a9-126">Who was the last user to modify the resource.</span></span>|
|<span data-ttu-id="c42a9-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c42a9-127">lastModifiedDateTime</span></span>|<span data-ttu-id="c42a9-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c42a9-128">DateTimeOffset</span></span>|<span data-ttu-id="c42a9-129">Момент времени последнего изменения ресурса.</span><span class="sxs-lookup"><span data-stu-id="c42a9-129">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="c42a9-130">Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="c42a9-130">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c42a9-131">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c42a9-131">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c42a9-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c42a9-132">JSON representation</span></span>

<span data-ttu-id="c42a9-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c42a9-133">The following is a JSON representation of the resource.</span></span>

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
