---
title: Тип ресурса Синчронизатионкуарантине
description: Предоставляет сведения о состоянии карантина Синчронизатионжоб.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 129dc7a07fb111bdf85dfc84eec29375a153e7fa
ms.sourcegitcommit: 471f07c30867658688bd932e06822be1bbcea360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2019
ms.locfileid: "37036342"
---
# <a name="synchronizationquarantine-resource-type"></a><span data-ttu-id="aa742-103">Тип ресурса Синчронизатионкуарантине</span><span class="sxs-lookup"><span data-stu-id="aa742-103">synchronizationQuarantine resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa742-104">Предоставляет сведения о состоянии карантина [синчронизатионжоб](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="aa742-104">Provides information about the quarantine state of a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="aa742-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="aa742-105">Properties</span></span>
| <span data-ttu-id="aa742-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa742-106">Property</span></span>     | <span data-ttu-id="aa742-107">Тип</span><span class="sxs-lookup"><span data-stu-id="aa742-107">Type</span></span>   |<span data-ttu-id="aa742-108">Описание</span><span class="sxs-lookup"><span data-stu-id="aa742-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa742-109">куррентбеган</span><span class="sxs-lookup"><span data-stu-id="aa742-109">currentBegan</span></span>|<span data-ttu-id="aa742-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa742-110">DateTimeOffset</span></span>|<span data-ttu-id="aa742-111">Дата и время последнего вычисления и ликвидации карантина.</span><span class="sxs-lookup"><span data-stu-id="aa742-111">Date and time when the quarantine was last evaluated and imposed.</span></span> <span data-ttu-id="aa742-112">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="aa742-112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="aa742-113">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="aa742-113">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="aa742-114">некстаттемпт</span><span class="sxs-lookup"><span data-stu-id="aa742-114">nextAttempt</span></span>|<span data-ttu-id="aa742-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa742-115">DateTimeOffset</span></span>|<span data-ttu-id="aa742-116">Дата и время следующей попытки повторной оценки карантина.</span><span class="sxs-lookup"><span data-stu-id="aa742-116">Date and time when the next attempt to re-evaluate the quarantine will be made.</span></span> <span data-ttu-id="aa742-117">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="aa742-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="aa742-118">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="aa742-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="aa742-119">причиной</span><span class="sxs-lookup"><span data-stu-id="aa742-119">reason</span></span>|<span data-ttu-id="aa742-120">String.</span><span class="sxs-lookup"><span data-stu-id="aa742-120">String</span></span>|<span data-ttu-id="aa742-121">Код, обозначающий, почему был наложен карантин.</span><span class="sxs-lookup"><span data-stu-id="aa742-121">A code that signifies why the quarantine was imposed.</span></span> <span data-ttu-id="aa742-122">Возможные значения: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `QuarantinedOnDemand`, `TooManyDeletes`, `Unknown`.</span><span class="sxs-lookup"><span data-stu-id="aa742-122">Possible values are: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `QuarantinedOnDemand`, `TooManyDeletes`, `Unknown`.</span></span>|
|<span data-ttu-id="aa742-123">сериесбеган</span><span class="sxs-lookup"><span data-stu-id="aa742-123">seriesBegan</span></span>|<span data-ttu-id="aa742-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa742-124">DateTimeOffset</span></span>|<span data-ttu-id="aa742-125">Дата и время первого помещения карантина в этот цикл (ряд начинается при первом включении карантина и сбрасывается, как только будет ликвидируется карантин).</span><span class="sxs-lookup"><span data-stu-id="aa742-125">Date and time when the quarantine was first imposed in this series (a series starts when a quarantine is first imposed, and is reset as soon as the quarantine is lifted).</span></span> <span data-ttu-id="aa742-126">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="aa742-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="aa742-127">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="aa742-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="aa742-128">сериескаунт</span><span class="sxs-lookup"><span data-stu-id="aa742-128">seriesCount</span></span>|<span data-ttu-id="aa742-129">Int64</span><span class="sxs-lookup"><span data-stu-id="aa742-129">Int64</span></span>|<span data-ttu-id="aa742-130">Количество повторных попыток вычисления и вступления в действия карантина для этой серии (ряд начинается при первом включении карантина и сбрасывается, как только приликвидируется карантин).</span><span class="sxs-lookup"><span data-stu-id="aa742-130">Number of times in this series the quarantine was re-evaluated and left in effect (a series starts when quarantine is first imposed, and is reset as soon as quarantine is lifted).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aa742-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aa742-131">JSON representation</span></span>

<span data-ttu-id="aa742-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa742-132">The following is a JSON representation of the resource.</span></span>

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
