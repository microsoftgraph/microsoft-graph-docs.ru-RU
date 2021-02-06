---
title: Тип ресурса governanceSchedule
description: 'Представляет расписание для governanceRoleAssignmentRequest. Для запроса на назначение роли расписание контролирует время выполнения операции назначения роли, время остановки назначения роли и то, как часто выполняется операция назначения ролей. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: e7b444b1daa45daf3228476fb48a38be4e7bb2b2
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132678"
---
# <a name="governanceschedule-resource-type"></a><span data-ttu-id="96668-104">Тип ресурса governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="96668-104">governanceSchedule resource type</span></span>

<span data-ttu-id="96668-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96668-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96668-106">Представляет расписание для [governanceRoleAssignmentRequest.](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="96668-106">Represents the schedule for a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> <span data-ttu-id="96668-107">Для запроса на назначение роли расписание контролирует время выполнения операции назначения роли, время остановки назначения роли и время выполнения операции назначения роли.</span><span class="sxs-lookup"><span data-stu-id="96668-107">For a role assignment request, the schedule controls when to perform the role assignment operation, when to stop the role assignment, and how frequently to do the role assignment operation.</span></span>



## <a name="properties"></a><span data-ttu-id="96668-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="96668-108">Properties</span></span>
| <span data-ttu-id="96668-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="96668-109">Property</span></span>     | <span data-ttu-id="96668-110">Тип</span><span class="sxs-lookup"><span data-stu-id="96668-110">Type</span></span>   |<span data-ttu-id="96668-111">Описание</span><span class="sxs-lookup"><span data-stu-id="96668-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96668-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="96668-112">startDateTime</span></span>|<span data-ttu-id="96668-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96668-113">DateTimeOffset</span></span>|<span data-ttu-id="96668-114">Время начала назначения роли.</span><span class="sxs-lookup"><span data-stu-id="96668-114">The start time of the role assignment.</span></span> <span data-ttu-id="96668-115">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="96668-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="96668-116">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="96668-116">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="96668-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="96668-117">endDateTime</span></span>|<span data-ttu-id="96668-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96668-118">DateTimeOffset</span></span>|<span data-ttu-id="96668-119">Время окончания назначения роли.</span><span class="sxs-lookup"><span data-stu-id="96668-119">The end time of the role assignment.</span></span> <span data-ttu-id="96668-120">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="96668-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="96668-121">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="96668-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="96668-122">*Примечание. Если это значение, `null` оно указывает на постоянное назначение.*</span><span class="sxs-lookup"><span data-stu-id="96668-122">*Note: if the value is `null`, it indicates a permanent assignment.*</span></span>|
|<span data-ttu-id="96668-123">type</span><span class="sxs-lookup"><span data-stu-id="96668-123">type</span></span>|<span data-ttu-id="96668-124">Строка</span><span class="sxs-lookup"><span data-stu-id="96668-124">String</span></span>|<span data-ttu-id="96668-125">Тип расписания назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="96668-125">The role assignment schedule type.</span></span> <span data-ttu-id="96668-126">Пока `Once` поддерживается только.</span><span class="sxs-lookup"><span data-stu-id="96668-126">Only `Once` is supported for now.</span></span>
|<span data-ttu-id="96668-127">duration</span><span class="sxs-lookup"><span data-stu-id="96668-127">duration</span></span>|<span data-ttu-id="96668-128">Duration</span><span class="sxs-lookup"><span data-stu-id="96668-128">Duration</span></span>|<span data-ttu-id="96668-129">Продолжительность назначения роли.</span><span class="sxs-lookup"><span data-stu-id="96668-129">The duration of a role assignment.</span></span> <span data-ttu-id="96668-130">Он имеет формат TimeSpan.</span><span class="sxs-lookup"><span data-stu-id="96668-130">It is in format of a TimeSpan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="96668-131">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="96668-131">JSON representation</span></span>

<span data-ttu-id="96668-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="96668-132">Here is a JSON representation of the resource.</span></span>

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


