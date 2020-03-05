---
title: Тип ресурса Синчронизатионсчедуле
description: Определяет расписание, используемое для запуска Синчронизатионжоб.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dc34a596af9b8f1270462b7c180e62ffde0cf0f0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520046"
---
# <a name="synchronizationschedule-resource-type"></a><span data-ttu-id="fe237-103">Тип ресурса Синчронизатионсчедуле</span><span class="sxs-lookup"><span data-stu-id="fe237-103">synchronizationSchedule resource type</span></span>

<span data-ttu-id="fe237-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fe237-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe237-105">Определяет расписание, используемое для запуска [синчронизатионжоб](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="fe237-105">Defines the schedule used to run a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="fe237-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="fe237-106">Properties</span></span>
| <span data-ttu-id="fe237-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe237-107">Property</span></span>     | <span data-ttu-id="fe237-108">Тип</span><span class="sxs-lookup"><span data-stu-id="fe237-108">Type</span></span>   |<span data-ttu-id="fe237-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fe237-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe237-110">срока действия</span><span class="sxs-lookup"><span data-stu-id="fe237-110">expiration</span></span>|<span data-ttu-id="fe237-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe237-111">DateTimeOffset</span></span>|<span data-ttu-id="fe237-112">Дата и время истечения срока действия этого задания.</span><span class="sxs-lookup"><span data-stu-id="fe237-112">Date and time when this job will expire.</span></span> <span data-ttu-id="fe237-113">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="fe237-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fe237-114">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="fe237-114">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="fe237-115">interval</span><span class="sxs-lookup"><span data-stu-id="fe237-115">interval</span></span>|<span data-ttu-id="fe237-116">Длительность</span><span class="sxs-lookup"><span data-stu-id="fe237-116">Duration</span></span>|<span data-ttu-id="fe237-117">Интервал между итерациями синхронизации.</span><span class="sxs-lookup"><span data-stu-id="fe237-117">The interval between synchronization iterations.</span></span>|
|<span data-ttu-id="fe237-118">state</span><span class="sxs-lookup"><span data-stu-id="fe237-118">state</span></span>|<span data-ttu-id="fe237-119">String</span><span class="sxs-lookup"><span data-stu-id="fe237-119">String</span></span>| <span data-ttu-id="fe237-120">Возможные значения: `Active`, `Disabled`.</span><span class="sxs-lookup"><span data-stu-id="fe237-120">Possible values are: `Active`, `Disabled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fe237-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fe237-121">JSON representation</span></span>

<span data-ttu-id="fe237-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe237-122">The following is a JSON representation of the resource.</span></span>

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
