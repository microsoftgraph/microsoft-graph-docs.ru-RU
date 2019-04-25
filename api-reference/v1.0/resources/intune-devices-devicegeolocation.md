---
title: Тип ресурса deviceGeoLocation
description: Расположение устройства
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b51768aea1338486431ceffadd95f8760a7216ab
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542034"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="62f99-103">Тип ресурса deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="62f99-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="62f99-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="62f99-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62f99-105">Расположение устройства</span><span class="sxs-lookup"><span data-stu-id="62f99-105">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="62f99-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="62f99-106">Properties</span></span>
|<span data-ttu-id="62f99-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="62f99-107">Property</span></span>|<span data-ttu-id="62f99-108">Тип</span><span class="sxs-lookup"><span data-stu-id="62f99-108">Type</span></span>|<span data-ttu-id="62f99-109">Описание</span><span class="sxs-lookup"><span data-stu-id="62f99-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62f99-110">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="62f99-110">lastCollectedDateTime</span></span>|<span data-ttu-id="62f99-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62f99-111">DateTimeOffset</span></span>|<span data-ttu-id="62f99-112">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="62f99-112">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="62f99-113">longitude</span><span class="sxs-lookup"><span data-stu-id="62f99-113">longitude</span></span>|<span data-ttu-id="62f99-114">Двойное</span><span class="sxs-lookup"><span data-stu-id="62f99-114">Double</span></span>|<span data-ttu-id="62f99-115">Долгота расположения устройства</span><span class="sxs-lookup"><span data-stu-id="62f99-115">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="62f99-116">latitude</span><span class="sxs-lookup"><span data-stu-id="62f99-116">latitude</span></span>|<span data-ttu-id="62f99-117">Двойное</span><span class="sxs-lookup"><span data-stu-id="62f99-117">Double</span></span>|<span data-ttu-id="62f99-118">Широта расположения устройства</span><span class="sxs-lookup"><span data-stu-id="62f99-118">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="62f99-119">altitude</span><span class="sxs-lookup"><span data-stu-id="62f99-119">altitude</span></span>|<span data-ttu-id="62f99-120">Двойное</span><span class="sxs-lookup"><span data-stu-id="62f99-120">Double</span></span>|<span data-ttu-id="62f99-121">Высота (метров над уровнем моря)</span><span class="sxs-lookup"><span data-stu-id="62f99-121">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="62f99-122">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="62f99-122">horizontalAccuracy</span></span>|<span data-ttu-id="62f99-123">Двойное</span><span class="sxs-lookup"><span data-stu-id="62f99-123">Double</span></span>|<span data-ttu-id="62f99-124">Точность долготы и широты (м)</span><span class="sxs-lookup"><span data-stu-id="62f99-124">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="62f99-125">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="62f99-125">verticalAccuracy</span></span>|<span data-ttu-id="62f99-126">Двойное</span><span class="sxs-lookup"><span data-stu-id="62f99-126">Double</span></span>|<span data-ttu-id="62f99-127">Точность высоты (м)</span><span class="sxs-lookup"><span data-stu-id="62f99-127">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="62f99-128">heading</span><span class="sxs-lookup"><span data-stu-id="62f99-128">heading</span></span>|<span data-ttu-id="62f99-129">Двойное</span><span class="sxs-lookup"><span data-stu-id="62f99-129">Double</span></span>|<span data-ttu-id="62f99-130">Направление от географического севера (градусов)</span><span class="sxs-lookup"><span data-stu-id="62f99-130">Heading in degrees from true north</span></span>|
|<span data-ttu-id="62f99-131">speed</span><span class="sxs-lookup"><span data-stu-id="62f99-131">speed</span></span>|<span data-ttu-id="62f99-132">Double</span><span class="sxs-lookup"><span data-stu-id="62f99-132">Double</span></span>|<span data-ttu-id="62f99-133">Скорость передвижения устройства (м/с)</span><span class="sxs-lookup"><span data-stu-id="62f99-133">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="62f99-134">Отношения</span><span class="sxs-lookup"><span data-stu-id="62f99-134">Relationships</span></span>
<span data-ttu-id="62f99-135">Нет</span><span class="sxs-lookup"><span data-stu-id="62f99-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="62f99-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="62f99-136">JSON Representation</span></span>
<span data-ttu-id="62f99-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62f99-137">Here is a JSON representation of the resource.</span></span>
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



