---
title: Тип ресурса synchronizationProgress
description: Представляет ход выполнения synchronizationJob к завершению.
localization_priority: Normal
ms.openlocfilehash: b22bd95f54a9f268524dc98a8d3df94fcc14f773
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510976"
---
# <a name="synchronizationprogress-resource-type"></a><span data-ttu-id="fa477-103">Тип ресурса synchronizationProgress</span><span class="sxs-lookup"><span data-stu-id="fa477-103">synchronizationProgress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa477-104">Представляет ход выполнения [synchronizationJob](synchronization-synchronizationjob.md) к завершению.</span><span class="sxs-lookup"><span data-stu-id="fa477-104">Represents the progress of a [synchronizationJob](synchronization-synchronizationjob.md) toward completion.</span></span>

## <a name="properties"></a><span data-ttu-id="fa477-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="fa477-105">Properties</span></span>

| <span data-ttu-id="fa477-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa477-106">Property</span></span>                              | <span data-ttu-id="fa477-107">Тип</span><span class="sxs-lookup"><span data-stu-id="fa477-107">Type</span></span>      | <span data-ttu-id="fa477-108">Описание</span><span class="sxs-lookup"><span data-stu-id="fa477-108">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="fa477-109">completedUnits</span><span class="sxs-lookup"><span data-stu-id="fa477-109">completedUnits</span></span>|<span data-ttu-id="fa477-110">Int32</span><span class="sxs-lookup"><span data-stu-id="fa477-110">Int32</span></span>|<span data-ttu-id="fa477-111">Числитель соотношение хода выполнения; Количество единиц уже обработки изменений.</span><span class="sxs-lookup"><span data-stu-id="fa477-111">The numerator of a progress ratio; the number of units of changes already processed.</span></span>|
|<span data-ttu-id="fa477-112">progressObservationDateTime</span><span class="sxs-lookup"><span data-stu-id="fa477-112">progressObservationDateTime</span></span>|<span data-ttu-id="fa477-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa477-113">DateTimeOffset</span></span>|<span data-ttu-id="fa477-114">Время наблюдения хода выполнения как смещение в минутах от времени UTC.</span><span class="sxs-lookup"><span data-stu-id="fa477-114">The time of a progress observation as an offset in minutes from UTC.</span></span>|
|<span data-ttu-id="fa477-115">totalUnits</span><span class="sxs-lookup"><span data-stu-id="fa477-115">totalUnits</span></span>|<span data-ttu-id="fa477-116">Int32</span><span class="sxs-lookup"><span data-stu-id="fa477-116">Int32</span></span>|<span data-ttu-id="fa477-117">Делителя соотношение хода выполнения; Количество единиц изменения обработки для выполнения синхронизации.</span><span class="sxs-lookup"><span data-stu-id="fa477-117">The denominator of a progress ratio; a number of units of changes to be processed to accomplish synchronization.</span></span>|
|<span data-ttu-id="fa477-118">Units</span><span class="sxs-lookup"><span data-stu-id="fa477-118">units</span></span>|<span data-ttu-id="fa477-119">String</span><span class="sxs-lookup"><span data-stu-id="fa477-119">String</span></span>|<span data-ttu-id="fa477-120">Необязательное описание единицы измерения.</span><span class="sxs-lookup"><span data-stu-id="fa477-120">An optional description of the units.</span></span>|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a><span data-ttu-id="fa477-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fa477-121">JSON representation</span></span>

<span data-ttu-id="fa477-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa477-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationStatus"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationprogress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
