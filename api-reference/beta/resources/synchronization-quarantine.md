---
title: Тип ресурса Синчронизатионкуарантине
description: Предоставляет сведения о состоянии карантина Синчронизатионжоб.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ca404ced0448534f6ed116f6376a8d26bcb24a90
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620467"
---
# <a name="synchronizationquarantine-resource-type"></a><span data-ttu-id="f47c7-103">Тип ресурса Синчронизатионкуарантине</span><span class="sxs-lookup"><span data-stu-id="f47c7-103">synchronizationQuarantine resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f47c7-104">Предоставляет сведения о состоянии карантина [синчронизатионжоб](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="f47c7-104">Provides information about the quarantine state of a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f47c7-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f47c7-105">Properties</span></span>
| <span data-ttu-id="f47c7-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f47c7-106">Property</span></span>     | <span data-ttu-id="f47c7-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f47c7-107">Type</span></span>   |<span data-ttu-id="f47c7-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f47c7-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f47c7-109">Куррентбеган</span><span class="sxs-lookup"><span data-stu-id="f47c7-109">currentBegan</span></span>|<span data-ttu-id="f47c7-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f47c7-110">DateTimeOffset</span></span>|<span data-ttu-id="f47c7-111">Дата и время последнего вычисления и ликвидации карантина.</span><span class="sxs-lookup"><span data-stu-id="f47c7-111">Date and time when the quarantine was last evaluated and imposed.</span></span> <span data-ttu-id="f47c7-112">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="f47c7-112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f47c7-113">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f47c7-113">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="f47c7-114">Некстаттемпт</span><span class="sxs-lookup"><span data-stu-id="f47c7-114">nextAttempt</span></span>|<span data-ttu-id="f47c7-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f47c7-115">DateTimeOffset</span></span>|<span data-ttu-id="f47c7-116">Дата и время следующей попытки повторной оценки карантина.</span><span class="sxs-lookup"><span data-stu-id="f47c7-116">Date and time when the next attempt to re-evaluate the quarantine will be made.</span></span> <span data-ttu-id="f47c7-117">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="f47c7-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f47c7-118">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f47c7-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="f47c7-119">причиной</span><span class="sxs-lookup"><span data-stu-id="f47c7-119">reason</span></span>|<span data-ttu-id="f47c7-120">String</span><span class="sxs-lookup"><span data-stu-id="f47c7-120">String</span></span>|<span data-ttu-id="f47c7-121">Код, обозначающий, почему был наложен карантин.</span><span class="sxs-lookup"><span data-stu-id="f47c7-121">A code that signifies why the quarantine was imposed.</span></span> <span data-ttu-id="f47c7-122">Возможные значения: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `Unknown`.</span><span class="sxs-lookup"><span data-stu-id="f47c7-122">Possible values are: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `Unknown`.</span></span>|
|<span data-ttu-id="f47c7-123">Сериесбеган</span><span class="sxs-lookup"><span data-stu-id="f47c7-123">seriesBegan</span></span>|<span data-ttu-id="f47c7-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f47c7-124">DateTimeOffset</span></span>|<span data-ttu-id="f47c7-125">Дата и время первого помещения карантина в этот цикл (ряд начинается при первом включении карантина и сбрасывается, как только будет ликвидируется карантин).</span><span class="sxs-lookup"><span data-stu-id="f47c7-125">Date and time when the quarantine was first imposed in this series (a series starts when a quarantine is first imposed, and is reset as soon as the quarantine is lifted).</span></span> <span data-ttu-id="f47c7-126">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="f47c7-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f47c7-127">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f47c7-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="f47c7-128">Сериескаунт</span><span class="sxs-lookup"><span data-stu-id="f47c7-128">seriesCount</span></span>|<span data-ttu-id="f47c7-129">Int64</span><span class="sxs-lookup"><span data-stu-id="f47c7-129">Int64</span></span>|<span data-ttu-id="f47c7-130">Количество повторных попыток вычисления и вступления в действия карантина для этой серии (ряд начинается при первом включении карантина и сбрасывается, как только приликвидируется карантин).</span><span class="sxs-lookup"><span data-stu-id="f47c7-130">Number of times in this series the quarantine was re-evaluated and left in effect (a series starts when quarantine is first imposed, and is reset as soon as quarantine is lifted).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f47c7-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f47c7-131">JSON representation</span></span>

<span data-ttu-id="f47c7-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f47c7-132">The following is a JSON representation of the resource.</span></span>

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
