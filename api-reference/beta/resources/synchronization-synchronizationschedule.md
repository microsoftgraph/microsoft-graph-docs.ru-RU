---
title: Тип ресурса synchronizationSchedule
description: Определяет расписание, используемую для запуска synchronizationJob.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: cce48886fd461e52647fc342d707f5d97676faae
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133373"
---
# <a name="synchronizationschedule-resource-type"></a><span data-ttu-id="3c312-103">Тип ресурса synchronizationSchedule</span><span class="sxs-lookup"><span data-stu-id="3c312-103">synchronizationSchedule resource type</span></span>

<span data-ttu-id="3c312-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c312-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c312-105">Определяет расписание, используемую для запуска [synchronizationJob.](synchronization-synchronizationjob.md)</span><span class="sxs-lookup"><span data-stu-id="3c312-105">Defines the schedule used to run a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3c312-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3c312-106">Properties</span></span>
| <span data-ttu-id="3c312-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c312-107">Property</span></span>     | <span data-ttu-id="3c312-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3c312-108">Type</span></span>   |<span data-ttu-id="3c312-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3c312-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c312-110">expiration</span><span class="sxs-lookup"><span data-stu-id="3c312-110">expiration</span></span>|<span data-ttu-id="3c312-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c312-111">DateTimeOffset</span></span>|<span data-ttu-id="3c312-112">Дата и время окончания срока действия задания.</span><span class="sxs-lookup"><span data-stu-id="3c312-112">Date and time when this job will expire.</span></span> <span data-ttu-id="3c312-113">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="3c312-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3c312-114">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3c312-114">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="3c312-115">interval</span><span class="sxs-lookup"><span data-stu-id="3c312-115">interval</span></span>|<span data-ttu-id="3c312-116">Duration</span><span class="sxs-lookup"><span data-stu-id="3c312-116">Duration</span></span>|<span data-ttu-id="3c312-117">Интервал между итерациями синхронизации.</span><span class="sxs-lookup"><span data-stu-id="3c312-117">The interval between synchronization iterations.</span></span>|
|<span data-ttu-id="3c312-118">state</span><span class="sxs-lookup"><span data-stu-id="3c312-118">state</span></span>|<span data-ttu-id="3c312-119">String</span><span class="sxs-lookup"><span data-stu-id="3c312-119">String</span></span>| <span data-ttu-id="3c312-120">Возможные значения: `Active`, `Disabled`.</span><span class="sxs-lookup"><span data-stu-id="3c312-120">Possible values are: `Active`, `Disabled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3c312-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3c312-121">JSON representation</span></span>

<span data-ttu-id="3c312-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3c312-122">The following is a JSON representation of the resource.</span></span>

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


