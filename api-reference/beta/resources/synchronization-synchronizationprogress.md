---
title: Тип ресурса synchronizationProgress
description: Представляет ход выполнения синхронизации.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: f6f8f7cc5d0419a6f0e9203513db5b1452db1797
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131644"
---
# <a name="synchronizationprogress-resource-type"></a><span data-ttu-id="25b75-103">Тип ресурса synchronizationProgress</span><span class="sxs-lookup"><span data-stu-id="25b75-103">synchronizationProgress resource type</span></span>

<span data-ttu-id="25b75-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25b75-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25b75-105">Представляет ход выполнения [синхронизации.](synchronization-synchronizationjob.md)</span><span class="sxs-lookup"><span data-stu-id="25b75-105">Represents the progress of a [synchronizationJob](synchronization-synchronizationjob.md) toward completion.</span></span>

## <a name="properties"></a><span data-ttu-id="25b75-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="25b75-106">Properties</span></span>

| <span data-ttu-id="25b75-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="25b75-107">Property</span></span>                              | <span data-ttu-id="25b75-108">Тип</span><span class="sxs-lookup"><span data-stu-id="25b75-108">Type</span></span>      | <span data-ttu-id="25b75-109">Описание</span><span class="sxs-lookup"><span data-stu-id="25b75-109">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="25b75-110">completedUnits</span><span class="sxs-lookup"><span data-stu-id="25b75-110">completedUnits</span></span>|<span data-ttu-id="25b75-111">Int32</span><span class="sxs-lookup"><span data-stu-id="25b75-111">Int32</span></span>|<span data-ttu-id="25b75-112">Числитель соотношения хода выполнения; количество уже обработанных единиц изменений.</span><span class="sxs-lookup"><span data-stu-id="25b75-112">The numerator of a progress ratio; the number of units of changes already processed.</span></span>|
|<span data-ttu-id="25b75-113">progressObservationDateTime</span><span class="sxs-lookup"><span data-stu-id="25b75-113">progressObservationDateTime</span></span>|<span data-ttu-id="25b75-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25b75-114">DateTimeOffset</span></span>|<span data-ttu-id="25b75-115">Время наблюдения за ходом выполнения как смещение в минутах от времени в UTC.</span><span class="sxs-lookup"><span data-stu-id="25b75-115">The time of a progress observation as an offset in minutes from UTC.</span></span>|
|<span data-ttu-id="25b75-116">totalUnits</span><span class="sxs-lookup"><span data-stu-id="25b75-116">totalUnits</span></span>|<span data-ttu-id="25b75-117">Int32</span><span class="sxs-lookup"><span data-stu-id="25b75-117">Int32</span></span>|<span data-ttu-id="25b75-118">Коэффициент выполнения; количество единиц изменений, которые необходимо обработать для выполнения синхронизации.</span><span class="sxs-lookup"><span data-stu-id="25b75-118">The denominator of a progress ratio; a number of units of changes to be processed to accomplish synchronization.</span></span>|
|<span data-ttu-id="25b75-119">units</span><span class="sxs-lookup"><span data-stu-id="25b75-119">units</span></span>|<span data-ttu-id="25b75-120">Строка</span><span class="sxs-lookup"><span data-stu-id="25b75-120">String</span></span>|<span data-ttu-id="25b75-121">Необязательное описание единиц.</span><span class="sxs-lookup"><span data-stu-id="25b75-121">An optional description of the units.</span></span>|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a><span data-ttu-id="25b75-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="25b75-122">JSON representation</span></span>

<span data-ttu-id="25b75-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="25b75-123">The following is a JSON representation of the resource.</span></span>

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


