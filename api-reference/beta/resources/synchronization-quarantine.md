---
title: Тип ресурса synchronizationQuarantine
description: Предоставляет информацию о состоянии карантина synchronizationJob.
localization_priority: Normal
ms.openlocfilehash: fba0077d48e69ed4c2c190d0b50a6fcfc1749626
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849730"
---
# <a name="synchronizationquarantine-resource-type"></a><span data-ttu-id="58887-103">Тип ресурса synchronizationQuarantine</span><span class="sxs-lookup"><span data-stu-id="58887-103">synchronizationQuarantine resource type</span></span>

> <span data-ttu-id="58887-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="58887-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="58887-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58887-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="58887-106">Предоставляет информацию о состоянии карантина [synchronizationJob](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="58887-106">Provides information about the quarantine state of a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="58887-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="58887-107">Properties</span></span>
| <span data-ttu-id="58887-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="58887-108">Property</span></span>     | <span data-ttu-id="58887-109">Тип</span><span class="sxs-lookup"><span data-stu-id="58887-109">Type</span></span>   |<span data-ttu-id="58887-110">Описание</span><span class="sxs-lookup"><span data-stu-id="58887-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58887-111">currentBegan</span><span class="sxs-lookup"><span data-stu-id="58887-111">currentBegan</span></span>|<span data-ttu-id="58887-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58887-112">DateTimeOffset</span></span>|<span data-ttu-id="58887-113">Дата и время последнего карантина вычисляется и накладываемого.</span><span class="sxs-lookup"><span data-stu-id="58887-113">Date and time when the quarantine was last evaluated and imposed.</span></span> <span data-ttu-id="58887-114">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="58887-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="58887-115">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="58887-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="58887-116">nextAttempt</span><span class="sxs-lookup"><span data-stu-id="58887-116">nextAttempt</span></span>|<span data-ttu-id="58887-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58887-117">DateTimeOffset</span></span>|<span data-ttu-id="58887-118">Дата и время, станут при следующей попытке выполните повторную оценку на карантин.</span><span class="sxs-lookup"><span data-stu-id="58887-118">Date and time when the next attempt to re-evaluate the quarantine will be made.</span></span> <span data-ttu-id="58887-119">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="58887-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="58887-120">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="58887-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="58887-121">Причина</span><span class="sxs-lookup"><span data-stu-id="58887-121">reason</span></span>|<span data-ttu-id="58887-122">Строка</span><span class="sxs-lookup"><span data-stu-id="58887-122">String</span></span>|<span data-ttu-id="58887-123">Код, который обозначает зачем накладываемого карантина.</span><span class="sxs-lookup"><span data-stu-id="58887-123">A code that signifies why the quarantine was imposed.</span></span> <span data-ttu-id="58887-124">Возможные значения: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `Unknown`.</span><span class="sxs-lookup"><span data-stu-id="58887-124">Possible values are: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `Unknown`.</span></span>|
|<span data-ttu-id="58887-125">seriesBegan</span><span class="sxs-lookup"><span data-stu-id="58887-125">seriesBegan</span></span>|<span data-ttu-id="58887-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58887-126">DateTimeOffset</span></span>|<span data-ttu-id="58887-127">Дата и время, когда карантина был сначала установленных в этой серии (серии запускается при карантина сначала накладываемого и сброс сразу же удален карантина).</span><span class="sxs-lookup"><span data-stu-id="58887-127">Date and time when the quarantine was first imposed in this series (a series starts when a quarantine is first imposed, and is reset as soon as the quarantine is lifted).</span></span> <span data-ttu-id="58887-128">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="58887-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="58887-129">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="58887-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="58887-130">seriesCount</span><span class="sxs-lookup"><span data-stu-id="58887-130">seriesCount</span></span>|<span data-ttu-id="58887-131">Int64</span><span class="sxs-lookup"><span data-stu-id="58887-131">Int64</span></span>|<span data-ttu-id="58887-132">Сколько раз в этой серии карантина было повторно вычисляется и фактически слева (серии запускается при карантина сначала накладываемого и сброс сразу же удален карантин).</span><span class="sxs-lookup"><span data-stu-id="58887-132">Number of times in this series the quarantine was re-evaluated and left in effect (a series starts when quarantine is first imposed, and is reset as soon as quarantine is lifted).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="58887-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="58887-133">JSON representation</span></span>

<span data-ttu-id="58887-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58887-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationQuarantine"
}-->

```json
{
  "currentBegan": "String (timestamp)",
  "nextAttempt": "String (timestamp)",
  "reason": "String",
  "seriesBegan": "String (timestamp)",
  "seriesCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationQuarantine resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
