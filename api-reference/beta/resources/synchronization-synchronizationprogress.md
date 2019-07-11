---
title: Тип ресурса Синчронизатионпрогресс
description: Представляет ход выполнения Синчронизатионжоб в сторону завершения.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 92260f5e4ee0a036322b9ce1a7593a02a0a1565a
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35621174"
---
# <a name="synchronizationprogress-resource-type"></a><span data-ttu-id="0340f-103">Тип ресурса Синчронизатионпрогресс</span><span class="sxs-lookup"><span data-stu-id="0340f-103">synchronizationProgress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0340f-104">Представляет ход выполнения [синчронизатионжоб](synchronization-synchronizationjob.md) в сторону завершения.</span><span class="sxs-lookup"><span data-stu-id="0340f-104">Represents the progress of a [synchronizationJob](synchronization-synchronizationjob.md) toward completion.</span></span>

## <a name="properties"></a><span data-ttu-id="0340f-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="0340f-105">Properties</span></span>

| <span data-ttu-id="0340f-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="0340f-106">Property</span></span>                              | <span data-ttu-id="0340f-107">Тип</span><span class="sxs-lookup"><span data-stu-id="0340f-107">Type</span></span>      | <span data-ttu-id="0340f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0340f-108">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="0340f-109">Комплетедунитс</span><span class="sxs-lookup"><span data-stu-id="0340f-109">completedUnits</span></span>|<span data-ttu-id="0340f-110">Int32</span><span class="sxs-lookup"><span data-stu-id="0340f-110">Int32</span></span>|<span data-ttu-id="0340f-111">Числитель коэффициента выполнения; количество единиц изменений, которые уже обработаны.</span><span class="sxs-lookup"><span data-stu-id="0340f-111">The numerator of a progress ratio; the number of units of changes already processed.</span></span>|
|<span data-ttu-id="0340f-112">Прогрессобсерватиондатетиме</span><span class="sxs-lookup"><span data-stu-id="0340f-112">progressObservationDateTime</span></span>|<span data-ttu-id="0340f-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0340f-113">DateTimeOffset</span></span>|<span data-ttu-id="0340f-114">Время отслеживания хода выполнения как смещение в минутах от времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="0340f-114">The time of a progress observation as an offset in minutes from UTC.</span></span>|
|<span data-ttu-id="0340f-115">Тоталунитс</span><span class="sxs-lookup"><span data-stu-id="0340f-115">totalUnits</span></span>|<span data-ttu-id="0340f-116">Int32</span><span class="sxs-lookup"><span data-stu-id="0340f-116">Int32</span></span>|<span data-ttu-id="0340f-117">Знаменатель коэффициента выполнения; количество единиц изменений, которые необходимо обработать для выполнения синхронизации.</span><span class="sxs-lookup"><span data-stu-id="0340f-117">The denominator of a progress ratio; a number of units of changes to be processed to accomplish synchronization.</span></span>|
|<span data-ttu-id="0340f-118">продукции</span><span class="sxs-lookup"><span data-stu-id="0340f-118">units</span></span>|<span data-ttu-id="0340f-119">String</span><span class="sxs-lookup"><span data-stu-id="0340f-119">String</span></span>|<span data-ttu-id="0340f-120">Необязательное описание единиц измерения.</span><span class="sxs-lookup"><span data-stu-id="0340f-120">An optional description of the units.</span></span>|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a><span data-ttu-id="0340f-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0340f-121">JSON representation</span></span>

<span data-ttu-id="0340f-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0340f-122">The following is a JSON representation of the resource.</span></span>

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
