---
title: Тип ресурса deviceGeoLocation
description: Расположение устройства
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: acf2987e7c022754ff0659d82027b4d0d26901bd
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31772176"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="4507e-103">Тип ресурса deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="4507e-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="4507e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4507e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4507e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4507e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4507e-106">Расположение устройства</span><span class="sxs-lookup"><span data-stu-id="4507e-106">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="4507e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4507e-107">Properties</span></span>
|<span data-ttu-id="4507e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4507e-108">Property</span></span>|<span data-ttu-id="4507e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4507e-109">Type</span></span>|<span data-ttu-id="4507e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4507e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4507e-111">Ластколлектеддатетимеутк</span><span class="sxs-lookup"><span data-stu-id="4507e-111">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="4507e-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4507e-112">DateTimeOffset</span></span>|<span data-ttu-id="4507e-113">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="4507e-113">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="4507e-114">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="4507e-114">lastCollectedDateTime</span></span>|<span data-ttu-id="4507e-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4507e-115">DateTimeOffset</span></span>|<span data-ttu-id="4507e-116">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="4507e-116">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="4507e-117">longitude</span><span class="sxs-lookup"><span data-stu-id="4507e-117">longitude</span></span>|<span data-ttu-id="4507e-118">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="4507e-118">Double</span></span>|<span data-ttu-id="4507e-119">Долгота расположения устройства</span><span class="sxs-lookup"><span data-stu-id="4507e-119">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="4507e-120">latitude</span><span class="sxs-lookup"><span data-stu-id="4507e-120">latitude</span></span>|<span data-ttu-id="4507e-121">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="4507e-121">Double</span></span>|<span data-ttu-id="4507e-122">Широта расположения устройства</span><span class="sxs-lookup"><span data-stu-id="4507e-122">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="4507e-123">altitude</span><span class="sxs-lookup"><span data-stu-id="4507e-123">altitude</span></span>|<span data-ttu-id="4507e-124">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="4507e-124">Double</span></span>|<span data-ttu-id="4507e-125">Высота (метров над уровнем моря)</span><span class="sxs-lookup"><span data-stu-id="4507e-125">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="4507e-126">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="4507e-126">horizontalAccuracy</span></span>|<span data-ttu-id="4507e-127">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="4507e-127">Double</span></span>|<span data-ttu-id="4507e-128">Точность долготы и широты (м)</span><span class="sxs-lookup"><span data-stu-id="4507e-128">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="4507e-129">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="4507e-129">verticalAccuracy</span></span>|<span data-ttu-id="4507e-130">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="4507e-130">Double</span></span>|<span data-ttu-id="4507e-131">Точность высоты (м)</span><span class="sxs-lookup"><span data-stu-id="4507e-131">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="4507e-132">heading</span><span class="sxs-lookup"><span data-stu-id="4507e-132">heading</span></span>|<span data-ttu-id="4507e-133">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="4507e-133">Double</span></span>|<span data-ttu-id="4507e-134">Направление от географического севера (градусов)</span><span class="sxs-lookup"><span data-stu-id="4507e-134">Heading in degrees from true north</span></span>|
|<span data-ttu-id="4507e-135">speed</span><span class="sxs-lookup"><span data-stu-id="4507e-135">speed</span></span>|<span data-ttu-id="4507e-136">Double</span><span class="sxs-lookup"><span data-stu-id="4507e-136">Double</span></span>|<span data-ttu-id="4507e-137">Скорость передвижения устройства (м/с)</span><span class="sxs-lookup"><span data-stu-id="4507e-137">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="4507e-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="4507e-138">Relationships</span></span>
<span data-ttu-id="4507e-139">Нет</span><span class="sxs-lookup"><span data-stu-id="4507e-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4507e-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4507e-140">JSON Representation</span></span>
<span data-ttu-id="4507e-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4507e-141">Here is a JSON representation of the resource.</span></span>
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





