---
title: Тип ресурса deviceGeoLocation
description: Расположение устройства
ms.openlocfilehash: 1bc72e4fb2d01c55d5d16ff2a45a020c5eaf99e5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027371"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="2dbbb-103">Тип ресурса deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="2dbbb-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="2dbbb-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2dbbb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2dbbb-105">Расположение устройства</span><span class="sxs-lookup"><span data-stu-id="2dbbb-105">Device location</span></span>
## <a name="properties"></a><span data-ttu-id="2dbbb-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2dbbb-106">Properties</span></span>
|<span data-ttu-id="2dbbb-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="2dbbb-107">Property</span></span>|<span data-ttu-id="2dbbb-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2dbbb-108">Type</span></span>|<span data-ttu-id="2dbbb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2dbbb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2dbbb-110">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="2dbbb-110">lastCollectedDateTime</span></span>|<span data-ttu-id="2dbbb-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2dbbb-111">DateTimeOffset</span></span>|<span data-ttu-id="2dbbb-112">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="2dbbb-112">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="2dbbb-113">longitude</span><span class="sxs-lookup"><span data-stu-id="2dbbb-113">longitude</span></span>|<span data-ttu-id="2dbbb-114">Double</span><span class="sxs-lookup"><span data-stu-id="2dbbb-114">Double</span></span>|<span data-ttu-id="2dbbb-115">Долгота расположения устройства</span><span class="sxs-lookup"><span data-stu-id="2dbbb-115">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="2dbbb-116">latitude</span><span class="sxs-lookup"><span data-stu-id="2dbbb-116">latitude</span></span>|<span data-ttu-id="2dbbb-117">Double</span><span class="sxs-lookup"><span data-stu-id="2dbbb-117">Double</span></span>|<span data-ttu-id="2dbbb-118">Широта расположения устройства</span><span class="sxs-lookup"><span data-stu-id="2dbbb-118">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="2dbbb-119">altitude</span><span class="sxs-lookup"><span data-stu-id="2dbbb-119">altitude</span></span>|<span data-ttu-id="2dbbb-120">Double</span><span class="sxs-lookup"><span data-stu-id="2dbbb-120">Double</span></span>|<span data-ttu-id="2dbbb-121">Высота (метров над уровнем моря)</span><span class="sxs-lookup"><span data-stu-id="2dbbb-121">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="2dbbb-122">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="2dbbb-122">horizontalAccuracy</span></span>|<span data-ttu-id="2dbbb-123">Double</span><span class="sxs-lookup"><span data-stu-id="2dbbb-123">Double</span></span>|<span data-ttu-id="2dbbb-124">Точность долготы и широты (м)</span><span class="sxs-lookup"><span data-stu-id="2dbbb-124">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="2dbbb-125">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="2dbbb-125">verticalAccuracy</span></span>|<span data-ttu-id="2dbbb-126">Double</span><span class="sxs-lookup"><span data-stu-id="2dbbb-126">Double</span></span>|<span data-ttu-id="2dbbb-127">Точность высоты (м)</span><span class="sxs-lookup"><span data-stu-id="2dbbb-127">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="2dbbb-128">heading</span><span class="sxs-lookup"><span data-stu-id="2dbbb-128">heading</span></span>|<span data-ttu-id="2dbbb-129">Double</span><span class="sxs-lookup"><span data-stu-id="2dbbb-129">Double</span></span>|<span data-ttu-id="2dbbb-130">Направление от географического севера (градусов)</span><span class="sxs-lookup"><span data-stu-id="2dbbb-130">Heading in degrees from true north</span></span>|
|<span data-ttu-id="2dbbb-131">speed</span><span class="sxs-lookup"><span data-stu-id="2dbbb-131">speed</span></span>|<span data-ttu-id="2dbbb-132">Double</span><span class="sxs-lookup"><span data-stu-id="2dbbb-132">Double</span></span>|<span data-ttu-id="2dbbb-133">Скорость передвижения устройства (м/с)</span><span class="sxs-lookup"><span data-stu-id="2dbbb-133">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="2dbbb-134">Связи</span><span class="sxs-lookup"><span data-stu-id="2dbbb-134">Relationships</span></span>
<span data-ttu-id="2dbbb-135">Нет</span><span class="sxs-lookup"><span data-stu-id="2dbbb-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2dbbb-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2dbbb-136">JSON Representation</span></span>
<span data-ttu-id="2dbbb-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2dbbb-137">Here is a JSON representation of the resource.</span></span>
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



