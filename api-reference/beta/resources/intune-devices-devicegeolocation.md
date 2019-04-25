---
title: Тип ресурса deviceGeoLocation
description: Расположение устройства
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: acf2987e7c022754ff0659d82027b4d0d26901bd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524444"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="13720-103">Тип ресурса deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="13720-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="13720-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13720-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13720-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="13720-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13720-106">Расположение устройства</span><span class="sxs-lookup"><span data-stu-id="13720-106">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="13720-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="13720-107">Properties</span></span>
|<span data-ttu-id="13720-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="13720-108">Property</span></span>|<span data-ttu-id="13720-109">Тип</span><span class="sxs-lookup"><span data-stu-id="13720-109">Type</span></span>|<span data-ttu-id="13720-110">Описание</span><span class="sxs-lookup"><span data-stu-id="13720-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13720-111">Ластколлектеддатетимеутк</span><span class="sxs-lookup"><span data-stu-id="13720-111">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="13720-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13720-112">DateTimeOffset</span></span>|<span data-ttu-id="13720-113">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="13720-113">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="13720-114">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="13720-114">lastCollectedDateTime</span></span>|<span data-ttu-id="13720-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13720-115">DateTimeOffset</span></span>|<span data-ttu-id="13720-116">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="13720-116">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="13720-117">longitude</span><span class="sxs-lookup"><span data-stu-id="13720-117">longitude</span></span>|<span data-ttu-id="13720-118">Double</span><span class="sxs-lookup"><span data-stu-id="13720-118">Double</span></span>|<span data-ttu-id="13720-119">Долгота расположения устройства</span><span class="sxs-lookup"><span data-stu-id="13720-119">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="13720-120">latitude</span><span class="sxs-lookup"><span data-stu-id="13720-120">latitude</span></span>|<span data-ttu-id="13720-121">Double</span><span class="sxs-lookup"><span data-stu-id="13720-121">Double</span></span>|<span data-ttu-id="13720-122">Широта расположения устройства</span><span class="sxs-lookup"><span data-stu-id="13720-122">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="13720-123">altitude</span><span class="sxs-lookup"><span data-stu-id="13720-123">altitude</span></span>|<span data-ttu-id="13720-124">Double</span><span class="sxs-lookup"><span data-stu-id="13720-124">Double</span></span>|<span data-ttu-id="13720-125">Высота (метров над уровнем моря)</span><span class="sxs-lookup"><span data-stu-id="13720-125">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="13720-126">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="13720-126">horizontalAccuracy</span></span>|<span data-ttu-id="13720-127">Double</span><span class="sxs-lookup"><span data-stu-id="13720-127">Double</span></span>|<span data-ttu-id="13720-128">Точность долготы и широты (м)</span><span class="sxs-lookup"><span data-stu-id="13720-128">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="13720-129">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="13720-129">verticalAccuracy</span></span>|<span data-ttu-id="13720-130">Double</span><span class="sxs-lookup"><span data-stu-id="13720-130">Double</span></span>|<span data-ttu-id="13720-131">Точность высоты (м)</span><span class="sxs-lookup"><span data-stu-id="13720-131">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="13720-132">heading</span><span class="sxs-lookup"><span data-stu-id="13720-132">heading</span></span>|<span data-ttu-id="13720-133">Double</span><span class="sxs-lookup"><span data-stu-id="13720-133">Double</span></span>|<span data-ttu-id="13720-134">Направление от географического севера (градусов)</span><span class="sxs-lookup"><span data-stu-id="13720-134">Heading in degrees from true north</span></span>|
|<span data-ttu-id="13720-135">speed</span><span class="sxs-lookup"><span data-stu-id="13720-135">speed</span></span>|<span data-ttu-id="13720-136">Double</span><span class="sxs-lookup"><span data-stu-id="13720-136">Double</span></span>|<span data-ttu-id="13720-137">Скорость передвижения устройства (м/с)</span><span class="sxs-lookup"><span data-stu-id="13720-137">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="13720-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="13720-138">Relationships</span></span>
<span data-ttu-id="13720-139">Нет</span><span class="sxs-lookup"><span data-stu-id="13720-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="13720-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="13720-140">JSON Representation</span></span>
<span data-ttu-id="13720-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13720-141">Here is a JSON representation of the resource.</span></span>
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





