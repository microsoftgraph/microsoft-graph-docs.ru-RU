---
title: Тип ресурса Говернанцесчедуле
description: 'Представляет расписание для объекта governanceRoleAssignmentRequest. Для запроса на назначение роли расписание определяет, когда следует выполнять операцию назначения роли, когда следует остановить назначение роли и как часто выполняется операция назначения роли. '
localization_priority: Normal
ms.openlocfilehash: 798b2a7f3e67ac466189f1ece55437214931056d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340318"
---
# <a name="governanceschedule-resource-type"></a><span data-ttu-id="b3607-104">Тип ресурса Говернанцесчедуле</span><span class="sxs-lookup"><span data-stu-id="b3607-104">governanceSchedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3607-105">Представляет расписание для объекта [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="b3607-105">Represents the schedule for a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> <span data-ttu-id="b3607-106">Для запроса на назначение роли расписание определяет, когда следует выполнять операцию назначения роли, когда следует остановить назначение роли и как часто выполняется операция назначения роли.</span><span class="sxs-lookup"><span data-stu-id="b3607-106">For a role assignment request, the schedule controls when to perform the role assignment operation, when to stop the role assignment, and how frequently to do the role assignment operation.</span></span> 



## <a name="properties"></a><span data-ttu-id="b3607-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b3607-107">Properties</span></span>
| <span data-ttu-id="b3607-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b3607-108">Property</span></span>     | <span data-ttu-id="b3607-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b3607-109">Type</span></span>   |<span data-ttu-id="b3607-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b3607-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b3607-111">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b3607-111">startDateTime</span></span>|<span data-ttu-id="b3607-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3607-112">DateTimeOffset</span></span>|<span data-ttu-id="b3607-113">Время начала назначения роли.</span><span class="sxs-lookup"><span data-stu-id="b3607-113">The start time of the role assignment.</span></span> <span data-ttu-id="b3607-114">Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="b3607-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b3607-115">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b3607-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b3607-116">endDateTime</span><span class="sxs-lookup"><span data-stu-id="b3607-116">endDateTime</span></span>|<span data-ttu-id="b3607-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3607-117">DateTimeOffset</span></span>|<span data-ttu-id="b3607-118">Время окончания назначения роли.</span><span class="sxs-lookup"><span data-stu-id="b3607-118">The end time of the role assignment.</span></span> <span data-ttu-id="b3607-119">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="b3607-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b3607-120">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b3607-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="b3607-121">*Note: Если значение задано `null`, оно указывает на постоянное назначение.*</span><span class="sxs-lookup"><span data-stu-id="b3607-121">*Note: if the value is `null`, it indicates a permanent assignment.*</span></span>|
|<span data-ttu-id="b3607-122">type</span><span class="sxs-lookup"><span data-stu-id="b3607-122">type</span></span>|<span data-ttu-id="b3607-123">String</span><span class="sxs-lookup"><span data-stu-id="b3607-123">String</span></span>|<span data-ttu-id="b3607-124">Тип расписания назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="b3607-124">The role assignment schedule type.</span></span> <span data-ttu-id="b3607-125">Поддерживается `Once` только в настоящее время.</span><span class="sxs-lookup"><span data-stu-id="b3607-125">Only `Once` is supported for now.</span></span>
|<span data-ttu-id="b3607-126">duration</span><span class="sxs-lookup"><span data-stu-id="b3607-126">duration</span></span>|<span data-ttu-id="b3607-127">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="b3607-127">Duration</span></span>|<span data-ttu-id="b3607-128">Продолжительность назначения роли.</span><span class="sxs-lookup"><span data-stu-id="b3607-128">The duration of a role assignment.</span></span> <span data-ttu-id="b3607-129">Он имеет формат TimeSpan.</span><span class="sxs-lookup"><span data-stu-id="b3607-129">It is in format of a TimeSpan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b3607-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b3607-130">JSON representation</span></span>

<span data-ttu-id="b3607-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b3607-131">Here is a JSON representation of the resource.</span></span>

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
