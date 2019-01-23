---
title: Тип ресурса deviceGeoLocation
description: Расположение устройства
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3b2105711a9a8f84b705a5a01c658c87cbe48c75
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395057"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="d3e39-103">Тип ресурса deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="d3e39-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="d3e39-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d3e39-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d3e39-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3e39-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d3e39-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d3e39-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3e39-107">Расположение устройства</span><span class="sxs-lookup"><span data-stu-id="d3e39-107">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="d3e39-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d3e39-108">Properties</span></span>
|<span data-ttu-id="d3e39-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3e39-109">Property</span></span>|<span data-ttu-id="d3e39-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d3e39-110">Type</span></span>|<span data-ttu-id="d3e39-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d3e39-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3e39-112">lastCollectedDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="d3e39-112">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="d3e39-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3e39-113">DateTimeOffset</span></span>|<span data-ttu-id="d3e39-114">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="d3e39-114">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="d3e39-115">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3e39-115">lastCollectedDateTime</span></span>|<span data-ttu-id="d3e39-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3e39-116">DateTimeOffset</span></span>|<span data-ttu-id="d3e39-117">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="d3e39-117">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="d3e39-118">longitude</span><span class="sxs-lookup"><span data-stu-id="d3e39-118">longitude</span></span>|<span data-ttu-id="d3e39-119">Double</span><span class="sxs-lookup"><span data-stu-id="d3e39-119">Double</span></span>|<span data-ttu-id="d3e39-120">Долгота расположения устройства</span><span class="sxs-lookup"><span data-stu-id="d3e39-120">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="d3e39-121">latitude</span><span class="sxs-lookup"><span data-stu-id="d3e39-121">latitude</span></span>|<span data-ttu-id="d3e39-122">Double</span><span class="sxs-lookup"><span data-stu-id="d3e39-122">Double</span></span>|<span data-ttu-id="d3e39-123">Широта расположения устройства</span><span class="sxs-lookup"><span data-stu-id="d3e39-123">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="d3e39-124">altitude</span><span class="sxs-lookup"><span data-stu-id="d3e39-124">altitude</span></span>|<span data-ttu-id="d3e39-125">Double</span><span class="sxs-lookup"><span data-stu-id="d3e39-125">Double</span></span>|<span data-ttu-id="d3e39-126">Высота (метров над уровнем моря)</span><span class="sxs-lookup"><span data-stu-id="d3e39-126">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="d3e39-127">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="d3e39-127">horizontalAccuracy</span></span>|<span data-ttu-id="d3e39-128">Double</span><span class="sxs-lookup"><span data-stu-id="d3e39-128">Double</span></span>|<span data-ttu-id="d3e39-129">Точность долготы и широты (м)</span><span class="sxs-lookup"><span data-stu-id="d3e39-129">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="d3e39-130">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="d3e39-130">verticalAccuracy</span></span>|<span data-ttu-id="d3e39-131">Double</span><span class="sxs-lookup"><span data-stu-id="d3e39-131">Double</span></span>|<span data-ttu-id="d3e39-132">Точность высоты (м)</span><span class="sxs-lookup"><span data-stu-id="d3e39-132">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="d3e39-133">heading</span><span class="sxs-lookup"><span data-stu-id="d3e39-133">heading</span></span>|<span data-ttu-id="d3e39-134">Double</span><span class="sxs-lookup"><span data-stu-id="d3e39-134">Double</span></span>|<span data-ttu-id="d3e39-135">Направление от географического севера (градусов)</span><span class="sxs-lookup"><span data-stu-id="d3e39-135">Heading in degrees from true north</span></span>|
|<span data-ttu-id="d3e39-136">speed</span><span class="sxs-lookup"><span data-stu-id="d3e39-136">speed</span></span>|<span data-ttu-id="d3e39-137">Double</span><span class="sxs-lookup"><span data-stu-id="d3e39-137">Double</span></span>|<span data-ttu-id="d3e39-138">Скорость передвижения устройства (м/с)</span><span class="sxs-lookup"><span data-stu-id="d3e39-138">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3e39-139">Связи</span><span class="sxs-lookup"><span data-stu-id="d3e39-139">Relationships</span></span>
<span data-ttu-id="d3e39-140">Нет</span><span class="sxs-lookup"><span data-stu-id="d3e39-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3e39-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d3e39-141">JSON Representation</span></span>
<span data-ttu-id="d3e39-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3e39-142">Here is a JSON representation of the resource.</span></span>
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




