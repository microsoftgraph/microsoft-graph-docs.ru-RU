---
title: Тип ресурса Синчронизатионсчедуле
description: Определяет расписание, используемое для запуска Синчронизатионжоб.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 70b44acb7f00e55bf4082ac064950e819cb33f2f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046743"
---
# <a name="synchronizationschedule-resource-type"></a><span data-ttu-id="d3e43-103">Тип ресурса Синчронизатионсчедуле</span><span class="sxs-lookup"><span data-stu-id="d3e43-103">synchronizationSchedule resource type</span></span>

<span data-ttu-id="d3e43-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3e43-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3e43-105">Определяет расписание, используемое для запуска [синчронизатионжоб](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="d3e43-105">Defines the schedule used to run a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d3e43-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d3e43-106">Properties</span></span>
| <span data-ttu-id="d3e43-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3e43-107">Property</span></span>     | <span data-ttu-id="d3e43-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d3e43-108">Type</span></span>   |<span data-ttu-id="d3e43-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d3e43-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3e43-110">срока действия</span><span class="sxs-lookup"><span data-stu-id="d3e43-110">expiration</span></span>|<span data-ttu-id="d3e43-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3e43-111">DateTimeOffset</span></span>|<span data-ttu-id="d3e43-112">Дата и время истечения срока действия этого задания.</span><span class="sxs-lookup"><span data-stu-id="d3e43-112">Date and time when this job will expire.</span></span> <span data-ttu-id="d3e43-113">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="d3e43-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d3e43-114">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d3e43-114">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="d3e43-115">interval</span><span class="sxs-lookup"><span data-stu-id="d3e43-115">interval</span></span>|<span data-ttu-id="d3e43-116">Длительность</span><span class="sxs-lookup"><span data-stu-id="d3e43-116">Duration</span></span>|<span data-ttu-id="d3e43-117">Интервал между итерациями синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d3e43-117">The interval between synchronization iterations.</span></span>|
|<span data-ttu-id="d3e43-118">state</span><span class="sxs-lookup"><span data-stu-id="d3e43-118">state</span></span>|<span data-ttu-id="d3e43-119">String</span><span class="sxs-lookup"><span data-stu-id="d3e43-119">String</span></span>| <span data-ttu-id="d3e43-120">Возможные значения: `Active`, `Disabled`.</span><span class="sxs-lookup"><span data-stu-id="d3e43-120">Possible values are: `Active`, `Disabled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d3e43-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d3e43-121">JSON representation</span></span>

<span data-ttu-id="d3e43-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3e43-122">The following is a JSON representation of the resource.</span></span>

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


