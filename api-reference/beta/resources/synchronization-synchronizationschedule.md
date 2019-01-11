---
title: Тип ресурса synchronizationSchedule
description: Определяет расписание, используемая для запуска synchronizationJob.
localization_priority: Normal
ms.openlocfilehash: b59c36a36d837c21c147033dff8de66b85c863a1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877870"
---
# <a name="synchronizationschedule-resource-type"></a><span data-ttu-id="26e66-103">Тип ресурса synchronizationSchedule</span><span class="sxs-lookup"><span data-stu-id="26e66-103">synchronizationSchedule resource type</span></span>

> <span data-ttu-id="26e66-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="26e66-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="26e66-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26e66-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="26e66-106">Определяет расписание, используемая для запуска [synchronizationJob](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="26e66-106">Defines the schedule used to run a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="26e66-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="26e66-107">Properties</span></span>
| <span data-ttu-id="26e66-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="26e66-108">Property</span></span>     | <span data-ttu-id="26e66-109">Тип</span><span class="sxs-lookup"><span data-stu-id="26e66-109">Type</span></span>   |<span data-ttu-id="26e66-110">Описание</span><span class="sxs-lookup"><span data-stu-id="26e66-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26e66-111">истечение срока действия</span><span class="sxs-lookup"><span data-stu-id="26e66-111">expiration</span></span>|<span data-ttu-id="26e66-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26e66-112">DateTimeOffset</span></span>|<span data-ttu-id="26e66-113">Дата и время истечения срока действия этого задания.</span><span class="sxs-lookup"><span data-stu-id="26e66-113">Date and time when this job will expire.</span></span> <span data-ttu-id="26e66-114">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="26e66-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="26e66-115">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="26e66-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="26e66-116">interval</span><span class="sxs-lookup"><span data-stu-id="26e66-116">interval</span></span>|<span data-ttu-id="26e66-117">Продолжительность</span><span class="sxs-lookup"><span data-stu-id="26e66-117">Duration</span></span>|<span data-ttu-id="26e66-118">Интервал между итерациями синхронизации.</span><span class="sxs-lookup"><span data-stu-id="26e66-118">The interval between synchronization iterations.</span></span>|
|<span data-ttu-id="26e66-119">state</span><span class="sxs-lookup"><span data-stu-id="26e66-119">state</span></span>|<span data-ttu-id="26e66-120">String</span><span class="sxs-lookup"><span data-stu-id="26e66-120">String</span></span>| <span data-ttu-id="26e66-121">Возможные значения: `Active`, `Disabled`.</span><span class="sxs-lookup"><span data-stu-id="26e66-121">Possible values are: `Active`, `Disabled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="26e66-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="26e66-122">JSON representation</span></span>

<span data-ttu-id="26e66-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26e66-123">The following is a JSON representation of the resource.</span></span>

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
