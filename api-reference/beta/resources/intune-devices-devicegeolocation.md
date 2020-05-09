---
title: Тип ресурса deviceGeoLocation
description: Расположение устройства
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 896f463daadef157b9f8c10628dd9101508b88f0
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44175646"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="b60bf-103">Тип ресурса deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="b60bf-103">deviceGeoLocation resource type</span></span>

<span data-ttu-id="b60bf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b60bf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b60bf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b60bf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b60bf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b60bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b60bf-107">Расположение устройства</span><span class="sxs-lookup"><span data-stu-id="b60bf-107">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="b60bf-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b60bf-108">Properties</span></span>
|<span data-ttu-id="b60bf-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b60bf-109">Property</span></span>|<span data-ttu-id="b60bf-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b60bf-110">Type</span></span>|<span data-ttu-id="b60bf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b60bf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b60bf-112">ластколлектеддатетимеутк</span><span class="sxs-lookup"><span data-stu-id="b60bf-112">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="b60bf-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b60bf-113">DateTimeOffset</span></span>|<span data-ttu-id="b60bf-114">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="b60bf-114">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="b60bf-115">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="b60bf-115">lastCollectedDateTime</span></span>|<span data-ttu-id="b60bf-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b60bf-116">DateTimeOffset</span></span>|<span data-ttu-id="b60bf-117">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="b60bf-117">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="b60bf-118">longitude</span><span class="sxs-lookup"><span data-stu-id="b60bf-118">longitude</span></span>|<span data-ttu-id="b60bf-119">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="b60bf-119">Double</span></span>|<span data-ttu-id="b60bf-120">Долгота расположения устройства</span><span class="sxs-lookup"><span data-stu-id="b60bf-120">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="b60bf-121">latitude</span><span class="sxs-lookup"><span data-stu-id="b60bf-121">latitude</span></span>|<span data-ttu-id="b60bf-122">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="b60bf-122">Double</span></span>|<span data-ttu-id="b60bf-123">Широта расположения устройства</span><span class="sxs-lookup"><span data-stu-id="b60bf-123">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="b60bf-124">altitude</span><span class="sxs-lookup"><span data-stu-id="b60bf-124">altitude</span></span>|<span data-ttu-id="b60bf-125">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="b60bf-125">Double</span></span>|<span data-ttu-id="b60bf-126">Высота (метров над уровнем моря)</span><span class="sxs-lookup"><span data-stu-id="b60bf-126">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="b60bf-127">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="b60bf-127">horizontalAccuracy</span></span>|<span data-ttu-id="b60bf-128">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="b60bf-128">Double</span></span>|<span data-ttu-id="b60bf-129">Точность долготы и широты (м)</span><span class="sxs-lookup"><span data-stu-id="b60bf-129">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="b60bf-130">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="b60bf-130">verticalAccuracy</span></span>|<span data-ttu-id="b60bf-131">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="b60bf-131">Double</span></span>|<span data-ttu-id="b60bf-132">Точность высоты (м)</span><span class="sxs-lookup"><span data-stu-id="b60bf-132">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="b60bf-133">heading</span><span class="sxs-lookup"><span data-stu-id="b60bf-133">heading</span></span>|<span data-ttu-id="b60bf-134">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="b60bf-134">Double</span></span>|<span data-ttu-id="b60bf-135">Направление от географического севера (градусов)</span><span class="sxs-lookup"><span data-stu-id="b60bf-135">Heading in degrees from true north</span></span>|
|<span data-ttu-id="b60bf-136">speed</span><span class="sxs-lookup"><span data-stu-id="b60bf-136">speed</span></span>|<span data-ttu-id="b60bf-137">Double</span><span class="sxs-lookup"><span data-stu-id="b60bf-137">Double</span></span>|<span data-ttu-id="b60bf-138">Скорость передвижения устройства (м/с)</span><span class="sxs-lookup"><span data-stu-id="b60bf-138">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="b60bf-139">Связи</span><span class="sxs-lookup"><span data-stu-id="b60bf-139">Relationships</span></span>
<span data-ttu-id="b60bf-140">Нет</span><span class="sxs-lookup"><span data-stu-id="b60bf-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b60bf-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b60bf-141">JSON Representation</span></span>
<span data-ttu-id="b60bf-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b60bf-142">Here is a JSON representation of the resource.</span></span>
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



