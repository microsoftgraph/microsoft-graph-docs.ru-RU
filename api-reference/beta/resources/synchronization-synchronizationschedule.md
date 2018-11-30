---
title: Тип ресурса synchronizationSchedule
description: Определяет расписание, используемая для запуска synchronizationJob.
ms.openlocfilehash: c0435b3957f138751f34a1e0e522683b352294da
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078568"
---
# <a name="synchronizationschedule-resource-type"></a><span data-ttu-id="ee479-103">Тип ресурса synchronizationSchedule</span><span class="sxs-lookup"><span data-stu-id="ee479-103">synchronizationSchedule resource type</span></span>

> <span data-ttu-id="ee479-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ee479-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ee479-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee479-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ee479-106">Определяет расписание, используемая для запуска [synchronizationJob](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="ee479-106">Defines the schedule used to run a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ee479-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ee479-107">Properties</span></span>
| <span data-ttu-id="ee479-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee479-108">Property</span></span>     | <span data-ttu-id="ee479-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ee479-109">Type</span></span>   |<span data-ttu-id="ee479-110">Description</span><span class="sxs-lookup"><span data-stu-id="ee479-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee479-111">истечение срока действия</span><span class="sxs-lookup"><span data-stu-id="ee479-111">expiration</span></span>|<span data-ttu-id="ee479-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee479-112">DateTimeOffset</span></span>|<span data-ttu-id="ee479-113">Дата и время истечения срока действия этого задания.</span><span class="sxs-lookup"><span data-stu-id="ee479-113">Date and time when this job will expire.</span></span> <span data-ttu-id="ee479-114">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="ee479-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ee479-115">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="ee479-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="ee479-116">interval</span><span class="sxs-lookup"><span data-stu-id="ee479-116">interval</span></span>|<span data-ttu-id="ee479-117">Продолжительность</span><span class="sxs-lookup"><span data-stu-id="ee479-117">Duration</span></span>|<span data-ttu-id="ee479-118">Интервал между итерациями синхронизации.</span><span class="sxs-lookup"><span data-stu-id="ee479-118">The interval between synchronization iterations.</span></span>|
|<span data-ttu-id="ee479-119">state</span><span class="sxs-lookup"><span data-stu-id="ee479-119">state</span></span>|<span data-ttu-id="ee479-120">String</span><span class="sxs-lookup"><span data-stu-id="ee479-120">String</span></span>| <span data-ttu-id="ee479-121">Возможные значения: `Active`, `Disabled`.</span><span class="sxs-lookup"><span data-stu-id="ee479-121">Possible values are: `Active`, `Disabled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ee479-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ee479-122">JSON representation</span></span>

<span data-ttu-id="ee479-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee479-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationSchedule"
}-->

```json
{
  "expiration": "String (timestamp)",
  "interval": "String (duration)",
  "state": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSchedule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->