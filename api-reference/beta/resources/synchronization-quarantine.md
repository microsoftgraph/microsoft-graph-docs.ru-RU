---
title: Тип ресурса Синчронизатионкуарантине
description: Предоставляет сведения о состоянии карантина Синчронизатионжоб.
localization_priority: Normal
ms.openlocfilehash: 6d5d5c3cbe96eda6b39833287e8efb6e0771b19a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523217"
---
# <a name="synchronizationquarantine-resource-type"></a><span data-ttu-id="1882e-103">Тип ресурса Синчронизатионкуарантине</span><span class="sxs-lookup"><span data-stu-id="1882e-103">synchronizationQuarantine resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1882e-104">Предоставляет сведения о состоянии карантина [синчронизатионжоб](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="1882e-104">Provides information about the quarantine state of a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1882e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="1882e-105">Properties</span></span>
| <span data-ttu-id="1882e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="1882e-106">Property</span></span>     | <span data-ttu-id="1882e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="1882e-107">Type</span></span>   |<span data-ttu-id="1882e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1882e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1882e-109">Куррентбеган</span><span class="sxs-lookup"><span data-stu-id="1882e-109">currentBegan</span></span>|<span data-ttu-id="1882e-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1882e-110">DateTimeOffset</span></span>|<span data-ttu-id="1882e-111">Дата и время последнего вычисления и ликвидации карантина.</span><span class="sxs-lookup"><span data-stu-id="1882e-111">Date and time when the quarantine was last evaluated and imposed.</span></span> <span data-ttu-id="1882e-112">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="1882e-112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1882e-113">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="1882e-113">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="1882e-114">Некстаттемпт</span><span class="sxs-lookup"><span data-stu-id="1882e-114">nextAttempt</span></span>|<span data-ttu-id="1882e-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1882e-115">DateTimeOffset</span></span>|<span data-ttu-id="1882e-116">Дата и время следующей попытки повторной оценки карантина.</span><span class="sxs-lookup"><span data-stu-id="1882e-116">Date and time when the next attempt to re-evaluate the quarantine will be made.</span></span> <span data-ttu-id="1882e-117">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="1882e-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1882e-118">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="1882e-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="1882e-119">причиной</span><span class="sxs-lookup"><span data-stu-id="1882e-119">reason</span></span>|<span data-ttu-id="1882e-120">String</span><span class="sxs-lookup"><span data-stu-id="1882e-120">String</span></span>|<span data-ttu-id="1882e-121">Код, обозначающий, почему был наложен карантин.</span><span class="sxs-lookup"><span data-stu-id="1882e-121">A code that signifies why the quarantine was imposed.</span></span> <span data-ttu-id="1882e-122">Возможные значения: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `Unknown`.</span><span class="sxs-lookup"><span data-stu-id="1882e-122">Possible values are: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `Unknown`.</span></span>|
|<span data-ttu-id="1882e-123">Сериесбеган</span><span class="sxs-lookup"><span data-stu-id="1882e-123">seriesBegan</span></span>|<span data-ttu-id="1882e-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1882e-124">DateTimeOffset</span></span>|<span data-ttu-id="1882e-125">Дата и время первого помещения карантина в этот цикл (ряд начинается при первом включении карантина и сбрасывается, как только будет ликвидируется карантин).</span><span class="sxs-lookup"><span data-stu-id="1882e-125">Date and time when the quarantine was first imposed in this series (a series starts when a quarantine is first imposed, and is reset as soon as the quarantine is lifted).</span></span> <span data-ttu-id="1882e-126">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="1882e-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1882e-127">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="1882e-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="1882e-128">Сериескаунт</span><span class="sxs-lookup"><span data-stu-id="1882e-128">seriesCount</span></span>|<span data-ttu-id="1882e-129">Int64</span><span class="sxs-lookup"><span data-stu-id="1882e-129">Int64</span></span>|<span data-ttu-id="1882e-130">Количество повторных попыток вычисления и вступления в действия карантина для этой серии (ряд начинается при первом включении карантина и сбрасывается, как только приликвидируется карантин).</span><span class="sxs-lookup"><span data-stu-id="1882e-130">Number of times in this series the quarantine was re-evaluated and left in effect (a series starts when quarantine is first imposed, and is reset as soon as quarantine is lifted).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1882e-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1882e-131">JSON representation</span></span>

<span data-ttu-id="1882e-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1882e-132">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-quarantine.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
