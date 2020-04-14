---
title: Тип ресурса deviceGeoLocation
description: Расположение устройства
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f9dc9e4883030936982b9029d1e14242b2a37e37
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43423643"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="791e6-103">Тип ресурса deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="791e6-103">deviceGeoLocation resource type</span></span>

<span data-ttu-id="791e6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="791e6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="791e6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="791e6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="791e6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="791e6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="791e6-107">Расположение устройства</span><span class="sxs-lookup"><span data-stu-id="791e6-107">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="791e6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="791e6-108">Properties</span></span>
|<span data-ttu-id="791e6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="791e6-109">Property</span></span>|<span data-ttu-id="791e6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="791e6-110">Type</span></span>|<span data-ttu-id="791e6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="791e6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="791e6-112">ластколлектеддатетимеутк</span><span class="sxs-lookup"><span data-stu-id="791e6-112">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="791e6-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="791e6-113">DateTimeOffset</span></span>|<span data-ttu-id="791e6-114">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="791e6-114">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="791e6-115">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="791e6-115">lastCollectedDateTime</span></span>|<span data-ttu-id="791e6-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="791e6-116">DateTimeOffset</span></span>|<span data-ttu-id="791e6-117">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="791e6-117">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="791e6-118">longitude</span><span class="sxs-lookup"><span data-stu-id="791e6-118">longitude</span></span>|<span data-ttu-id="791e6-119">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="791e6-119">Double</span></span>|<span data-ttu-id="791e6-120">Долгота расположения устройства</span><span class="sxs-lookup"><span data-stu-id="791e6-120">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="791e6-121">latitude</span><span class="sxs-lookup"><span data-stu-id="791e6-121">latitude</span></span>|<span data-ttu-id="791e6-122">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="791e6-122">Double</span></span>|<span data-ttu-id="791e6-123">Широта расположения устройства</span><span class="sxs-lookup"><span data-stu-id="791e6-123">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="791e6-124">altitude</span><span class="sxs-lookup"><span data-stu-id="791e6-124">altitude</span></span>|<span data-ttu-id="791e6-125">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="791e6-125">Double</span></span>|<span data-ttu-id="791e6-126">Высота (метров над уровнем моря)</span><span class="sxs-lookup"><span data-stu-id="791e6-126">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="791e6-127">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="791e6-127">horizontalAccuracy</span></span>|<span data-ttu-id="791e6-128">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="791e6-128">Double</span></span>|<span data-ttu-id="791e6-129">Точность долготы и широты (м)</span><span class="sxs-lookup"><span data-stu-id="791e6-129">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="791e6-130">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="791e6-130">verticalAccuracy</span></span>|<span data-ttu-id="791e6-131">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="791e6-131">Double</span></span>|<span data-ttu-id="791e6-132">Точность высоты (м)</span><span class="sxs-lookup"><span data-stu-id="791e6-132">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="791e6-133">heading</span><span class="sxs-lookup"><span data-stu-id="791e6-133">heading</span></span>|<span data-ttu-id="791e6-134">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="791e6-134">Double</span></span>|<span data-ttu-id="791e6-135">Направление от географического севера (градусов)</span><span class="sxs-lookup"><span data-stu-id="791e6-135">Heading in degrees from true north</span></span>|
|<span data-ttu-id="791e6-136">speed</span><span class="sxs-lookup"><span data-stu-id="791e6-136">speed</span></span>|<span data-ttu-id="791e6-137">Double</span><span class="sxs-lookup"><span data-stu-id="791e6-137">Double</span></span>|<span data-ttu-id="791e6-138">Скорость передвижения устройства (м/с)</span><span class="sxs-lookup"><span data-stu-id="791e6-138">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="791e6-139">Связи</span><span class="sxs-lookup"><span data-stu-id="791e6-139">Relationships</span></span>
<span data-ttu-id="791e6-140">Нет</span><span class="sxs-lookup"><span data-stu-id="791e6-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="791e6-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="791e6-141">JSON Representation</span></span>
<span data-ttu-id="791e6-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="791e6-142">Here is a JSON representation of the resource.</span></span>
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



