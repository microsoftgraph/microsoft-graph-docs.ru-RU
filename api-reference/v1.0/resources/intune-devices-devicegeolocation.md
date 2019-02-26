---
title: Тип ресурса deviceGeoLocation
description: Расположение устройства
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b51768aea1338486431ceffadd95f8760a7216ab
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260216"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="6a2bc-103">Тип ресурса deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="6a2bc-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="6a2bc-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6a2bc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a2bc-105">Расположение устройства</span><span class="sxs-lookup"><span data-stu-id="6a2bc-105">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="6a2bc-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6a2bc-106">Properties</span></span>
|<span data-ttu-id="6a2bc-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a2bc-107">Property</span></span>|<span data-ttu-id="6a2bc-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6a2bc-108">Type</span></span>|<span data-ttu-id="6a2bc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6a2bc-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a2bc-110">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a2bc-110">lastCollectedDateTime</span></span>|<span data-ttu-id="6a2bc-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a2bc-111">DateTimeOffset</span></span>|<span data-ttu-id="6a2bc-112">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="6a2bc-112">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="6a2bc-113">longitude</span><span class="sxs-lookup"><span data-stu-id="6a2bc-113">longitude</span></span>|<span data-ttu-id="6a2bc-114">Double</span><span class="sxs-lookup"><span data-stu-id="6a2bc-114">Double</span></span>|<span data-ttu-id="6a2bc-115">Долгота расположения устройства</span><span class="sxs-lookup"><span data-stu-id="6a2bc-115">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="6a2bc-116">latitude</span><span class="sxs-lookup"><span data-stu-id="6a2bc-116">latitude</span></span>|<span data-ttu-id="6a2bc-117">Double</span><span class="sxs-lookup"><span data-stu-id="6a2bc-117">Double</span></span>|<span data-ttu-id="6a2bc-118">Широта расположения устройства</span><span class="sxs-lookup"><span data-stu-id="6a2bc-118">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="6a2bc-119">altitude</span><span class="sxs-lookup"><span data-stu-id="6a2bc-119">altitude</span></span>|<span data-ttu-id="6a2bc-120">Double</span><span class="sxs-lookup"><span data-stu-id="6a2bc-120">Double</span></span>|<span data-ttu-id="6a2bc-121">Высота (метров над уровнем моря)</span><span class="sxs-lookup"><span data-stu-id="6a2bc-121">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="6a2bc-122">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="6a2bc-122">horizontalAccuracy</span></span>|<span data-ttu-id="6a2bc-123">Double</span><span class="sxs-lookup"><span data-stu-id="6a2bc-123">Double</span></span>|<span data-ttu-id="6a2bc-124">Точность долготы и широты (м)</span><span class="sxs-lookup"><span data-stu-id="6a2bc-124">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="6a2bc-125">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="6a2bc-125">verticalAccuracy</span></span>|<span data-ttu-id="6a2bc-126">Double</span><span class="sxs-lookup"><span data-stu-id="6a2bc-126">Double</span></span>|<span data-ttu-id="6a2bc-127">Точность высоты (м)</span><span class="sxs-lookup"><span data-stu-id="6a2bc-127">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="6a2bc-128">heading</span><span class="sxs-lookup"><span data-stu-id="6a2bc-128">heading</span></span>|<span data-ttu-id="6a2bc-129">Double</span><span class="sxs-lookup"><span data-stu-id="6a2bc-129">Double</span></span>|<span data-ttu-id="6a2bc-130">Направление от географического севера (градусов)</span><span class="sxs-lookup"><span data-stu-id="6a2bc-130">Heading in degrees from true north</span></span>|
|<span data-ttu-id="6a2bc-131">speed</span><span class="sxs-lookup"><span data-stu-id="6a2bc-131">speed</span></span>|<span data-ttu-id="6a2bc-132">Double</span><span class="sxs-lookup"><span data-stu-id="6a2bc-132">Double</span></span>|<span data-ttu-id="6a2bc-133">Скорость передвижения устройства (м/с)</span><span class="sxs-lookup"><span data-stu-id="6a2bc-133">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a2bc-134">Связи</span><span class="sxs-lookup"><span data-stu-id="6a2bc-134">Relationships</span></span>
<span data-ttu-id="6a2bc-135">Нет</span><span class="sxs-lookup"><span data-stu-id="6a2bc-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a2bc-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6a2bc-136">JSON Representation</span></span>
<span data-ttu-id="6a2bc-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a2bc-137">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceGeoLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceGeoLocation",
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



