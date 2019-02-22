---
title: Тип ресурса deviceGeoLocation
description: Расположение устройства
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1eaa46929ae627dbf6cdee8d300b7910b4817ffc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149604"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="bd7b6-103">Тип ресурса deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="bd7b6-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="bd7b6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd7b6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd7b6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bd7b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd7b6-106">Расположение устройства</span><span class="sxs-lookup"><span data-stu-id="bd7b6-106">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="bd7b6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bd7b6-107">Properties</span></span>
|<span data-ttu-id="bd7b6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd7b6-108">Property</span></span>|<span data-ttu-id="bd7b6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bd7b6-109">Type</span></span>|<span data-ttu-id="bd7b6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bd7b6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd7b6-111">Ластколлектеддатетимеутк</span><span class="sxs-lookup"><span data-stu-id="bd7b6-111">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="bd7b6-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd7b6-112">DateTimeOffset</span></span>|<span data-ttu-id="bd7b6-113">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="bd7b6-113">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="bd7b6-114">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="bd7b6-114">lastCollectedDateTime</span></span>|<span data-ttu-id="bd7b6-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd7b6-115">DateTimeOffset</span></span>|<span data-ttu-id="bd7b6-116">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="bd7b6-116">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="bd7b6-117">longitude</span><span class="sxs-lookup"><span data-stu-id="bd7b6-117">longitude</span></span>|<span data-ttu-id="bd7b6-118">Double</span><span class="sxs-lookup"><span data-stu-id="bd7b6-118">Double</span></span>|<span data-ttu-id="bd7b6-119">Долгота расположения устройства</span><span class="sxs-lookup"><span data-stu-id="bd7b6-119">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="bd7b6-120">latitude</span><span class="sxs-lookup"><span data-stu-id="bd7b6-120">latitude</span></span>|<span data-ttu-id="bd7b6-121">Double</span><span class="sxs-lookup"><span data-stu-id="bd7b6-121">Double</span></span>|<span data-ttu-id="bd7b6-122">Широта расположения устройства</span><span class="sxs-lookup"><span data-stu-id="bd7b6-122">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="bd7b6-123">altitude</span><span class="sxs-lookup"><span data-stu-id="bd7b6-123">altitude</span></span>|<span data-ttu-id="bd7b6-124">Double</span><span class="sxs-lookup"><span data-stu-id="bd7b6-124">Double</span></span>|<span data-ttu-id="bd7b6-125">Высота (метров над уровнем моря)</span><span class="sxs-lookup"><span data-stu-id="bd7b6-125">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="bd7b6-126">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="bd7b6-126">horizontalAccuracy</span></span>|<span data-ttu-id="bd7b6-127">Double</span><span class="sxs-lookup"><span data-stu-id="bd7b6-127">Double</span></span>|<span data-ttu-id="bd7b6-128">Точность долготы и широты (м)</span><span class="sxs-lookup"><span data-stu-id="bd7b6-128">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="bd7b6-129">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="bd7b6-129">verticalAccuracy</span></span>|<span data-ttu-id="bd7b6-130">Double</span><span class="sxs-lookup"><span data-stu-id="bd7b6-130">Double</span></span>|<span data-ttu-id="bd7b6-131">Точность высоты (м)</span><span class="sxs-lookup"><span data-stu-id="bd7b6-131">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="bd7b6-132">heading</span><span class="sxs-lookup"><span data-stu-id="bd7b6-132">heading</span></span>|<span data-ttu-id="bd7b6-133">Double</span><span class="sxs-lookup"><span data-stu-id="bd7b6-133">Double</span></span>|<span data-ttu-id="bd7b6-134">Направление от географического севера (градусов)</span><span class="sxs-lookup"><span data-stu-id="bd7b6-134">Heading in degrees from true north</span></span>|
|<span data-ttu-id="bd7b6-135">speed</span><span class="sxs-lookup"><span data-stu-id="bd7b6-135">speed</span></span>|<span data-ttu-id="bd7b6-136">Double</span><span class="sxs-lookup"><span data-stu-id="bd7b6-136">Double</span></span>|<span data-ttu-id="bd7b6-137">Скорость передвижения устройства (м/с)</span><span class="sxs-lookup"><span data-stu-id="bd7b6-137">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd7b6-138">Связи</span><span class="sxs-lookup"><span data-stu-id="bd7b6-138">Relationships</span></span>
<span data-ttu-id="bd7b6-139">Нет</span><span class="sxs-lookup"><span data-stu-id="bd7b6-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd7b6-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bd7b6-140">JSON Representation</span></span>
<span data-ttu-id="bd7b6-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd7b6-141">Here is a JSON representation of the resource.</span></span>
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




