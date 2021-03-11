---
title: тип ресурса governanceSchedule
description: 'Представляет расписание для governanceRoleAssignmentRequest. Для запроса назначения ролей расписание контролирует время выполнения операции назначения ролей, остановку назначения ролей и частое выполнение операции назначения ролей. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: f7583f15641c541493ded9f9a4779777e9f35f2a
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722286"
---
# <a name="governanceschedule-resource-type"></a><span data-ttu-id="b7533-104">тип ресурса governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="b7533-104">governanceSchedule resource type</span></span>

<span data-ttu-id="b7533-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7533-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7533-106">Представляет расписание для [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="b7533-106">Represents the schedule for a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> <span data-ttu-id="b7533-107">Для запроса назначения ролей расписание контролирует время выполнения операции назначения ролей, остановку назначения ролей и частое выполнение операции назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="b7533-107">For a role assignment request, the schedule controls when to perform the role assignment operation, when to stop the role assignment, and how frequently to do the role assignment operation.</span></span>



## <a name="properties"></a><span data-ttu-id="b7533-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b7533-108">Properties</span></span>
| <span data-ttu-id="b7533-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b7533-109">Property</span></span>     | <span data-ttu-id="b7533-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b7533-110">Type</span></span>   |<span data-ttu-id="b7533-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b7533-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7533-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b7533-112">startDateTime</span></span>|<span data-ttu-id="b7533-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7533-113">DateTimeOffset</span></span>|<span data-ttu-id="b7533-114">Время начала назначения роли.</span><span class="sxs-lookup"><span data-stu-id="b7533-114">The start time of the role assignment.</span></span> <span data-ttu-id="b7533-115">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="b7533-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b7533-116">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="b7533-116">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="b7533-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="b7533-117">endDateTime</span></span>|<span data-ttu-id="b7533-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7533-118">DateTimeOffset</span></span>|<span data-ttu-id="b7533-119">Конечное время назначения роли.</span><span class="sxs-lookup"><span data-stu-id="b7533-119">The end time of the role assignment.</span></span> <span data-ttu-id="b7533-120">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="b7533-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b7533-121">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="b7533-121">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="b7533-122">*Примечание. Если это `null` значение, оно указывает на постоянное назначение.*</span><span class="sxs-lookup"><span data-stu-id="b7533-122">*Note: if the value is `null`, it indicates a permanent assignment.*</span></span>|
|<span data-ttu-id="b7533-123">type</span><span class="sxs-lookup"><span data-stu-id="b7533-123">type</span></span>|<span data-ttu-id="b7533-124">String</span><span class="sxs-lookup"><span data-stu-id="b7533-124">String</span></span>|<span data-ttu-id="b7533-125">Тип расписания назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="b7533-125">The role assignment schedule type.</span></span> <span data-ttu-id="b7533-126">Только `Once` поддерживается на данный момент.</span><span class="sxs-lookup"><span data-stu-id="b7533-126">Only `Once` is supported for now.</span></span>
|<span data-ttu-id="b7533-127">duration</span><span class="sxs-lookup"><span data-stu-id="b7533-127">duration</span></span>|<span data-ttu-id="b7533-128">Duration</span><span class="sxs-lookup"><span data-stu-id="b7533-128">Duration</span></span>|<span data-ttu-id="b7533-129">Продолжительность назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="b7533-129">The duration of a role assignment.</span></span> <span data-ttu-id="b7533-130">Он находится в формате TimeSpan.</span><span class="sxs-lookup"><span data-stu-id="b7533-130">It is in format of a TimeSpan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b7533-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b7533-131">JSON representation</span></span>

<span data-ttu-id="b7533-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b7533-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceSchedule"
}-->

```json
{
  "duration": "String (timespan)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceSchedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


