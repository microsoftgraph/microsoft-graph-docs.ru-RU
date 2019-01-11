---
title: Тип ресурса governanceSchedule
description: 'Представляет расписание для governanceRoleAssignmentRequest. Для запроса назначений ролей, расписание определяет, когда следует выполнить операцию назначения ролей, время завершения назначения ролей и как часто следует выполнить операцию назначения ролей. '
localization_priority: Normal
ms.openlocfilehash: 8bf36b786adbd8064ee0c00c0ce293408c6e2b7f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882315"
---
# <a name="governanceschedule-resource-type"></a><span data-ttu-id="0ea33-104">Тип ресурса governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="0ea33-104">governanceSchedule resource type</span></span>

> <span data-ttu-id="0ea33-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0ea33-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ea33-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ea33-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0ea33-107">Представляет расписание для [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="0ea33-107">Represents the schedule for a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> <span data-ttu-id="0ea33-108">Для запроса назначений ролей, расписание определяет, когда следует выполнить операцию назначения ролей, время завершения назначения ролей и как часто следует выполнить операцию назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="0ea33-108">For a role assignment request, the schedule controls when to perform the role assignment operation, when to stop the role assignment, and how frequently to do the role assignment operation.</span></span> 



## <a name="properties"></a><span data-ttu-id="0ea33-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="0ea33-109">Properties</span></span>
| <span data-ttu-id="0ea33-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ea33-110">Property</span></span>     | <span data-ttu-id="0ea33-111">Тип</span><span class="sxs-lookup"><span data-stu-id="0ea33-111">Type</span></span>   |<span data-ttu-id="0ea33-112">Описание</span><span class="sxs-lookup"><span data-stu-id="0ea33-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ea33-113">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0ea33-113">startDateTime</span></span>|<span data-ttu-id="0ea33-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ea33-114">DateTimeOffset</span></span>|<span data-ttu-id="0ea33-115">Время начала назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="0ea33-115">The start time of the role assignment.</span></span> <span data-ttu-id="0ea33-116">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="0ea33-116">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0ea33-117">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0ea33-117">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0ea33-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="0ea33-118">endDateTime</span></span>|<span data-ttu-id="0ea33-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ea33-119">DateTimeOffset</span></span>|<span data-ttu-id="0ea33-120">Время окончания назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="0ea33-120">The end time of the role assignment.</span></span> <span data-ttu-id="0ea33-121">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="0ea33-121">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0ea33-122">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0ea33-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="0ea33-123">*Примечание: Если значение равно `null`, указывает постоянное назначение.*</span><span class="sxs-lookup"><span data-stu-id="0ea33-123">*Note: if the value is `null`, it indicates a permanent assignment.*</span></span>|
|<span data-ttu-id="0ea33-124">type</span><span class="sxs-lookup"><span data-stu-id="0ea33-124">type</span></span>|<span data-ttu-id="0ea33-125">Строка</span><span class="sxs-lookup"><span data-stu-id="0ea33-125">String</span></span>|<span data-ttu-id="0ea33-126">Тип расписания назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="0ea33-126">The role assignment schedule type.</span></span> <span data-ttu-id="0ea33-127">Только `Once` поддерживается в данный момент.</span><span class="sxs-lookup"><span data-stu-id="0ea33-127">Only `Once` is supported for now.</span></span>
|<span data-ttu-id="0ea33-128">duration</span><span class="sxs-lookup"><span data-stu-id="0ea33-128">duration</span></span>|<span data-ttu-id="0ea33-129">Продолжительность</span><span class="sxs-lookup"><span data-stu-id="0ea33-129">Duration</span></span>|<span data-ttu-id="0ea33-130">Длительность назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="0ea33-130">The duration of a role assignment.</span></span> <span data-ttu-id="0ea33-131">Это в формате интервал времени.</span><span class="sxs-lookup"><span data-stu-id="0ea33-131">It is in format of a TimeSpan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0ea33-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0ea33-132">JSON representation</span></span>

<span data-ttu-id="0ea33-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ea33-133">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "governanceSchedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
