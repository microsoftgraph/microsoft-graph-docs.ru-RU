---
title: Тип ресурса deviceGeoLocation
description: Расположение устройства
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 46a92f1faad55d82e2ed8184c5f4a4d360b7d588
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33942138"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="35d0d-103">Тип ресурса deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="35d0d-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="35d0d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35d0d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35d0d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="35d0d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35d0d-106">Расположение устройства</span><span class="sxs-lookup"><span data-stu-id="35d0d-106">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="35d0d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="35d0d-107">Properties</span></span>
|<span data-ttu-id="35d0d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="35d0d-108">Property</span></span>|<span data-ttu-id="35d0d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="35d0d-109">Type</span></span>|<span data-ttu-id="35d0d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="35d0d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35d0d-111">Ластколлектеддатетимеутк</span><span class="sxs-lookup"><span data-stu-id="35d0d-111">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="35d0d-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35d0d-112">DateTimeOffset</span></span>|<span data-ttu-id="35d0d-113">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="35d0d-113">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="35d0d-114">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="35d0d-114">lastCollectedDateTime</span></span>|<span data-ttu-id="35d0d-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35d0d-115">DateTimeOffset</span></span>|<span data-ttu-id="35d0d-116">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="35d0d-116">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="35d0d-117">longitude</span><span class="sxs-lookup"><span data-stu-id="35d0d-117">longitude</span></span>|<span data-ttu-id="35d0d-118">Двойное</span><span class="sxs-lookup"><span data-stu-id="35d0d-118">Double</span></span>|<span data-ttu-id="35d0d-119">Долгота расположения устройства</span><span class="sxs-lookup"><span data-stu-id="35d0d-119">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="35d0d-120">latitude</span><span class="sxs-lookup"><span data-stu-id="35d0d-120">latitude</span></span>|<span data-ttu-id="35d0d-121">Двойное</span><span class="sxs-lookup"><span data-stu-id="35d0d-121">Double</span></span>|<span data-ttu-id="35d0d-122">Широта расположения устройства</span><span class="sxs-lookup"><span data-stu-id="35d0d-122">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="35d0d-123">altitude</span><span class="sxs-lookup"><span data-stu-id="35d0d-123">altitude</span></span>|<span data-ttu-id="35d0d-124">Двойное</span><span class="sxs-lookup"><span data-stu-id="35d0d-124">Double</span></span>|<span data-ttu-id="35d0d-125">Высота (метров над уровнем моря)</span><span class="sxs-lookup"><span data-stu-id="35d0d-125">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="35d0d-126">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="35d0d-126">horizontalAccuracy</span></span>|<span data-ttu-id="35d0d-127">Двойное</span><span class="sxs-lookup"><span data-stu-id="35d0d-127">Double</span></span>|<span data-ttu-id="35d0d-128">Точность долготы и широты (м)</span><span class="sxs-lookup"><span data-stu-id="35d0d-128">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="35d0d-129">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="35d0d-129">verticalAccuracy</span></span>|<span data-ttu-id="35d0d-130">Двойное</span><span class="sxs-lookup"><span data-stu-id="35d0d-130">Double</span></span>|<span data-ttu-id="35d0d-131">Точность высоты (м)</span><span class="sxs-lookup"><span data-stu-id="35d0d-131">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="35d0d-132">heading</span><span class="sxs-lookup"><span data-stu-id="35d0d-132">heading</span></span>|<span data-ttu-id="35d0d-133">Двойное</span><span class="sxs-lookup"><span data-stu-id="35d0d-133">Double</span></span>|<span data-ttu-id="35d0d-134">Направление от географического севера (градусов)</span><span class="sxs-lookup"><span data-stu-id="35d0d-134">Heading in degrees from true north</span></span>|
|<span data-ttu-id="35d0d-135">speed</span><span class="sxs-lookup"><span data-stu-id="35d0d-135">speed</span></span>|<span data-ttu-id="35d0d-136">Double</span><span class="sxs-lookup"><span data-stu-id="35d0d-136">Double</span></span>|<span data-ttu-id="35d0d-137">Скорость передвижения устройства (м/с)</span><span class="sxs-lookup"><span data-stu-id="35d0d-137">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="35d0d-138">Связи</span><span class="sxs-lookup"><span data-stu-id="35d0d-138">Relationships</span></span>
<span data-ttu-id="35d0d-139">Нет</span><span class="sxs-lookup"><span data-stu-id="35d0d-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35d0d-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35d0d-140">JSON Representation</span></span>
<span data-ttu-id="35d0d-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35d0d-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceGeoLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceGeoLocation",
  "lastCollectedDateTimeUtc": "String (timestamp)",
  "lastCollectedDateTime": "String (timestamp)",
  "longitude": "<Unknown Primitive Type Edm.Double>",
  "latitude": "<Unknown Primitive Type Edm.Double>",
  "altitude": "<Unknown Primitive Type Edm.Double>",
  "horizontalAccuracy": "<Unknown Primitive Type Edm.Double>",
  "verticalAccuracy": "<Unknown Primitive Type Edm.Double>",
  "heading": "<Unknown Primitive Type Edm.Double>",
  "speed": "<Unknown Primitive Type Edm.Double>"
}
```




