---
title: Тип ресурса Говернанцесчедуле
description: 'Представляет расписание для объекта governanceRoleAssignmentRequest. Для запроса на назначение роли расписание определяет, когда следует выполнять операцию назначения роли, когда следует остановить назначение роли и как часто выполняется операция назначения роли. '
localization_priority: Normal
ms.openlocfilehash: d7ccfe74804166ad2204ea02c072d79341cf75e7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506456"
---
# <a name="governanceschedule-resource-type"></a><span data-ttu-id="b390f-104">Тип ресурса Говернанцесчедуле</span><span class="sxs-lookup"><span data-stu-id="b390f-104">governanceSchedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b390f-105">Представляет расписание для объекта [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="b390f-105">Represents the schedule for a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> <span data-ttu-id="b390f-106">Для запроса на назначение роли расписание определяет, когда следует выполнять операцию назначения роли, когда следует остановить назначение роли и как часто выполняется операция назначения роли.</span><span class="sxs-lookup"><span data-stu-id="b390f-106">For a role assignment request, the schedule controls when to perform the role assignment operation, when to stop the role assignment, and how frequently to do the role assignment operation.</span></span> 



## <a name="properties"></a><span data-ttu-id="b390f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b390f-107">Properties</span></span>
| <span data-ttu-id="b390f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b390f-108">Property</span></span>     | <span data-ttu-id="b390f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b390f-109">Type</span></span>   |<span data-ttu-id="b390f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b390f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b390f-111">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b390f-111">startDateTime</span></span>|<span data-ttu-id="b390f-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b390f-112">DateTimeOffset</span></span>|<span data-ttu-id="b390f-113">Время начала назначения роли.</span><span class="sxs-lookup"><span data-stu-id="b390f-113">The start time of the role assignment.</span></span> <span data-ttu-id="b390f-114">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="b390f-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b390f-115">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b390f-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b390f-116">endDateTime</span><span class="sxs-lookup"><span data-stu-id="b390f-116">endDateTime</span></span>|<span data-ttu-id="b390f-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b390f-117">DateTimeOffset</span></span>|<span data-ttu-id="b390f-118">Время окончания назначения роли.</span><span class="sxs-lookup"><span data-stu-id="b390f-118">The end time of the role assignment.</span></span> <span data-ttu-id="b390f-119">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="b390f-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b390f-120">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b390f-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="b390f-121">*Note: Если значение задано `null`, оно указывает на постоянное назначение.*</span><span class="sxs-lookup"><span data-stu-id="b390f-121">*Note: if the value is `null`, it indicates a permanent assignment.*</span></span>|
|<span data-ttu-id="b390f-122">type</span><span class="sxs-lookup"><span data-stu-id="b390f-122">type</span></span>|<span data-ttu-id="b390f-123">String</span><span class="sxs-lookup"><span data-stu-id="b390f-123">String</span></span>|<span data-ttu-id="b390f-124">Тип расписания назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="b390f-124">The role assignment schedule type.</span></span> <span data-ttu-id="b390f-125">Поддерживается `Once` только в настоящее время.</span><span class="sxs-lookup"><span data-stu-id="b390f-125">Only `Once` is supported for now.</span></span>
|<span data-ttu-id="b390f-126">duration</span><span class="sxs-lookup"><span data-stu-id="b390f-126">duration</span></span>|<span data-ttu-id="b390f-127">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="b390f-127">Duration</span></span>|<span data-ttu-id="b390f-128">Продолжительность назначения роли.</span><span class="sxs-lookup"><span data-stu-id="b390f-128">The duration of a role assignment.</span></span> <span data-ttu-id="b390f-129">Он имеет формат TimeSpan.</span><span class="sxs-lookup"><span data-stu-id="b390f-129">It is in format of a TimeSpan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b390f-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b390f-130">JSON representation</span></span>

<span data-ttu-id="b390f-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b390f-131">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceschedule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
