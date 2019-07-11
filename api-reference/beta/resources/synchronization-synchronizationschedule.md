---
title: Тип ресурса Синчронизатионсчедуле
description: Определяет расписание, используемое для запуска Синчронизатионжоб.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f6802f6a5a17de53ec070621c87d077dd1b45f87
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620705"
---
# <a name="synchronizationschedule-resource-type"></a><span data-ttu-id="47578-103">Тип ресурса Синчронизатионсчедуле</span><span class="sxs-lookup"><span data-stu-id="47578-103">synchronizationSchedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47578-104">Определяет расписание, используемое для запуска [синчронизатионжоб](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="47578-104">Defines the schedule used to run a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="47578-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="47578-105">Properties</span></span>
| <span data-ttu-id="47578-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="47578-106">Property</span></span>     | <span data-ttu-id="47578-107">Тип</span><span class="sxs-lookup"><span data-stu-id="47578-107">Type</span></span>   |<span data-ttu-id="47578-108">Описание</span><span class="sxs-lookup"><span data-stu-id="47578-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47578-109">срока действия</span><span class="sxs-lookup"><span data-stu-id="47578-109">expiration</span></span>|<span data-ttu-id="47578-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47578-110">DateTimeOffset</span></span>|<span data-ttu-id="47578-111">Дата и время истечения срока действия этого задания.</span><span class="sxs-lookup"><span data-stu-id="47578-111">Date and time when this job will expire.</span></span> <span data-ttu-id="47578-112">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="47578-112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="47578-113">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="47578-113">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="47578-114">interval</span><span class="sxs-lookup"><span data-stu-id="47578-114">interval</span></span>|<span data-ttu-id="47578-115">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="47578-115">Duration</span></span>|<span data-ttu-id="47578-116">Интервал между итерациями синхронизации.</span><span class="sxs-lookup"><span data-stu-id="47578-116">The interval between synchronization iterations.</span></span>|
|<span data-ttu-id="47578-117">state</span><span class="sxs-lookup"><span data-stu-id="47578-117">state</span></span>|<span data-ttu-id="47578-118">String</span><span class="sxs-lookup"><span data-stu-id="47578-118">String</span></span>| <span data-ttu-id="47578-119">Возможные значения: `Active`, `Disabled`.</span><span class="sxs-lookup"><span data-stu-id="47578-119">Possible values are: `Active`, `Disabled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="47578-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="47578-120">JSON representation</span></span>

<span data-ttu-id="47578-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47578-121">The following is a JSON representation of the resource.</span></span>

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
