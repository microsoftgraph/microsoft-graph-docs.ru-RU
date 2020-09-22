---
title: Тип ресурса deviceGeoLocation
description: Расположение устройства
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c189b21570dcc218586f4cc74cd605aa6712f0c1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060484"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="28a8d-103">Тип ресурса deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="28a8d-103">deviceGeoLocation resource type</span></span>

<span data-ttu-id="28a8d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28a8d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="28a8d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28a8d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28a8d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="28a8d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28a8d-107">Расположение устройства</span><span class="sxs-lookup"><span data-stu-id="28a8d-107">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="28a8d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="28a8d-108">Properties</span></span>
|<span data-ttu-id="28a8d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="28a8d-109">Property</span></span>|<span data-ttu-id="28a8d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="28a8d-110">Type</span></span>|<span data-ttu-id="28a8d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="28a8d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28a8d-112">ластколлектеддатетимеутк</span><span class="sxs-lookup"><span data-stu-id="28a8d-112">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="28a8d-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28a8d-113">DateTimeOffset</span></span>|<span data-ttu-id="28a8d-114">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="28a8d-114">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="28a8d-115">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="28a8d-115">lastCollectedDateTime</span></span>|<span data-ttu-id="28a8d-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28a8d-116">DateTimeOffset</span></span>|<span data-ttu-id="28a8d-117">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="28a8d-117">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="28a8d-118">longitude</span><span class="sxs-lookup"><span data-stu-id="28a8d-118">longitude</span></span>|<span data-ttu-id="28a8d-119">Double</span><span class="sxs-lookup"><span data-stu-id="28a8d-119">Double</span></span>|<span data-ttu-id="28a8d-120">Долгота расположения устройства</span><span class="sxs-lookup"><span data-stu-id="28a8d-120">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="28a8d-121">latitude</span><span class="sxs-lookup"><span data-stu-id="28a8d-121">latitude</span></span>|<span data-ttu-id="28a8d-122">Double</span><span class="sxs-lookup"><span data-stu-id="28a8d-122">Double</span></span>|<span data-ttu-id="28a8d-123">Широта расположения устройства</span><span class="sxs-lookup"><span data-stu-id="28a8d-123">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="28a8d-124">altitude</span><span class="sxs-lookup"><span data-stu-id="28a8d-124">altitude</span></span>|<span data-ttu-id="28a8d-125">Double</span><span class="sxs-lookup"><span data-stu-id="28a8d-125">Double</span></span>|<span data-ttu-id="28a8d-126">Высота (метров над уровнем моря)</span><span class="sxs-lookup"><span data-stu-id="28a8d-126">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="28a8d-127">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="28a8d-127">horizontalAccuracy</span></span>|<span data-ttu-id="28a8d-128">Double</span><span class="sxs-lookup"><span data-stu-id="28a8d-128">Double</span></span>|<span data-ttu-id="28a8d-129">Точность долготы и широты (м)</span><span class="sxs-lookup"><span data-stu-id="28a8d-129">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="28a8d-130">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="28a8d-130">verticalAccuracy</span></span>|<span data-ttu-id="28a8d-131">Double</span><span class="sxs-lookup"><span data-stu-id="28a8d-131">Double</span></span>|<span data-ttu-id="28a8d-132">Точность высоты (м)</span><span class="sxs-lookup"><span data-stu-id="28a8d-132">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="28a8d-133">heading</span><span class="sxs-lookup"><span data-stu-id="28a8d-133">heading</span></span>|<span data-ttu-id="28a8d-134">Double</span><span class="sxs-lookup"><span data-stu-id="28a8d-134">Double</span></span>|<span data-ttu-id="28a8d-135">Направление от географического севера (градусов)</span><span class="sxs-lookup"><span data-stu-id="28a8d-135">Heading in degrees from true north</span></span>|
|<span data-ttu-id="28a8d-136">speed</span><span class="sxs-lookup"><span data-stu-id="28a8d-136">speed</span></span>|<span data-ttu-id="28a8d-137">Double</span><span class="sxs-lookup"><span data-stu-id="28a8d-137">Double</span></span>|<span data-ttu-id="28a8d-138">Скорость передвижения устройства (м/с)</span><span class="sxs-lookup"><span data-stu-id="28a8d-138">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="28a8d-139">Связи</span><span class="sxs-lookup"><span data-stu-id="28a8d-139">Relationships</span></span>
<span data-ttu-id="28a8d-140">Нет</span><span class="sxs-lookup"><span data-stu-id="28a8d-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="28a8d-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="28a8d-141">JSON Representation</span></span>
<span data-ttu-id="28a8d-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28a8d-142">Here is a JSON representation of the resource.</span></span>
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
  "longitude": "4.2",
  "latitude": "4.2",
  "altitude": "4.2",
  "horizontalAccuracy": "4.2",
  "verticalAccuracy": "4.2",
  "heading": "4.2",
  "speed": "4.2"
}
```






