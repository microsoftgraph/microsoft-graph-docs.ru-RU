---
title: тип ресурса synchronizationQuarantine
description: Предоставляет сведения о состоянии карантина синхронизацииJob.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 45381594a242251995de3d43bb7fd02e0638484b
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720503"
---
# <a name="synchronizationquarantine-resource-type"></a><span data-ttu-id="fd9f1-103">тип ресурса synchronizationQuarantine</span><span class="sxs-lookup"><span data-stu-id="fd9f1-103">synchronizationQuarantine resource type</span></span>

<span data-ttu-id="fd9f1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd9f1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd9f1-105">Предоставляет сведения о состоянии карантина [синхронизацииJob.](synchronization-synchronizationjob.md)</span><span class="sxs-lookup"><span data-stu-id="fd9f1-105">Provides information about the quarantine state of a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="fd9f1-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="fd9f1-106">Properties</span></span>
| <span data-ttu-id="fd9f1-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd9f1-107">Property</span></span>     | <span data-ttu-id="fd9f1-108">Тип</span><span class="sxs-lookup"><span data-stu-id="fd9f1-108">Type</span></span>   |<span data-ttu-id="fd9f1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fd9f1-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd9f1-110">currentBegan</span><span class="sxs-lookup"><span data-stu-id="fd9f1-110">currentBegan</span></span>|<span data-ttu-id="fd9f1-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd9f1-111">DateTimeOffset</span></span>|<span data-ttu-id="fd9f1-112">Дата и время последней оценки и введения карантина.</span><span class="sxs-lookup"><span data-stu-id="fd9f1-112">Date and time when the quarantine was last evaluated and imposed.</span></span> <span data-ttu-id="fd9f1-113">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="fd9f1-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fd9f1-114">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="fd9f1-114">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="fd9f1-115">nextAttempt</span><span class="sxs-lookup"><span data-stu-id="fd9f1-115">nextAttempt</span></span>|<span data-ttu-id="fd9f1-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd9f1-116">DateTimeOffset</span></span>|<span data-ttu-id="fd9f1-117">Дата и время, когда будет предпринята следующая попытка повторной оценки карантина.</span><span class="sxs-lookup"><span data-stu-id="fd9f1-117">Date and time when the next attempt to re-evaluate the quarantine will be made.</span></span> <span data-ttu-id="fd9f1-118">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="fd9f1-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fd9f1-119">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="fd9f1-119">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="fd9f1-120">reason</span><span class="sxs-lookup"><span data-stu-id="fd9f1-120">reason</span></span>|<span data-ttu-id="fd9f1-121">String</span><span class="sxs-lookup"><span data-stu-id="fd9f1-121">String</span></span>|<span data-ttu-id="fd9f1-122">Код, который означает, почему был введен карантин.</span><span class="sxs-lookup"><span data-stu-id="fd9f1-122">A code that signifies why the quarantine was imposed.</span></span> <span data-ttu-id="fd9f1-123">Возможные значения: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `QuarantinedOnDemand`, `TooManyDeletes`, `Unknown`.</span><span class="sxs-lookup"><span data-stu-id="fd9f1-123">Possible values are: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `QuarantinedOnDemand`, `TooManyDeletes`, `Unknown`.</span></span>|
|<span data-ttu-id="fd9f1-124">seriesBegan</span><span class="sxs-lookup"><span data-stu-id="fd9f1-124">seriesBegan</span></span>|<span data-ttu-id="fd9f1-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd9f1-125">DateTimeOffset</span></span>|<span data-ttu-id="fd9f1-126">Дата и время, когда карантин был впервые введен в этой серии (серия начинается при первом введении карантина и сбрасывается, как только карантин отменяется).</span><span class="sxs-lookup"><span data-stu-id="fd9f1-126">Date and time when the quarantine was first imposed in this series (a series starts when a quarantine is first imposed, and is reset as soon as the quarantine is lifted).</span></span> <span data-ttu-id="fd9f1-127">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="fd9f1-127">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fd9f1-128">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="fd9f1-128">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="fd9f1-129">seriesCount</span><span class="sxs-lookup"><span data-stu-id="fd9f1-129">seriesCount</span></span>|<span data-ttu-id="fd9f1-130">Int64</span><span class="sxs-lookup"><span data-stu-id="fd9f1-130">Int64</span></span>|<span data-ttu-id="fd9f1-131">Количество раз в этой серии карантин был повторно оценен и оставлен в силе (серия начинается при первом введении карантина и сбрасывается, как только карантин отменяется).</span><span class="sxs-lookup"><span data-stu-id="fd9f1-131">Number of times in this series the quarantine was re-evaluated and left in effect (a series starts when quarantine is first imposed, and is reset as soon as quarantine is lifted).</span></span>|
|<span data-ttu-id="fd9f1-132">error</span><span class="sxs-lookup"><span data-stu-id="fd9f1-132">error</span></span>|[<span data-ttu-id="fd9f1-133">синхронизацияError</span><span class="sxs-lookup"><span data-stu-id="fd9f1-133">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="fd9f1-134">Описывает ошибку(ы), которая произошла при вводе задания синхронизации в карантин.</span><span class="sxs-lookup"><span data-stu-id="fd9f1-134">Describes the error(s) that occurred when putting the synchronization job into quarantine.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fd9f1-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fd9f1-135">JSON representation</span></span>

<span data-ttu-id="fd9f1-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fd9f1-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationQuarantine"
}-->

```json
{
  "error": {"@odata.type": "microsoft.graph.synchronizationError"},
  "currentBegan": "String (timestamp)",
  "nextAttempt": "String (timestamp)",
  "reason": "String",
  "seriesBegan": "String (timestamp)",
  "seriesCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationQuarantine resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


