---
title: Тип ресурса Виндовскиоскфорцеупдатесчедуле
description: Расписание принудительного обновления Windows 10 для устройств киоска.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bc53498bf14dff5c62a4646f504ae1a31c84ed1b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039778"
---
# <a name="windowskioskforceupdateschedule-resource-type"></a><span data-ttu-id="18a03-103">Тип ресурса Виндовскиоскфорцеупдатесчедуле</span><span class="sxs-lookup"><span data-stu-id="18a03-103">windowsKioskForceUpdateSchedule resource type</span></span>

<span data-ttu-id="18a03-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18a03-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18a03-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18a03-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18a03-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="18a03-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18a03-107">Расписание принудительного обновления Windows 10 для устройств киоска.</span><span class="sxs-lookup"><span data-stu-id="18a03-107">Windows 10 force update schedule for Kiosk devices.</span></span>

## <a name="properties"></a><span data-ttu-id="18a03-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="18a03-108">Properties</span></span>
|<span data-ttu-id="18a03-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="18a03-109">Property</span></span>|<span data-ttu-id="18a03-110">Тип</span><span class="sxs-lookup"><span data-stu-id="18a03-110">Type</span></span>|<span data-ttu-id="18a03-111">Описание</span><span class="sxs-lookup"><span data-stu-id="18a03-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18a03-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="18a03-112">startDateTime</span></span>|<span data-ttu-id="18a03-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18a03-113">DateTimeOffset</span></span>|<span data-ttu-id="18a03-114">Время начала принудительного перезапуска.</span><span class="sxs-lookup"><span data-stu-id="18a03-114">The start time for the force restart.</span></span>|
|<span data-ttu-id="18a03-115">recurrence</span><span class="sxs-lookup"><span data-stu-id="18a03-115">recurrence</span></span>|[<span data-ttu-id="18a03-116">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="18a03-116">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="18a03-117">Расписание повторения.</span><span class="sxs-lookup"><span data-stu-id="18a03-117">Recurrence schedule.</span></span> <span data-ttu-id="18a03-118">Возможные значения: `none`, `daily`, `weekly`, `monthly`.</span><span class="sxs-lookup"><span data-stu-id="18a03-118">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="18a03-119">dayofWeek</span><span class="sxs-lookup"><span data-stu-id="18a03-119">dayofWeek</span></span>|[<span data-ttu-id="18a03-120">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="18a03-120">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="18a03-121">День недели.</span><span class="sxs-lookup"><span data-stu-id="18a03-121">Day of week.</span></span> <span data-ttu-id="18a03-122">Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="18a03-122">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="18a03-123">dayofMonth</span><span class="sxs-lookup"><span data-stu-id="18a03-123">dayofMonth</span></span>|<span data-ttu-id="18a03-124">Int32</span><span class="sxs-lookup"><span data-stu-id="18a03-124">Int32</span></span>|<span data-ttu-id="18a03-125">День месяца.</span><span class="sxs-lookup"><span data-stu-id="18a03-125">Day of month.</span></span> <span data-ttu-id="18a03-126">Допустимые значения — от 1 до 31.</span><span class="sxs-lookup"><span data-stu-id="18a03-126">Valid values 1 to 31</span></span>|
|<span data-ttu-id="18a03-127">руниммедиателифафтерстартдатетиме</span><span class="sxs-lookup"><span data-stu-id="18a03-127">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="18a03-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="18a03-128">Boolean</span></span>|<span data-ttu-id="18a03-129">Если этот параметр имеет значение true, задача выполняется немедленно, если StartDateTime находится в прошлое, иначе — выполняется при следующем повторении.</span><span class="sxs-lookup"><span data-stu-id="18a03-129">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="18a03-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="18a03-130">Relationships</span></span>
<span data-ttu-id="18a03-131">Нет</span><span class="sxs-lookup"><span data-stu-id="18a03-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="18a03-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="18a03-132">JSON Representation</span></span>
<span data-ttu-id="18a03-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18a03-133">Here is a JSON representation of the resource.</span></span>
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






