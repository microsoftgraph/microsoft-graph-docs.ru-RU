---
title: Тип ресурса governanceSchedule
description: 'Представляет расписание для governanceRoleAssignmentRequest. Для запроса назначений ролей, расписание определяет, когда следует выполнить операцию назначения ролей, время завершения назначения ролей и как часто следует выполнить операцию назначения ролей. '
localization_priority: Normal
ms.openlocfilehash: 11ac010829309c9b701e20da8ad40ebf905e02ba
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575253"
---
# <a name="microsoftgraphgovernanceschedule-resource-type"></a><span data-ttu-id="28484-104">Тип ресурса microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="28484-104">microsoft.graph.governanceSchedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28484-105">Представляет расписание для [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="28484-105">Represents the schedule for a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> <span data-ttu-id="28484-106">Для запроса назначений ролей, расписание определяет, когда следует выполнить операцию назначения ролей, время завершения назначения ролей и как часто следует выполнить операцию назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="28484-106">For a role assignment request, the schedule controls when to perform the role assignment operation, when to stop the role assignment, and how frequently to do the role assignment operation.</span></span> 



## <a name="properties"></a><span data-ttu-id="28484-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="28484-107">Properties</span></span>
| <span data-ttu-id="28484-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="28484-108">Property</span></span>     | <span data-ttu-id="28484-109">Тип</span><span class="sxs-lookup"><span data-stu-id="28484-109">Type</span></span>   |<span data-ttu-id="28484-110">Описание</span><span class="sxs-lookup"><span data-stu-id="28484-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28484-111">startDateTime</span><span class="sxs-lookup"><span data-stu-id="28484-111">startDateTime</span></span>|<span data-ttu-id="28484-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28484-112">DateTimeOffset</span></span>|<span data-ttu-id="28484-113">Время начала назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="28484-113">The start time of the role assignment.</span></span> <span data-ttu-id="28484-114">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="28484-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="28484-115">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="28484-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="28484-116">endDateTime</span><span class="sxs-lookup"><span data-stu-id="28484-116">endDateTime</span></span>|<span data-ttu-id="28484-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28484-117">DateTimeOffset</span></span>|<span data-ttu-id="28484-118">Время окончания назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="28484-118">The end time of the role assignment.</span></span> <span data-ttu-id="28484-119">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="28484-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="28484-120">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="28484-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="28484-121">*Примечание: Если значение равно `null`, указывает постоянное назначение.*</span><span class="sxs-lookup"><span data-stu-id="28484-121">*Note: if the value is `null`, it indicates a permanent assignment.*</span></span>|
|<span data-ttu-id="28484-122">type</span><span class="sxs-lookup"><span data-stu-id="28484-122">type</span></span>|<span data-ttu-id="28484-123">Строка</span><span class="sxs-lookup"><span data-stu-id="28484-123">String</span></span>|<span data-ttu-id="28484-124">Тип расписания назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="28484-124">The role assignment schedule type.</span></span> <span data-ttu-id="28484-125">Только `Once` поддерживается в данный момент.</span><span class="sxs-lookup"><span data-stu-id="28484-125">Only `Once` is supported for now.</span></span>
|<span data-ttu-id="28484-126">duration</span><span class="sxs-lookup"><span data-stu-id="28484-126">duration</span></span>|<span data-ttu-id="28484-127">Длительность</span><span class="sxs-lookup"><span data-stu-id="28484-127">Duration</span></span>|<span data-ttu-id="28484-128">Длительность назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="28484-128">The duration of a role assignment.</span></span> <span data-ttu-id="28484-129">Это в формате интервал времени.</span><span class="sxs-lookup"><span data-stu-id="28484-129">It is in format of a TimeSpan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="28484-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="28484-130">JSON representation</span></span>

<span data-ttu-id="28484-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28484-131">Here is a JSON representation of the resource.</span></span>

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
