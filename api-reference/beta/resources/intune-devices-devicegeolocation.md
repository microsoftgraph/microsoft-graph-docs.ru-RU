---
title: Тип ресурса deviceGeoLocation
description: Расположение устройства
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1da2a612a777491731fa0b85e2f754605ffa04bc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370167"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="2a4c8-103">Тип ресурса deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="2a4c8-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="2a4c8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a4c8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a4c8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2a4c8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a4c8-106">Расположение устройства</span><span class="sxs-lookup"><span data-stu-id="2a4c8-106">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="2a4c8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2a4c8-107">Properties</span></span>
|<span data-ttu-id="2a4c8-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a4c8-108">Property</span></span>|<span data-ttu-id="2a4c8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2a4c8-109">Type</span></span>|<span data-ttu-id="2a4c8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2a4c8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a4c8-111">ластколлектеддатетимеутк</span><span class="sxs-lookup"><span data-stu-id="2a4c8-111">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="2a4c8-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a4c8-112">DateTimeOffset</span></span>|<span data-ttu-id="2a4c8-113">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="2a4c8-113">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="2a4c8-114">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="2a4c8-114">lastCollectedDateTime</span></span>|<span data-ttu-id="2a4c8-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a4c8-115">DateTimeOffset</span></span>|<span data-ttu-id="2a4c8-116">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="2a4c8-116">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="2a4c8-117">longitude</span><span class="sxs-lookup"><span data-stu-id="2a4c8-117">longitude</span></span>|<span data-ttu-id="2a4c8-118">Двойное</span><span class="sxs-lookup"><span data-stu-id="2a4c8-118">Double</span></span>|<span data-ttu-id="2a4c8-119">Долгота расположения устройства</span><span class="sxs-lookup"><span data-stu-id="2a4c8-119">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="2a4c8-120">latitude</span><span class="sxs-lookup"><span data-stu-id="2a4c8-120">latitude</span></span>|<span data-ttu-id="2a4c8-121">Двойное</span><span class="sxs-lookup"><span data-stu-id="2a4c8-121">Double</span></span>|<span data-ttu-id="2a4c8-122">Широта расположения устройства</span><span class="sxs-lookup"><span data-stu-id="2a4c8-122">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="2a4c8-123">altitude</span><span class="sxs-lookup"><span data-stu-id="2a4c8-123">altitude</span></span>|<span data-ttu-id="2a4c8-124">Двойное</span><span class="sxs-lookup"><span data-stu-id="2a4c8-124">Double</span></span>|<span data-ttu-id="2a4c8-125">Высота (метров над уровнем моря)</span><span class="sxs-lookup"><span data-stu-id="2a4c8-125">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="2a4c8-126">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="2a4c8-126">horizontalAccuracy</span></span>|<span data-ttu-id="2a4c8-127">Двойное</span><span class="sxs-lookup"><span data-stu-id="2a4c8-127">Double</span></span>|<span data-ttu-id="2a4c8-128">Точность долготы и широты (м)</span><span class="sxs-lookup"><span data-stu-id="2a4c8-128">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="2a4c8-129">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="2a4c8-129">verticalAccuracy</span></span>|<span data-ttu-id="2a4c8-130">Двойное</span><span class="sxs-lookup"><span data-stu-id="2a4c8-130">Double</span></span>|<span data-ttu-id="2a4c8-131">Точность высоты (м)</span><span class="sxs-lookup"><span data-stu-id="2a4c8-131">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="2a4c8-132">heading</span><span class="sxs-lookup"><span data-stu-id="2a4c8-132">heading</span></span>|<span data-ttu-id="2a4c8-133">Двойное</span><span class="sxs-lookup"><span data-stu-id="2a4c8-133">Double</span></span>|<span data-ttu-id="2a4c8-134">Направление от географического севера (градусов)</span><span class="sxs-lookup"><span data-stu-id="2a4c8-134">Heading in degrees from true north</span></span>|
|<span data-ttu-id="2a4c8-135">speed</span><span class="sxs-lookup"><span data-stu-id="2a4c8-135">speed</span></span>|<span data-ttu-id="2a4c8-136">Double</span><span class="sxs-lookup"><span data-stu-id="2a4c8-136">Double</span></span>|<span data-ttu-id="2a4c8-137">Скорость передвижения устройства (м/с)</span><span class="sxs-lookup"><span data-stu-id="2a4c8-137">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a4c8-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="2a4c8-138">Relationships</span></span>
<span data-ttu-id="2a4c8-139">Нет</span><span class="sxs-lookup"><span data-stu-id="2a4c8-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2a4c8-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2a4c8-140">JSON Representation</span></span>
<span data-ttu-id="2a4c8-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a4c8-141">Here is a JSON representation of the resource.</span></span>
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



