---
title: Тип ресурса Говернанцесчедуле
description: 'Представляет расписание для объекта governanceRoleAssignmentRequest. Для запроса на назначение роли расписание определяет, когда следует выполнять операцию назначения роли, когда следует остановить назначение роли и как часто выполняется операция назначения роли. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d52df62d0bed004d2126a775c44b92b5f285607f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497218"
---
# <a name="governanceschedule-resource-type"></a><span data-ttu-id="01a91-104">Тип ресурса Говернанцесчедуле</span><span class="sxs-lookup"><span data-stu-id="01a91-104">governanceSchedule resource type</span></span>

<span data-ttu-id="01a91-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01a91-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01a91-106">Представляет расписание для объекта [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="01a91-106">Represents the schedule for a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> <span data-ttu-id="01a91-107">Для запроса на назначение роли расписание определяет, когда следует выполнять операцию назначения роли, когда следует остановить назначение роли и как часто выполняется операция назначения роли.</span><span class="sxs-lookup"><span data-stu-id="01a91-107">For a role assignment request, the schedule controls when to perform the role assignment operation, when to stop the role assignment, and how frequently to do the role assignment operation.</span></span> 



## <a name="properties"></a><span data-ttu-id="01a91-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="01a91-108">Properties</span></span>
| <span data-ttu-id="01a91-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="01a91-109">Property</span></span>     | <span data-ttu-id="01a91-110">Тип</span><span class="sxs-lookup"><span data-stu-id="01a91-110">Type</span></span>   |<span data-ttu-id="01a91-111">Описание</span><span class="sxs-lookup"><span data-stu-id="01a91-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01a91-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="01a91-112">startDateTime</span></span>|<span data-ttu-id="01a91-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01a91-113">DateTimeOffset</span></span>|<span data-ttu-id="01a91-114">Время начала назначения роли.</span><span class="sxs-lookup"><span data-stu-id="01a91-114">The start time of the role assignment.</span></span> <span data-ttu-id="01a91-115">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="01a91-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="01a91-116">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="01a91-116">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="01a91-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="01a91-117">endDateTime</span></span>|<span data-ttu-id="01a91-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01a91-118">DateTimeOffset</span></span>|<span data-ttu-id="01a91-119">Время окончания назначения роли.</span><span class="sxs-lookup"><span data-stu-id="01a91-119">The end time of the role assignment.</span></span> <span data-ttu-id="01a91-120">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="01a91-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="01a91-121">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="01a91-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="01a91-122">*Note: Если значение задано `null`, оно указывает на постоянное назначение.*</span><span class="sxs-lookup"><span data-stu-id="01a91-122">*Note: if the value is `null`, it indicates a permanent assignment.*</span></span>|
|<span data-ttu-id="01a91-123">type</span><span class="sxs-lookup"><span data-stu-id="01a91-123">type</span></span>|<span data-ttu-id="01a91-124">String</span><span class="sxs-lookup"><span data-stu-id="01a91-124">String</span></span>|<span data-ttu-id="01a91-125">Тип расписания назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="01a91-125">The role assignment schedule type.</span></span> <span data-ttu-id="01a91-126">Поддерживается `Once` только в настоящее время.</span><span class="sxs-lookup"><span data-stu-id="01a91-126">Only `Once` is supported for now.</span></span>
|<span data-ttu-id="01a91-127">duration</span><span class="sxs-lookup"><span data-stu-id="01a91-127">duration</span></span>|<span data-ttu-id="01a91-128">Длительность</span><span class="sxs-lookup"><span data-stu-id="01a91-128">Duration</span></span>|<span data-ttu-id="01a91-129">Продолжительность назначения роли.</span><span class="sxs-lookup"><span data-stu-id="01a91-129">The duration of a role assignment.</span></span> <span data-ttu-id="01a91-130">Он имеет формат TimeSpan.</span><span class="sxs-lookup"><span data-stu-id="01a91-130">It is in format of a TimeSpan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="01a91-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="01a91-131">JSON representation</span></span>

<span data-ttu-id="01a91-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01a91-132">Here is a JSON representation of the resource.</span></span>

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
