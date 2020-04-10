---
title: Тип ресурса Синчронизатионкуарантине
description: Предоставляет сведения о состоянии карантина Синчронизатионжоб.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dd2641c7327ce0670d3b13ab05701c7da5eb0de6
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217600"
---
# <a name="synchronizationquarantine-resource-type"></a><span data-ttu-id="f7e66-103">Тип ресурса Синчронизатионкуарантине</span><span class="sxs-lookup"><span data-stu-id="f7e66-103">synchronizationQuarantine resource type</span></span>

<span data-ttu-id="f7e66-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7e66-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7e66-105">Предоставляет сведения о состоянии карантина [синчронизатионжоб](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="f7e66-105">Provides information about the quarantine state of a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f7e66-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f7e66-106">Properties</span></span>
| <span data-ttu-id="f7e66-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7e66-107">Property</span></span>     | <span data-ttu-id="f7e66-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f7e66-108">Type</span></span>   |<span data-ttu-id="f7e66-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f7e66-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7e66-110">куррентбеган</span><span class="sxs-lookup"><span data-stu-id="f7e66-110">currentBegan</span></span>|<span data-ttu-id="f7e66-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7e66-111">DateTimeOffset</span></span>|<span data-ttu-id="f7e66-112">Дата и время последнего вычисления и ликвидации карантина.</span><span class="sxs-lookup"><span data-stu-id="f7e66-112">Date and time when the quarantine was last evaluated and imposed.</span></span> <span data-ttu-id="f7e66-113">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="f7e66-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f7e66-114">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f7e66-114">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="f7e66-115">некстаттемпт</span><span class="sxs-lookup"><span data-stu-id="f7e66-115">nextAttempt</span></span>|<span data-ttu-id="f7e66-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7e66-116">DateTimeOffset</span></span>|<span data-ttu-id="f7e66-117">Дата и время следующей попытки повторной оценки карантина.</span><span class="sxs-lookup"><span data-stu-id="f7e66-117">Date and time when the next attempt to re-evaluate the quarantine will be made.</span></span> <span data-ttu-id="f7e66-118">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="f7e66-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f7e66-119">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f7e66-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="f7e66-120">reason</span><span class="sxs-lookup"><span data-stu-id="f7e66-120">reason</span></span>|<span data-ttu-id="f7e66-121">Строка</span><span class="sxs-lookup"><span data-stu-id="f7e66-121">String</span></span>|<span data-ttu-id="f7e66-122">Код, обозначающий, почему был наложен карантин.</span><span class="sxs-lookup"><span data-stu-id="f7e66-122">A code that signifies why the quarantine was imposed.</span></span> <span data-ttu-id="f7e66-123">Возможные значения: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `QuarantinedOnDemand`, `TooManyDeletes`, `Unknown`.</span><span class="sxs-lookup"><span data-stu-id="f7e66-123">Possible values are: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `QuarantinedOnDemand`, `TooManyDeletes`, `Unknown`.</span></span>|
|<span data-ttu-id="f7e66-124">сериесбеган</span><span class="sxs-lookup"><span data-stu-id="f7e66-124">seriesBegan</span></span>|<span data-ttu-id="f7e66-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7e66-125">DateTimeOffset</span></span>|<span data-ttu-id="f7e66-126">Дата и время первого помещения карантина в этот цикл (ряд начинается при первом включении карантина и сбрасывается, как только будет ликвидируется карантин).</span><span class="sxs-lookup"><span data-stu-id="f7e66-126">Date and time when the quarantine was first imposed in this series (a series starts when a quarantine is first imposed, and is reset as soon as the quarantine is lifted).</span></span> <span data-ttu-id="f7e66-127">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="f7e66-127">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f7e66-128">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f7e66-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="f7e66-129">сериескаунт</span><span class="sxs-lookup"><span data-stu-id="f7e66-129">seriesCount</span></span>|<span data-ttu-id="f7e66-130">Int64</span><span class="sxs-lookup"><span data-stu-id="f7e66-130">Int64</span></span>|<span data-ttu-id="f7e66-131">Количество повторных попыток вычисления и вступления в действия карантина для этой серии (ряд начинается при первом включении карантина и сбрасывается, как только приликвидируется карантин).</span><span class="sxs-lookup"><span data-stu-id="f7e66-131">Number of times in this series the quarantine was re-evaluated and left in effect (a series starts when quarantine is first imposed, and is reset as soon as quarantine is lifted).</span></span>|
|<span data-ttu-id="f7e66-132">error</span><span class="sxs-lookup"><span data-stu-id="f7e66-132">error</span></span>|[<span data-ttu-id="f7e66-133">синчронизатионеррор</span><span class="sxs-lookup"><span data-stu-id="f7e66-133">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="f7e66-134">Описывает ошибки, которые произошли при переводе задания синхронизации в карантин.</span><span class="sxs-lookup"><span data-stu-id="f7e66-134">Describes the error(s) that occurred when putting the synchronization job into quarantine.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f7e66-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f7e66-135">JSON representation</span></span>

<span data-ttu-id="f7e66-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7e66-136">The following is a JSON representation of the resource.</span></span>

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
