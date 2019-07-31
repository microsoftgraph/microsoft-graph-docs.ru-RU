---
title: Тип ресурса Синчронизатионсчедуле
description: Определяет расписание, используемое для запуска Синчронизатионжоб.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5ffbc327d40edb071c70336032506b5f97c9e083
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964629"
---
# <a name="synchronizationschedule-resource-type"></a><span data-ttu-id="d0c38-103">Тип ресурса Синчронизатионсчедуле</span><span class="sxs-lookup"><span data-stu-id="d0c38-103">synchronizationSchedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0c38-104">Определяет расписание, используемое для запуска [синчронизатионжоб](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="d0c38-104">Defines the schedule used to run a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d0c38-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d0c38-105">Properties</span></span>
| <span data-ttu-id="d0c38-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0c38-106">Property</span></span>     | <span data-ttu-id="d0c38-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d0c38-107">Type</span></span>   |<span data-ttu-id="d0c38-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d0c38-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0c38-109">срока действия</span><span class="sxs-lookup"><span data-stu-id="d0c38-109">expiration</span></span>|<span data-ttu-id="d0c38-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0c38-110">DateTimeOffset</span></span>|<span data-ttu-id="d0c38-111">Дата и время истечения срока действия этого задания.</span><span class="sxs-lookup"><span data-stu-id="d0c38-111">Date and time when this job will expire.</span></span> <span data-ttu-id="d0c38-112">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="d0c38-112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d0c38-113">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d0c38-113">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="d0c38-114">interval</span><span class="sxs-lookup"><span data-stu-id="d0c38-114">interval</span></span>|<span data-ttu-id="d0c38-115">Duration (Длительность)</span><span class="sxs-lookup"><span data-stu-id="d0c38-115">Duration</span></span>|<span data-ttu-id="d0c38-116">Интервал между итерациями синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d0c38-116">The interval between synchronization iterations.</span></span>|
|<span data-ttu-id="d0c38-117">state</span><span class="sxs-lookup"><span data-stu-id="d0c38-117">state</span></span>|<span data-ttu-id="d0c38-118">String</span><span class="sxs-lookup"><span data-stu-id="d0c38-118">String</span></span>| <span data-ttu-id="d0c38-119">Возможные значения: `Active`, `Disabled`.</span><span class="sxs-lookup"><span data-stu-id="d0c38-119">Possible values are: `Active`, `Disabled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d0c38-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d0c38-120">JSON representation</span></span>

<span data-ttu-id="d0c38-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0c38-121">The following is a JSON representation of the resource.</span></span>

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
