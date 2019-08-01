---
title: Тип ресурса deviceGeoLocation
description: Расположение устройства
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 88802f3d4909f07ab96395efdf61ad7e817f4be8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030816"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="b599a-103">Тип ресурса deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="b599a-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="b599a-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b599a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b599a-105">Расположение устройства</span><span class="sxs-lookup"><span data-stu-id="b599a-105">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="b599a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b599a-106">Properties</span></span>
|<span data-ttu-id="b599a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b599a-107">Property</span></span>|<span data-ttu-id="b599a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b599a-108">Type</span></span>|<span data-ttu-id="b599a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b599a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b599a-110">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="b599a-110">lastCollectedDateTime</span></span>|<span data-ttu-id="b599a-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b599a-111">DateTimeOffset</span></span>|<span data-ttu-id="b599a-112">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="b599a-112">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="b599a-113">longitude</span><span class="sxs-lookup"><span data-stu-id="b599a-113">longitude</span></span>|<span data-ttu-id="b599a-114">Двойное</span><span class="sxs-lookup"><span data-stu-id="b599a-114">Double</span></span>|<span data-ttu-id="b599a-115">Долгота расположения устройства</span><span class="sxs-lookup"><span data-stu-id="b599a-115">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="b599a-116">latitude</span><span class="sxs-lookup"><span data-stu-id="b599a-116">latitude</span></span>|<span data-ttu-id="b599a-117">Двойное</span><span class="sxs-lookup"><span data-stu-id="b599a-117">Double</span></span>|<span data-ttu-id="b599a-118">Широта расположения устройства</span><span class="sxs-lookup"><span data-stu-id="b599a-118">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="b599a-119">altitude</span><span class="sxs-lookup"><span data-stu-id="b599a-119">altitude</span></span>|<span data-ttu-id="b599a-120">Двойное</span><span class="sxs-lookup"><span data-stu-id="b599a-120">Double</span></span>|<span data-ttu-id="b599a-121">Высота (метров над уровнем моря)</span><span class="sxs-lookup"><span data-stu-id="b599a-121">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="b599a-122">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="b599a-122">horizontalAccuracy</span></span>|<span data-ttu-id="b599a-123">Двойное</span><span class="sxs-lookup"><span data-stu-id="b599a-123">Double</span></span>|<span data-ttu-id="b599a-124">Точность долготы и широты (м)</span><span class="sxs-lookup"><span data-stu-id="b599a-124">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="b599a-125">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="b599a-125">verticalAccuracy</span></span>|<span data-ttu-id="b599a-126">Двойное</span><span class="sxs-lookup"><span data-stu-id="b599a-126">Double</span></span>|<span data-ttu-id="b599a-127">Точность высоты (м)</span><span class="sxs-lookup"><span data-stu-id="b599a-127">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="b599a-128">heading</span><span class="sxs-lookup"><span data-stu-id="b599a-128">heading</span></span>|<span data-ttu-id="b599a-129">Двойное</span><span class="sxs-lookup"><span data-stu-id="b599a-129">Double</span></span>|<span data-ttu-id="b599a-130">Направление от географического севера (градусов)</span><span class="sxs-lookup"><span data-stu-id="b599a-130">Heading in degrees from true north</span></span>|
|<span data-ttu-id="b599a-131">speed</span><span class="sxs-lookup"><span data-stu-id="b599a-131">speed</span></span>|<span data-ttu-id="b599a-132">Double</span><span class="sxs-lookup"><span data-stu-id="b599a-132">Double</span></span>|<span data-ttu-id="b599a-133">Скорость передвижения устройства (м/с)</span><span class="sxs-lookup"><span data-stu-id="b599a-133">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="b599a-134">Отношения</span><span class="sxs-lookup"><span data-stu-id="b599a-134">Relationships</span></span>
<span data-ttu-id="b599a-135">Нет</span><span class="sxs-lookup"><span data-stu-id="b599a-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b599a-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b599a-136">JSON Representation</span></span>
<span data-ttu-id="b599a-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b599a-137">Here is a JSON representation of the resource.</span></span>
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



