---
title: Тип ресурса deviceGeoLocation
description: Расположение устройства
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a406ede926ad637a338437559840cdefdadc64ce
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754583"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="204d8-103">Тип ресурса deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="204d8-103">deviceGeoLocation resource type</span></span>

<span data-ttu-id="204d8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="204d8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="204d8-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="204d8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="204d8-106">Расположение устройства</span><span class="sxs-lookup"><span data-stu-id="204d8-106">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="204d8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="204d8-107">Properties</span></span>
|<span data-ttu-id="204d8-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="204d8-108">Property</span></span>|<span data-ttu-id="204d8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="204d8-109">Type</span></span>|<span data-ttu-id="204d8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="204d8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="204d8-111">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="204d8-111">lastCollectedDateTime</span></span>|<span data-ttu-id="204d8-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="204d8-112">DateTimeOffset</span></span>|<span data-ttu-id="204d8-113">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="204d8-113">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="204d8-114">longitude</span><span class="sxs-lookup"><span data-stu-id="204d8-114">longitude</span></span>|<span data-ttu-id="204d8-115">Double</span><span class="sxs-lookup"><span data-stu-id="204d8-115">Double</span></span>|<span data-ttu-id="204d8-116">Долгота расположения устройства</span><span class="sxs-lookup"><span data-stu-id="204d8-116">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="204d8-117">latitude</span><span class="sxs-lookup"><span data-stu-id="204d8-117">latitude</span></span>|<span data-ttu-id="204d8-118">Double</span><span class="sxs-lookup"><span data-stu-id="204d8-118">Double</span></span>|<span data-ttu-id="204d8-119">Широта расположения устройства</span><span class="sxs-lookup"><span data-stu-id="204d8-119">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="204d8-120">altitude</span><span class="sxs-lookup"><span data-stu-id="204d8-120">altitude</span></span>|<span data-ttu-id="204d8-121">Double</span><span class="sxs-lookup"><span data-stu-id="204d8-121">Double</span></span>|<span data-ttu-id="204d8-122">Высота (метров над уровнем моря)</span><span class="sxs-lookup"><span data-stu-id="204d8-122">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="204d8-123">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="204d8-123">horizontalAccuracy</span></span>|<span data-ttu-id="204d8-124">Double</span><span class="sxs-lookup"><span data-stu-id="204d8-124">Double</span></span>|<span data-ttu-id="204d8-125">Точность долготы и широты (м)</span><span class="sxs-lookup"><span data-stu-id="204d8-125">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="204d8-126">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="204d8-126">verticalAccuracy</span></span>|<span data-ttu-id="204d8-127">Double</span><span class="sxs-lookup"><span data-stu-id="204d8-127">Double</span></span>|<span data-ttu-id="204d8-128">Точность высоты (м)</span><span class="sxs-lookup"><span data-stu-id="204d8-128">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="204d8-129">heading</span><span class="sxs-lookup"><span data-stu-id="204d8-129">heading</span></span>|<span data-ttu-id="204d8-130">Double</span><span class="sxs-lookup"><span data-stu-id="204d8-130">Double</span></span>|<span data-ttu-id="204d8-131">Направление от географического севера (градусов)</span><span class="sxs-lookup"><span data-stu-id="204d8-131">Heading in degrees from true north</span></span>|
|<span data-ttu-id="204d8-132">speed</span><span class="sxs-lookup"><span data-stu-id="204d8-132">speed</span></span>|<span data-ttu-id="204d8-133">Double</span><span class="sxs-lookup"><span data-stu-id="204d8-133">Double</span></span>|<span data-ttu-id="204d8-134">Скорость передвижения устройства (м/с)</span><span class="sxs-lookup"><span data-stu-id="204d8-134">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="204d8-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="204d8-135">Relationships</span></span>
<span data-ttu-id="204d8-136">Нет</span><span class="sxs-lookup"><span data-stu-id="204d8-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="204d8-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="204d8-137">JSON Representation</span></span>
<span data-ttu-id="204d8-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="204d8-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceGeoLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceGeoLocation",
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




