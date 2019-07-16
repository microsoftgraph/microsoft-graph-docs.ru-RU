---
title: Тип ресурса Виндовскиоскфорцеупдатесчедуле
description: Расписание принудительного обновления Windows 10 для устройств киоска.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6584312503678596a46d606de97ce6f52335d3c5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741522"
---
# <a name="windowskioskforceupdateschedule-resource-type"></a><span data-ttu-id="15458-103">Тип ресурса Виндовскиоскфорцеупдатесчедуле</span><span class="sxs-lookup"><span data-stu-id="15458-103">windowsKioskForceUpdateSchedule resource type</span></span>

> <span data-ttu-id="15458-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15458-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15458-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15458-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15458-106">Расписание принудительного обновления Windows 10 для устройств киоска.</span><span class="sxs-lookup"><span data-stu-id="15458-106">Windows 10 force update schedule for Kiosk devices.</span></span>

## <a name="properties"></a><span data-ttu-id="15458-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="15458-107">Properties</span></span>
|<span data-ttu-id="15458-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="15458-108">Property</span></span>|<span data-ttu-id="15458-109">Тип</span><span class="sxs-lookup"><span data-stu-id="15458-109">Type</span></span>|<span data-ttu-id="15458-110">Описание</span><span class="sxs-lookup"><span data-stu-id="15458-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15458-111">startDateTime</span><span class="sxs-lookup"><span data-stu-id="15458-111">startDateTime</span></span>|<span data-ttu-id="15458-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15458-112">DateTimeOffset</span></span>|<span data-ttu-id="15458-113">Время начала принудительного перезапуска.</span><span class="sxs-lookup"><span data-stu-id="15458-113">The start time for the force restart.</span></span>|
|<span data-ttu-id="15458-114">recurrence</span><span class="sxs-lookup"><span data-stu-id="15458-114">recurrence</span></span>|[<span data-ttu-id="15458-115">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="15458-115">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="15458-116">Расписание повторения.</span><span class="sxs-lookup"><span data-stu-id="15458-116">Recurrence schedule.</span></span> <span data-ttu-id="15458-117">Возможные значения: `none`, `daily`, `weekly`, `monthly`.</span><span class="sxs-lookup"><span data-stu-id="15458-117">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="15458-118">dayofWeek</span><span class="sxs-lookup"><span data-stu-id="15458-118">dayofWeek</span></span>|[<span data-ttu-id="15458-119">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="15458-119">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="15458-120">День недели.</span><span class="sxs-lookup"><span data-stu-id="15458-120">Day of week.</span></span> <span data-ttu-id="15458-121">Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="15458-121">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="15458-122">dayofMonth</span><span class="sxs-lookup"><span data-stu-id="15458-122">dayofMonth</span></span>|<span data-ttu-id="15458-123">Int32</span><span class="sxs-lookup"><span data-stu-id="15458-123">Int32</span></span>|<span data-ttu-id="15458-124">День месяца.</span><span class="sxs-lookup"><span data-stu-id="15458-124">Day of month.</span></span> <span data-ttu-id="15458-125">Допустимые значения — от 1 до 31.</span><span class="sxs-lookup"><span data-stu-id="15458-125">Valid values 1 to 31</span></span>|
|<span data-ttu-id="15458-126">Руниммедиателифафтерстартдатетиме</span><span class="sxs-lookup"><span data-stu-id="15458-126">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="15458-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="15458-127">Boolean</span></span>|<span data-ttu-id="15458-128">Если этот параметр имеет значение true, задача выполняется немедленно, если StartDateTime находится в прошлое, иначе — выполняется при следующем повторении.</span><span class="sxs-lookup"><span data-stu-id="15458-128">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="15458-129">Отношения</span><span class="sxs-lookup"><span data-stu-id="15458-129">Relationships</span></span>
<span data-ttu-id="15458-130">Нет</span><span class="sxs-lookup"><span data-stu-id="15458-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="15458-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="15458-131">JSON Representation</span></span>
<span data-ttu-id="15458-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15458-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskForceUpdateSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskForceUpdateSchedule",
  "startDateTime": "String (timestamp)",
  "recurrence": "String",
  "dayofWeek": "String",
  "dayofMonth": 1024,
  "runImmediatelyIfAfterStartDateTime": true
}
```





