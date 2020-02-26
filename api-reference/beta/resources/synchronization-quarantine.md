---
title: Тип ресурса Синчронизатионкуарантине
description: Предоставляет сведения о состоянии карантина Синчронизатионжоб.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d5e36d62c26225a3dda5fe0adb4610c56c226b79
ms.sourcegitcommit: d419565add1f731be50c9b5911eb1310fa007097
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2020
ms.locfileid: "42280703"
---
# <a name="synchronizationquarantine-resource-type"></a><span data-ttu-id="4999a-103">Тип ресурса Синчронизатионкуарантине</span><span class="sxs-lookup"><span data-stu-id="4999a-103">synchronizationQuarantine resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4999a-104">Предоставляет сведения о состоянии карантина [синчронизатионжоб](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="4999a-104">Provides information about the quarantine state of a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4999a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="4999a-105">Properties</span></span>
| <span data-ttu-id="4999a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="4999a-106">Property</span></span>     | <span data-ttu-id="4999a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="4999a-107">Type</span></span>   |<span data-ttu-id="4999a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4999a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4999a-109">куррентбеган</span><span class="sxs-lookup"><span data-stu-id="4999a-109">currentBegan</span></span>|<span data-ttu-id="4999a-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4999a-110">DateTimeOffset</span></span>|<span data-ttu-id="4999a-111">Дата и время последнего вычисления и ликвидации карантина.</span><span class="sxs-lookup"><span data-stu-id="4999a-111">Date and time when the quarantine was last evaluated and imposed.</span></span> <span data-ttu-id="4999a-112">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="4999a-112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4999a-113">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="4999a-113">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="4999a-114">некстаттемпт</span><span class="sxs-lookup"><span data-stu-id="4999a-114">nextAttempt</span></span>|<span data-ttu-id="4999a-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4999a-115">DateTimeOffset</span></span>|<span data-ttu-id="4999a-116">Дата и время следующей попытки повторной оценки карантина.</span><span class="sxs-lookup"><span data-stu-id="4999a-116">Date and time when the next attempt to re-evaluate the quarantine will be made.</span></span> <span data-ttu-id="4999a-117">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="4999a-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4999a-118">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="4999a-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="4999a-119">reason</span><span class="sxs-lookup"><span data-stu-id="4999a-119">reason</span></span>|<span data-ttu-id="4999a-120">String</span><span class="sxs-lookup"><span data-stu-id="4999a-120">String</span></span>|<span data-ttu-id="4999a-121">Код, обозначающий, почему был наложен карантин.</span><span class="sxs-lookup"><span data-stu-id="4999a-121">A code that signifies why the quarantine was imposed.</span></span> <span data-ttu-id="4999a-122">Возможные значения: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `QuarantinedOnDemand`, `TooManyDeletes`, `Unknown`.</span><span class="sxs-lookup"><span data-stu-id="4999a-122">Possible values are: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `QuarantinedOnDemand`, `TooManyDeletes`, `Unknown`.</span></span>|
|<span data-ttu-id="4999a-123">сериесбеган</span><span class="sxs-lookup"><span data-stu-id="4999a-123">seriesBegan</span></span>|<span data-ttu-id="4999a-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4999a-124">DateTimeOffset</span></span>|<span data-ttu-id="4999a-125">Дата и время первого помещения карантина в этот цикл (ряд начинается при первом включении карантина и сбрасывается, как только будет ликвидируется карантин).</span><span class="sxs-lookup"><span data-stu-id="4999a-125">Date and time when the quarantine was first imposed in this series (a series starts when a quarantine is first imposed, and is reset as soon as the quarantine is lifted).</span></span> <span data-ttu-id="4999a-126">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="4999a-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4999a-127">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="4999a-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="4999a-128">сериескаунт</span><span class="sxs-lookup"><span data-stu-id="4999a-128">seriesCount</span></span>|<span data-ttu-id="4999a-129">Int64</span><span class="sxs-lookup"><span data-stu-id="4999a-129">Int64</span></span>|<span data-ttu-id="4999a-130">Количество повторных попыток вычисления и вступления в действия карантина для этой серии (ряд начинается при первом включении карантина и сбрасывается, как только приликвидируется карантин).</span><span class="sxs-lookup"><span data-stu-id="4999a-130">Number of times in this series the quarantine was re-evaluated and left in effect (a series starts when quarantine is first imposed, and is reset as soon as quarantine is lifted).</span></span>|
|<span data-ttu-id="4999a-131">error</span><span class="sxs-lookup"><span data-stu-id="4999a-131">error</span></span>|[<span data-ttu-id="4999a-132">синчронизатионеррор</span><span class="sxs-lookup"><span data-stu-id="4999a-132">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="4999a-133">Описывает ошибки, которые произошли при переводе задания синхронизации в карантин.</span><span class="sxs-lookup"><span data-stu-id="4999a-133">Describes the error(s) that occurred when putting the synchronization job into quarantine.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4999a-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4999a-134">JSON representation</span></span>

<span data-ttu-id="4999a-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4999a-135">The following is a JSON representation of the resource.</span></span>

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
