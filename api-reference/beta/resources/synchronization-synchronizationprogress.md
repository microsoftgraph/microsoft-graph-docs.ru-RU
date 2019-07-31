---
title: Тип ресурса Синчронизатионпрогресс
description: Представляет ход выполнения Синчронизатионжоб в сторону завершения.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dd1292d34abdc745075e030609d3f28a17b2431a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964643"
---
# <a name="synchronizationprogress-resource-type"></a><span data-ttu-id="ab73b-103">Тип ресурса Синчронизатионпрогресс</span><span class="sxs-lookup"><span data-stu-id="ab73b-103">synchronizationProgress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab73b-104">Представляет ход выполнения [синчронизатионжоб](synchronization-synchronizationjob.md) в сторону завершения.</span><span class="sxs-lookup"><span data-stu-id="ab73b-104">Represents the progress of a [synchronizationJob](synchronization-synchronizationjob.md) toward completion.</span></span>

## <a name="properties"></a><span data-ttu-id="ab73b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ab73b-105">Properties</span></span>

| <span data-ttu-id="ab73b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab73b-106">Property</span></span>                              | <span data-ttu-id="ab73b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ab73b-107">Type</span></span>      | <span data-ttu-id="ab73b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ab73b-108">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="ab73b-109">Комплетедунитс</span><span class="sxs-lookup"><span data-stu-id="ab73b-109">completedUnits</span></span>|<span data-ttu-id="ab73b-110">Int32</span><span class="sxs-lookup"><span data-stu-id="ab73b-110">Int32</span></span>|<span data-ttu-id="ab73b-111">Числитель коэффициента выполнения; количество единиц изменений, которые уже обработаны.</span><span class="sxs-lookup"><span data-stu-id="ab73b-111">The numerator of a progress ratio; the number of units of changes already processed.</span></span>|
|<span data-ttu-id="ab73b-112">Прогрессобсерватиондатетиме</span><span class="sxs-lookup"><span data-stu-id="ab73b-112">progressObservationDateTime</span></span>|<span data-ttu-id="ab73b-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab73b-113">DateTimeOffset</span></span>|<span data-ttu-id="ab73b-114">Время отслеживания хода выполнения как смещение в минутах от времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="ab73b-114">The time of a progress observation as an offset in minutes from UTC.</span></span>|
|<span data-ttu-id="ab73b-115">Тоталунитс</span><span class="sxs-lookup"><span data-stu-id="ab73b-115">totalUnits</span></span>|<span data-ttu-id="ab73b-116">Int32</span><span class="sxs-lookup"><span data-stu-id="ab73b-116">Int32</span></span>|<span data-ttu-id="ab73b-117">Знаменатель коэффициента выполнения; количество единиц изменений, которые необходимо обработать для выполнения синхронизации.</span><span class="sxs-lookup"><span data-stu-id="ab73b-117">The denominator of a progress ratio; a number of units of changes to be processed to accomplish synchronization.</span></span>|
|<span data-ttu-id="ab73b-118">продукции</span><span class="sxs-lookup"><span data-stu-id="ab73b-118">units</span></span>|<span data-ttu-id="ab73b-119">String</span><span class="sxs-lookup"><span data-stu-id="ab73b-119">String</span></span>|<span data-ttu-id="ab73b-120">Необязательное описание единиц измерения.</span><span class="sxs-lookup"><span data-stu-id="ab73b-120">An optional description of the units.</span></span>|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a><span data-ttu-id="ab73b-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ab73b-121">JSON representation</span></span>

<span data-ttu-id="ab73b-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab73b-122">The following is a JSON representation of the resource.</span></span>

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
