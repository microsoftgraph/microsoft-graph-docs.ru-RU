---
title: тип ресурса синхронизацииSchedule
description: Определяет расписание, используемую для запуска синхронизацииJob.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 3d0b0a45515be459c436d24f8427f7b84ef1419f
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722064"
---
# <a name="synchronizationschedule-resource-type"></a><span data-ttu-id="526dd-103">тип ресурса синхронизацииSchedule</span><span class="sxs-lookup"><span data-stu-id="526dd-103">synchronizationSchedule resource type</span></span>

<span data-ttu-id="526dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="526dd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="526dd-105">Определяет расписание, используемую для запуска [синхронизацииJob.](synchronization-synchronizationjob.md)</span><span class="sxs-lookup"><span data-stu-id="526dd-105">Defines the schedule used to run a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="526dd-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="526dd-106">Properties</span></span>
| <span data-ttu-id="526dd-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="526dd-107">Property</span></span>     | <span data-ttu-id="526dd-108">Тип</span><span class="sxs-lookup"><span data-stu-id="526dd-108">Type</span></span>   |<span data-ttu-id="526dd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="526dd-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="526dd-110">истечение срока действия</span><span class="sxs-lookup"><span data-stu-id="526dd-110">expiration</span></span>|<span data-ttu-id="526dd-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="526dd-111">DateTimeOffset</span></span>|<span data-ttu-id="526dd-112">Дата и время истечения срока действия этого задания.</span><span class="sxs-lookup"><span data-stu-id="526dd-112">Date and time when this job will expire.</span></span> <span data-ttu-id="526dd-113">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="526dd-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="526dd-114">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="526dd-114">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="526dd-115">interval</span><span class="sxs-lookup"><span data-stu-id="526dd-115">interval</span></span>|<span data-ttu-id="526dd-116">Duration</span><span class="sxs-lookup"><span data-stu-id="526dd-116">Duration</span></span>|<span data-ttu-id="526dd-117">Интервал между итерациями синхронизации.</span><span class="sxs-lookup"><span data-stu-id="526dd-117">The interval between synchronization iterations.</span></span>|
|<span data-ttu-id="526dd-118">state</span><span class="sxs-lookup"><span data-stu-id="526dd-118">state</span></span>|<span data-ttu-id="526dd-119">String</span><span class="sxs-lookup"><span data-stu-id="526dd-119">String</span></span>| <span data-ttu-id="526dd-120">Возможные значения: `Active`, `Disabled`.</span><span class="sxs-lookup"><span data-stu-id="526dd-120">Possible values are: `Active`, `Disabled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="526dd-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="526dd-121">JSON representation</span></span>

<span data-ttu-id="526dd-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="526dd-122">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationSchedule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


