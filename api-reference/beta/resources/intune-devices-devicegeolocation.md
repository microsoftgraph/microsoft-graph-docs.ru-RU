---
title: Тип ресурса deviceGeoLocation
description: Расположение устройства
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 44c4b6285bc291001c35a5dd0d9580596599247f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983108"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="3290a-103">Тип ресурса deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="3290a-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="3290a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3290a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3290a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3290a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3290a-106">Расположение устройства</span><span class="sxs-lookup"><span data-stu-id="3290a-106">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="3290a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3290a-107">Properties</span></span>
|<span data-ttu-id="3290a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3290a-108">Property</span></span>|<span data-ttu-id="3290a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3290a-109">Type</span></span>|<span data-ttu-id="3290a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3290a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3290a-111">Ластколлектеддатетимеутк</span><span class="sxs-lookup"><span data-stu-id="3290a-111">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="3290a-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3290a-112">DateTimeOffset</span></span>|<span data-ttu-id="3290a-113">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="3290a-113">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="3290a-114">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="3290a-114">lastCollectedDateTime</span></span>|<span data-ttu-id="3290a-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3290a-115">DateTimeOffset</span></span>|<span data-ttu-id="3290a-116">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="3290a-116">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="3290a-117">longitude</span><span class="sxs-lookup"><span data-stu-id="3290a-117">longitude</span></span>|<span data-ttu-id="3290a-118">Двойное</span><span class="sxs-lookup"><span data-stu-id="3290a-118">Double</span></span>|<span data-ttu-id="3290a-119">Долгота расположения устройства</span><span class="sxs-lookup"><span data-stu-id="3290a-119">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="3290a-120">latitude</span><span class="sxs-lookup"><span data-stu-id="3290a-120">latitude</span></span>|<span data-ttu-id="3290a-121">Двойное</span><span class="sxs-lookup"><span data-stu-id="3290a-121">Double</span></span>|<span data-ttu-id="3290a-122">Широта расположения устройства</span><span class="sxs-lookup"><span data-stu-id="3290a-122">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="3290a-123">altitude</span><span class="sxs-lookup"><span data-stu-id="3290a-123">altitude</span></span>|<span data-ttu-id="3290a-124">Двойное</span><span class="sxs-lookup"><span data-stu-id="3290a-124">Double</span></span>|<span data-ttu-id="3290a-125">Высота (метров над уровнем моря)</span><span class="sxs-lookup"><span data-stu-id="3290a-125">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="3290a-126">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="3290a-126">horizontalAccuracy</span></span>|<span data-ttu-id="3290a-127">Двойное</span><span class="sxs-lookup"><span data-stu-id="3290a-127">Double</span></span>|<span data-ttu-id="3290a-128">Точность долготы и широты (м)</span><span class="sxs-lookup"><span data-stu-id="3290a-128">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="3290a-129">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="3290a-129">verticalAccuracy</span></span>|<span data-ttu-id="3290a-130">Двойное</span><span class="sxs-lookup"><span data-stu-id="3290a-130">Double</span></span>|<span data-ttu-id="3290a-131">Точность высоты (м)</span><span class="sxs-lookup"><span data-stu-id="3290a-131">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="3290a-132">heading</span><span class="sxs-lookup"><span data-stu-id="3290a-132">heading</span></span>|<span data-ttu-id="3290a-133">Двойное</span><span class="sxs-lookup"><span data-stu-id="3290a-133">Double</span></span>|<span data-ttu-id="3290a-134">Направление от географического севера (градусов)</span><span class="sxs-lookup"><span data-stu-id="3290a-134">Heading in degrees from true north</span></span>|
|<span data-ttu-id="3290a-135">speed</span><span class="sxs-lookup"><span data-stu-id="3290a-135">speed</span></span>|<span data-ttu-id="3290a-136">Double</span><span class="sxs-lookup"><span data-stu-id="3290a-136">Double</span></span>|<span data-ttu-id="3290a-137">Скорость передвижения устройства (м/с)</span><span class="sxs-lookup"><span data-stu-id="3290a-137">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="3290a-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="3290a-138">Relationships</span></span>
<span data-ttu-id="3290a-139">Нет</span><span class="sxs-lookup"><span data-stu-id="3290a-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3290a-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3290a-140">JSON Representation</span></span>
<span data-ttu-id="3290a-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3290a-141">Here is a JSON representation of the resource.</span></span>
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





