---
title: Тип ресурса Синчронизатионпрогресс
description: Представляет ход выполнения Синчронизатионжоб в сторону завершения.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5040cb32b664497f2cbed9dc9ca77ce2a2a54ee7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023830"
---
# <a name="synchronizationprogress-resource-type"></a><span data-ttu-id="b6522-103">Тип ресурса Синчронизатионпрогресс</span><span class="sxs-lookup"><span data-stu-id="b6522-103">synchronizationProgress resource type</span></span>

<span data-ttu-id="b6522-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6522-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6522-105">Представляет ход выполнения [синчронизатионжоб](synchronization-synchronizationjob.md) в сторону завершения.</span><span class="sxs-lookup"><span data-stu-id="b6522-105">Represents the progress of a [synchronizationJob](synchronization-synchronizationjob.md) toward completion.</span></span>

## <a name="properties"></a><span data-ttu-id="b6522-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b6522-106">Properties</span></span>

| <span data-ttu-id="b6522-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6522-107">Property</span></span>                              | <span data-ttu-id="b6522-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b6522-108">Type</span></span>      | <span data-ttu-id="b6522-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b6522-109">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="b6522-110">комплетедунитс</span><span class="sxs-lookup"><span data-stu-id="b6522-110">completedUnits</span></span>|<span data-ttu-id="b6522-111">Int32</span><span class="sxs-lookup"><span data-stu-id="b6522-111">Int32</span></span>|<span data-ttu-id="b6522-112">Числитель коэффициента выполнения; количество единиц изменений, которые уже обработаны.</span><span class="sxs-lookup"><span data-stu-id="b6522-112">The numerator of a progress ratio; the number of units of changes already processed.</span></span>|
|<span data-ttu-id="b6522-113">прогрессобсерватиондатетиме</span><span class="sxs-lookup"><span data-stu-id="b6522-113">progressObservationDateTime</span></span>|<span data-ttu-id="b6522-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6522-114">DateTimeOffset</span></span>|<span data-ttu-id="b6522-115">Время отслеживания хода выполнения как смещение в минутах от времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="b6522-115">The time of a progress observation as an offset in minutes from UTC.</span></span>|
|<span data-ttu-id="b6522-116">тоталунитс</span><span class="sxs-lookup"><span data-stu-id="b6522-116">totalUnits</span></span>|<span data-ttu-id="b6522-117">Int32</span><span class="sxs-lookup"><span data-stu-id="b6522-117">Int32</span></span>|<span data-ttu-id="b6522-118">Знаменатель коэффициента выполнения; количество единиц изменений, которые необходимо обработать для выполнения синхронизации.</span><span class="sxs-lookup"><span data-stu-id="b6522-118">The denominator of a progress ratio; a number of units of changes to be processed to accomplish synchronization.</span></span>|
|<span data-ttu-id="b6522-119">продукции</span><span class="sxs-lookup"><span data-stu-id="b6522-119">units</span></span>|<span data-ttu-id="b6522-120">String</span><span class="sxs-lookup"><span data-stu-id="b6522-120">String</span></span>|<span data-ttu-id="b6522-121">Необязательное описание единиц измерения.</span><span class="sxs-lookup"><span data-stu-id="b6522-121">An optional description of the units.</span></span>|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a><span data-ttu-id="b6522-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b6522-122">JSON representation</span></span>

<span data-ttu-id="b6522-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6522-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationProgress"
}-->

```json
{
  "completedUnits": 1025,
  "progressObservationDateTime": "2017-10-10T17:00:00Z",
  "totalUnits": 3024,
  "units": "pages"
}

```

<!-- uuid: 15571993-7e2f-4842-84d5-01ceb67cdc05
20185-08-14 22:30:00 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationProcess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


