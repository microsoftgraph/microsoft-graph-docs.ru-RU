---
title: Тип ресурса synchronizationProgress
description: Представляет ход выполнения synchronizationJob к завершению.
ms.openlocfilehash: 412b7754dac97a36efe082026ab360569c0fe789
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082431"
---
# <a name="synchronizationprogress-resource-type"></a><span data-ttu-id="de594-103">Тип ресурса synchronizationProgress</span><span class="sxs-lookup"><span data-stu-id="de594-103">synchronizationProgress resource type</span></span>

> <span data-ttu-id="de594-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="de594-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de594-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de594-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="de594-106">Представляет ход выполнения [synchronizationJob](synchronization-synchronizationjob.md) к завершению.</span><span class="sxs-lookup"><span data-stu-id="de594-106">Represents the progress of a [synchronizationJob](synchronization-synchronizationjob.md) toward completion.</span></span>

## <a name="properties"></a><span data-ttu-id="de594-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="de594-107">Properties</span></span>

| <span data-ttu-id="de594-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="de594-108">Property</span></span>                              | <span data-ttu-id="de594-109">Тип</span><span class="sxs-lookup"><span data-stu-id="de594-109">Type</span></span>      | <span data-ttu-id="de594-110">Description</span><span class="sxs-lookup"><span data-stu-id="de594-110">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="de594-111">completedUnits</span><span class="sxs-lookup"><span data-stu-id="de594-111">completedUnits</span></span>|<span data-ttu-id="de594-112">Int32</span><span class="sxs-lookup"><span data-stu-id="de594-112">Int32</span></span>|<span data-ttu-id="de594-113">Числитель соотношение хода выполнения; Количество единиц уже обработки изменений.</span><span class="sxs-lookup"><span data-stu-id="de594-113">The numerator of a progress ratio; the number of units of changes already processed.</span></span>|
|<span data-ttu-id="de594-114">progressObservationDateTime</span><span class="sxs-lookup"><span data-stu-id="de594-114">progressObservationDateTime</span></span>|<span data-ttu-id="de594-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de594-115">DateTimeOffset</span></span>|<span data-ttu-id="de594-116">Время наблюдения хода выполнения как смещение в минутах от времени UTC.</span><span class="sxs-lookup"><span data-stu-id="de594-116">The time of a progress observation as an offset in minutes from UTC.</span></span>|
|<span data-ttu-id="de594-117">totalUnits</span><span class="sxs-lookup"><span data-stu-id="de594-117">totalUnits</span></span>|<span data-ttu-id="de594-118">Int32</span><span class="sxs-lookup"><span data-stu-id="de594-118">Int32</span></span>|<span data-ttu-id="de594-119">Делителя соотношение хода выполнения; Количество единиц изменения обработки для выполнения синхронизации.</span><span class="sxs-lookup"><span data-stu-id="de594-119">The denominator of a progress ratio; a number of units of changes to be processed to accomplish synchronization.</span></span>|
|<span data-ttu-id="de594-120">единицы</span><span class="sxs-lookup"><span data-stu-id="de594-120">units</span></span>|<span data-ttu-id="de594-121">String</span><span class="sxs-lookup"><span data-stu-id="de594-121">String</span></span>|<span data-ttu-id="de594-122">Необязательное описание единицы измерения.</span><span class="sxs-lookup"><span data-stu-id="de594-122">An optional description of the units.</span></span>|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a><span data-ttu-id="de594-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="de594-123">JSON representation</span></span>

<span data-ttu-id="de594-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de594-124">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationProcess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
