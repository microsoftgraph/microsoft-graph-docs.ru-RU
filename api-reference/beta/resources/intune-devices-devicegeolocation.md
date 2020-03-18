---
title: Тип ресурса deviceGeoLocation
description: Расположение устройства
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3c3c8251987dee0aadafdb88eebd9e29afbb5f76
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785002"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="fa51a-103">Тип ресурса deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="fa51a-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="fa51a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa51a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa51a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fa51a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa51a-106">Расположение устройства</span><span class="sxs-lookup"><span data-stu-id="fa51a-106">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="fa51a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="fa51a-107">Properties</span></span>
|<span data-ttu-id="fa51a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa51a-108">Property</span></span>|<span data-ttu-id="fa51a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="fa51a-109">Type</span></span>|<span data-ttu-id="fa51a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fa51a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa51a-111">ластколлектеддатетимеутк</span><span class="sxs-lookup"><span data-stu-id="fa51a-111">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="fa51a-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa51a-112">DateTimeOffset</span></span>|<span data-ttu-id="fa51a-113">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="fa51a-113">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="fa51a-114">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa51a-114">lastCollectedDateTime</span></span>|<span data-ttu-id="fa51a-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa51a-115">DateTimeOffset</span></span>|<span data-ttu-id="fa51a-116">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="fa51a-116">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="fa51a-117">longitude</span><span class="sxs-lookup"><span data-stu-id="fa51a-117">longitude</span></span>|<span data-ttu-id="fa51a-118">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="fa51a-118">Double</span></span>|<span data-ttu-id="fa51a-119">Долгота расположения устройства</span><span class="sxs-lookup"><span data-stu-id="fa51a-119">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="fa51a-120">latitude</span><span class="sxs-lookup"><span data-stu-id="fa51a-120">latitude</span></span>|<span data-ttu-id="fa51a-121">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="fa51a-121">Double</span></span>|<span data-ttu-id="fa51a-122">Широта расположения устройства</span><span class="sxs-lookup"><span data-stu-id="fa51a-122">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="fa51a-123">altitude</span><span class="sxs-lookup"><span data-stu-id="fa51a-123">altitude</span></span>|<span data-ttu-id="fa51a-124">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="fa51a-124">Double</span></span>|<span data-ttu-id="fa51a-125">Высота (метров над уровнем моря)</span><span class="sxs-lookup"><span data-stu-id="fa51a-125">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="fa51a-126">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="fa51a-126">horizontalAccuracy</span></span>|<span data-ttu-id="fa51a-127">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="fa51a-127">Double</span></span>|<span data-ttu-id="fa51a-128">Точность долготы и широты (м)</span><span class="sxs-lookup"><span data-stu-id="fa51a-128">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="fa51a-129">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="fa51a-129">verticalAccuracy</span></span>|<span data-ttu-id="fa51a-130">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="fa51a-130">Double</span></span>|<span data-ttu-id="fa51a-131">Точность высоты (м)</span><span class="sxs-lookup"><span data-stu-id="fa51a-131">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="fa51a-132">heading</span><span class="sxs-lookup"><span data-stu-id="fa51a-132">heading</span></span>|<span data-ttu-id="fa51a-133">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="fa51a-133">Double</span></span>|<span data-ttu-id="fa51a-134">Направление от географического севера (градусов)</span><span class="sxs-lookup"><span data-stu-id="fa51a-134">Heading in degrees from true north</span></span>|
|<span data-ttu-id="fa51a-135">speed</span><span class="sxs-lookup"><span data-stu-id="fa51a-135">speed</span></span>|<span data-ttu-id="fa51a-136">Double</span><span class="sxs-lookup"><span data-stu-id="fa51a-136">Double</span></span>|<span data-ttu-id="fa51a-137">Скорость передвижения устройства (м/с)</span><span class="sxs-lookup"><span data-stu-id="fa51a-137">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa51a-138">Связи</span><span class="sxs-lookup"><span data-stu-id="fa51a-138">Relationships</span></span>
<span data-ttu-id="fa51a-139">Нет</span><span class="sxs-lookup"><span data-stu-id="fa51a-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa51a-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fa51a-140">JSON Representation</span></span>
<span data-ttu-id="fa51a-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa51a-141">Here is a JSON representation of the resource.</span></span>
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



