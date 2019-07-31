---
title: Тип ресурса Говернанцесчедуле
description: 'Представляет расписание для объекта governanceRoleAssignmentRequest. Для запроса на назначение роли расписание определяет, когда следует выполнять операцию назначения роли, когда следует остановить назначение роли и как часто выполняется операция назначения роли. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 36a2b4c73f5f85439a34a42ea2aa23cfe861c4ab
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006376"
---
# <a name="governanceschedule-resource-type"></a><span data-ttu-id="87c57-104">Тип ресурса Говернанцесчедуле</span><span class="sxs-lookup"><span data-stu-id="87c57-104">governanceSchedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87c57-105">Представляет расписание для объекта [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="87c57-105">Represents the schedule for a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> <span data-ttu-id="87c57-106">Для запроса на назначение роли расписание определяет, когда следует выполнять операцию назначения роли, когда следует остановить назначение роли и как часто выполняется операция назначения роли.</span><span class="sxs-lookup"><span data-stu-id="87c57-106">For a role assignment request, the schedule controls when to perform the role assignment operation, when to stop the role assignment, and how frequently to do the role assignment operation.</span></span> 



## <a name="properties"></a><span data-ttu-id="87c57-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="87c57-107">Properties</span></span>
| <span data-ttu-id="87c57-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="87c57-108">Property</span></span>     | <span data-ttu-id="87c57-109">Тип</span><span class="sxs-lookup"><span data-stu-id="87c57-109">Type</span></span>   |<span data-ttu-id="87c57-110">Описание</span><span class="sxs-lookup"><span data-stu-id="87c57-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="87c57-111">startDateTime</span><span class="sxs-lookup"><span data-stu-id="87c57-111">startDateTime</span></span>|<span data-ttu-id="87c57-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87c57-112">DateTimeOffset</span></span>|<span data-ttu-id="87c57-113">Время начала назначения роли.</span><span class="sxs-lookup"><span data-stu-id="87c57-113">The start time of the role assignment.</span></span> <span data-ttu-id="87c57-114">Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="87c57-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="87c57-115">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="87c57-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="87c57-116">endDateTime</span><span class="sxs-lookup"><span data-stu-id="87c57-116">endDateTime</span></span>|<span data-ttu-id="87c57-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87c57-117">DateTimeOffset</span></span>|<span data-ttu-id="87c57-118">Время окончания назначения роли.</span><span class="sxs-lookup"><span data-stu-id="87c57-118">The end time of the role assignment.</span></span> <span data-ttu-id="87c57-119">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="87c57-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="87c57-120">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="87c57-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="87c57-121">*Note: Если значение задано `null`, оно указывает на постоянное назначение.*</span><span class="sxs-lookup"><span data-stu-id="87c57-121">*Note: if the value is `null`, it indicates a permanent assignment.*</span></span>|
|<span data-ttu-id="87c57-122">type</span><span class="sxs-lookup"><span data-stu-id="87c57-122">type</span></span>|<span data-ttu-id="87c57-123">String</span><span class="sxs-lookup"><span data-stu-id="87c57-123">String</span></span>|<span data-ttu-id="87c57-124">Тип расписания назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="87c57-124">The role assignment schedule type.</span></span> <span data-ttu-id="87c57-125">Поддерживается `Once` только в настоящее время.</span><span class="sxs-lookup"><span data-stu-id="87c57-125">Only `Once` is supported for now.</span></span>
|<span data-ttu-id="87c57-126">duration</span><span class="sxs-lookup"><span data-stu-id="87c57-126">duration</span></span>|<span data-ttu-id="87c57-127">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="87c57-127">Duration</span></span>|<span data-ttu-id="87c57-128">Продолжительность назначения роли.</span><span class="sxs-lookup"><span data-stu-id="87c57-128">The duration of a role assignment.</span></span> <span data-ttu-id="87c57-129">Он имеет формат TimeSpan.</span><span class="sxs-lookup"><span data-stu-id="87c57-129">It is in format of a TimeSpan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="87c57-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="87c57-130">JSON representation</span></span>

<span data-ttu-id="87c57-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="87c57-131">Here is a JSON representation of the resource.</span></span>

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
