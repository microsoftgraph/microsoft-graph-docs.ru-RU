---
title: Тип ресурса deviceGeoLocation
description: Расположение устройства
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 091ef44a52e20acb987adddbac1c561087db718c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43368314"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="cbec3-103">Тип ресурса deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="cbec3-103">deviceGeoLocation resource type</span></span>

<span data-ttu-id="cbec3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cbec3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cbec3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cbec3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbec3-106">Расположение устройства</span><span class="sxs-lookup"><span data-stu-id="cbec3-106">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="cbec3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="cbec3-107">Properties</span></span>
|<span data-ttu-id="cbec3-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="cbec3-108">Property</span></span>|<span data-ttu-id="cbec3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="cbec3-109">Type</span></span>|<span data-ttu-id="cbec3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cbec3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbec3-111">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="cbec3-111">lastCollectedDateTime</span></span>|<span data-ttu-id="cbec3-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbec3-112">DateTimeOffset</span></span>|<span data-ttu-id="cbec3-113">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="cbec3-113">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="cbec3-114">longitude</span><span class="sxs-lookup"><span data-stu-id="cbec3-114">longitude</span></span>|<span data-ttu-id="cbec3-115">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="cbec3-115">Double</span></span>|<span data-ttu-id="cbec3-116">Долгота расположения устройства</span><span class="sxs-lookup"><span data-stu-id="cbec3-116">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="cbec3-117">latitude</span><span class="sxs-lookup"><span data-stu-id="cbec3-117">latitude</span></span>|<span data-ttu-id="cbec3-118">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="cbec3-118">Double</span></span>|<span data-ttu-id="cbec3-119">Широта расположения устройства</span><span class="sxs-lookup"><span data-stu-id="cbec3-119">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="cbec3-120">altitude</span><span class="sxs-lookup"><span data-stu-id="cbec3-120">altitude</span></span>|<span data-ttu-id="cbec3-121">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="cbec3-121">Double</span></span>|<span data-ttu-id="cbec3-122">Высота (метров над уровнем моря)</span><span class="sxs-lookup"><span data-stu-id="cbec3-122">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="cbec3-123">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="cbec3-123">horizontalAccuracy</span></span>|<span data-ttu-id="cbec3-124">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="cbec3-124">Double</span></span>|<span data-ttu-id="cbec3-125">Точность долготы и широты (м)</span><span class="sxs-lookup"><span data-stu-id="cbec3-125">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="cbec3-126">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="cbec3-126">verticalAccuracy</span></span>|<span data-ttu-id="cbec3-127">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="cbec3-127">Double</span></span>|<span data-ttu-id="cbec3-128">Точность высоты (м)</span><span class="sxs-lookup"><span data-stu-id="cbec3-128">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="cbec3-129">heading</span><span class="sxs-lookup"><span data-stu-id="cbec3-129">heading</span></span>|<span data-ttu-id="cbec3-130">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="cbec3-130">Double</span></span>|<span data-ttu-id="cbec3-131">Направление от географического севера (градусов)</span><span class="sxs-lookup"><span data-stu-id="cbec3-131">Heading in degrees from true north</span></span>|
|<span data-ttu-id="cbec3-132">speed</span><span class="sxs-lookup"><span data-stu-id="cbec3-132">speed</span></span>|<span data-ttu-id="cbec3-133">Double</span><span class="sxs-lookup"><span data-stu-id="cbec3-133">Double</span></span>|<span data-ttu-id="cbec3-134">Скорость передвижения устройства (м/с)</span><span class="sxs-lookup"><span data-stu-id="cbec3-134">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="cbec3-135">Связи</span><span class="sxs-lookup"><span data-stu-id="cbec3-135">Relationships</span></span>
<span data-ttu-id="cbec3-136">Нет</span><span class="sxs-lookup"><span data-stu-id="cbec3-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cbec3-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cbec3-137">JSON Representation</span></span>
<span data-ttu-id="cbec3-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cbec3-138">Here is a JSON representation of the resource.</span></span>
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







