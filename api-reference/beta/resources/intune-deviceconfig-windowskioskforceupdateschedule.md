---
title: Тип ресурса Виндовскиоскфорцеупдатесчедуле
description: Расписание принудительного обновления Windows 10 для устройств киоска.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a3dd2e5872a60884050cd7a32408288955e94f92
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49276170"
---
# <a name="windowskioskforceupdateschedule-resource-type"></a><span data-ttu-id="20f33-103">Тип ресурса Виндовскиоскфорцеупдатесчедуле</span><span class="sxs-lookup"><span data-stu-id="20f33-103">windowsKioskForceUpdateSchedule resource type</span></span>

<span data-ttu-id="20f33-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20f33-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="20f33-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20f33-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20f33-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="20f33-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20f33-107">Расписание принудительного обновления Windows 10 для устройств киоска.</span><span class="sxs-lookup"><span data-stu-id="20f33-107">Windows 10 force update schedule for Kiosk devices.</span></span>

## <a name="properties"></a><span data-ttu-id="20f33-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="20f33-108">Properties</span></span>
|<span data-ttu-id="20f33-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="20f33-109">Property</span></span>|<span data-ttu-id="20f33-110">Тип</span><span class="sxs-lookup"><span data-stu-id="20f33-110">Type</span></span>|<span data-ttu-id="20f33-111">Описание</span><span class="sxs-lookup"><span data-stu-id="20f33-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20f33-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="20f33-112">startDateTime</span></span>|<span data-ttu-id="20f33-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20f33-113">DateTimeOffset</span></span>|<span data-ttu-id="20f33-114">Время начала принудительного перезапуска.</span><span class="sxs-lookup"><span data-stu-id="20f33-114">The start time for the force restart.</span></span>|
|<span data-ttu-id="20f33-115">recurrence</span><span class="sxs-lookup"><span data-stu-id="20f33-115">recurrence</span></span>|[<span data-ttu-id="20f33-116">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="20f33-116">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="20f33-117">Расписание повторения.</span><span class="sxs-lookup"><span data-stu-id="20f33-117">Recurrence schedule.</span></span> <span data-ttu-id="20f33-118">Возможные значения: `none`, `daily`, `weekly`, `monthly`.</span><span class="sxs-lookup"><span data-stu-id="20f33-118">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="20f33-119">dayofWeek</span><span class="sxs-lookup"><span data-stu-id="20f33-119">dayofWeek</span></span>|[<span data-ttu-id="20f33-120">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="20f33-120">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="20f33-121">День недели.</span><span class="sxs-lookup"><span data-stu-id="20f33-121">Day of week.</span></span> <span data-ttu-id="20f33-122">Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="20f33-122">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="20f33-123">dayofMonth</span><span class="sxs-lookup"><span data-stu-id="20f33-123">dayofMonth</span></span>|<span data-ttu-id="20f33-124">Int32</span><span class="sxs-lookup"><span data-stu-id="20f33-124">Int32</span></span>|<span data-ttu-id="20f33-125">День месяца.</span><span class="sxs-lookup"><span data-stu-id="20f33-125">Day of month.</span></span> <span data-ttu-id="20f33-126">Допустимые значения — от 1 до 31.</span><span class="sxs-lookup"><span data-stu-id="20f33-126">Valid values 1 to 31</span></span>|
|<span data-ttu-id="20f33-127">руниммедиателифафтерстартдатетиме</span><span class="sxs-lookup"><span data-stu-id="20f33-127">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="20f33-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="20f33-128">Boolean</span></span>|<span data-ttu-id="20f33-129">Если этот параметр имеет значение true, задача выполняется немедленно, если StartDateTime находится в прошлое, иначе — выполняется при следующем повторении.</span><span class="sxs-lookup"><span data-stu-id="20f33-129">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="20f33-130">Связи</span><span class="sxs-lookup"><span data-stu-id="20f33-130">Relationships</span></span>
<span data-ttu-id="20f33-131">Нет</span><span class="sxs-lookup"><span data-stu-id="20f33-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="20f33-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="20f33-132">JSON Representation</span></span>
<span data-ttu-id="20f33-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20f33-133">Here is a JSON representation of the resource.</span></span>
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




