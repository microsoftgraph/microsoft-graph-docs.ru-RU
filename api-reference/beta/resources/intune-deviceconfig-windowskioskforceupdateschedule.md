---
title: Тип ресурса Виндовскиоскфорцеупдатесчедуле
description: Расписание принудительного обновления Windows 10 для устройств киоска.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d08a5e54aca83a71b094dbcd17095e421850b5ab
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525497"
---
# <a name="windowskioskforceupdateschedule-resource-type"></a><span data-ttu-id="eb96e-103">Тип ресурса Виндовскиоскфорцеупдатесчедуле</span><span class="sxs-lookup"><span data-stu-id="eb96e-103">windowsKioskForceUpdateSchedule resource type</span></span>

<span data-ttu-id="eb96e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="eb96e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eb96e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb96e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb96e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eb96e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb96e-107">Расписание принудительного обновления Windows 10 для устройств киоска.</span><span class="sxs-lookup"><span data-stu-id="eb96e-107">Windows 10 force update schedule for Kiosk devices.</span></span>

## <a name="properties"></a><span data-ttu-id="eb96e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="eb96e-108">Properties</span></span>
|<span data-ttu-id="eb96e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb96e-109">Property</span></span>|<span data-ttu-id="eb96e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="eb96e-110">Type</span></span>|<span data-ttu-id="eb96e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="eb96e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb96e-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="eb96e-112">startDateTime</span></span>|<span data-ttu-id="eb96e-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb96e-113">DateTimeOffset</span></span>|<span data-ttu-id="eb96e-114">Время начала принудительного перезапуска.</span><span class="sxs-lookup"><span data-stu-id="eb96e-114">The start time for the force restart.</span></span>|
|<span data-ttu-id="eb96e-115">recurrence</span><span class="sxs-lookup"><span data-stu-id="eb96e-115">recurrence</span></span>|[<span data-ttu-id="eb96e-116">windows10AppsUpdateRecurrence</span><span class="sxs-lookup"><span data-stu-id="eb96e-116">windows10AppsUpdateRecurrence</span></span>](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|<span data-ttu-id="eb96e-117">Расписание повторения.</span><span class="sxs-lookup"><span data-stu-id="eb96e-117">Recurrence schedule.</span></span> <span data-ttu-id="eb96e-118">Возможные значения: `none`, `daily`, `weekly`, `monthly`.</span><span class="sxs-lookup"><span data-stu-id="eb96e-118">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="eb96e-119">dayofWeek</span><span class="sxs-lookup"><span data-stu-id="eb96e-119">dayofWeek</span></span>|[<span data-ttu-id="eb96e-120">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="eb96e-120">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="eb96e-121">День недели.</span><span class="sxs-lookup"><span data-stu-id="eb96e-121">Day of week.</span></span> <span data-ttu-id="eb96e-122">Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="eb96e-122">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="eb96e-123">dayofMonth</span><span class="sxs-lookup"><span data-stu-id="eb96e-123">dayofMonth</span></span>|<span data-ttu-id="eb96e-124">Int32</span><span class="sxs-lookup"><span data-stu-id="eb96e-124">Int32</span></span>|<span data-ttu-id="eb96e-125">День месяца.</span><span class="sxs-lookup"><span data-stu-id="eb96e-125">Day of month.</span></span> <span data-ttu-id="eb96e-126">Допустимые значения — от 1 до 31.</span><span class="sxs-lookup"><span data-stu-id="eb96e-126">Valid values 1 to 31</span></span>|
|<span data-ttu-id="eb96e-127">руниммедиателифафтерстартдатетиме</span><span class="sxs-lookup"><span data-stu-id="eb96e-127">runImmediatelyIfAfterStartDateTime</span></span>|<span data-ttu-id="eb96e-128">Логический</span><span class="sxs-lookup"><span data-stu-id="eb96e-128">Boolean</span></span>|<span data-ttu-id="eb96e-129">Если этот параметр имеет значение true, задача выполняется немедленно, если StartDateTime находится в прошлое, иначе — выполняется при следующем повторении.</span><span class="sxs-lookup"><span data-stu-id="eb96e-129">If true, runs the task immediately if StartDateTime is in the past, else, runs at the next recurrence.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb96e-130">Связи</span><span class="sxs-lookup"><span data-stu-id="eb96e-130">Relationships</span></span>
<span data-ttu-id="eb96e-131">Нет</span><span class="sxs-lookup"><span data-stu-id="eb96e-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb96e-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eb96e-132">JSON Representation</span></span>
<span data-ttu-id="eb96e-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb96e-133">Here is a JSON representation of the resource.</span></span>
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



