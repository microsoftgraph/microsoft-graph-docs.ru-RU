---
title: Тип ресурса deviceGeoLocation
description: Расположение устройства
author: tfitzmac
ms.openlocfilehash: fe8ffe7684132c9871225747a28905da1983672d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336997"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="d13cf-103">Тип ресурса deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="d13cf-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="d13cf-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d13cf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d13cf-105">Расположение устройства</span><span class="sxs-lookup"><span data-stu-id="d13cf-105">Device location</span></span>
## <a name="properties"></a><span data-ttu-id="d13cf-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d13cf-106">Properties</span></span>
|<span data-ttu-id="d13cf-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d13cf-107">Property</span></span>|<span data-ttu-id="d13cf-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d13cf-108">Type</span></span>|<span data-ttu-id="d13cf-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d13cf-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d13cf-110">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="d13cf-110">lastCollectedDateTime</span></span>|<span data-ttu-id="d13cf-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d13cf-111">DateTimeOffset</span></span>|<span data-ttu-id="d13cf-112">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="d13cf-112">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="d13cf-113">longitude</span><span class="sxs-lookup"><span data-stu-id="d13cf-113">longitude</span></span>|<span data-ttu-id="d13cf-114">Double</span><span class="sxs-lookup"><span data-stu-id="d13cf-114">Double</span></span>|<span data-ttu-id="d13cf-115">Долгота расположения устройства</span><span class="sxs-lookup"><span data-stu-id="d13cf-115">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="d13cf-116">latitude</span><span class="sxs-lookup"><span data-stu-id="d13cf-116">latitude</span></span>|<span data-ttu-id="d13cf-117">Double</span><span class="sxs-lookup"><span data-stu-id="d13cf-117">Double</span></span>|<span data-ttu-id="d13cf-118">Широта расположения устройства</span><span class="sxs-lookup"><span data-stu-id="d13cf-118">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="d13cf-119">altitude</span><span class="sxs-lookup"><span data-stu-id="d13cf-119">altitude</span></span>|<span data-ttu-id="d13cf-120">Double</span><span class="sxs-lookup"><span data-stu-id="d13cf-120">Double</span></span>|<span data-ttu-id="d13cf-121">Высота (метров над уровнем моря)</span><span class="sxs-lookup"><span data-stu-id="d13cf-121">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="d13cf-122">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="d13cf-122">horizontalAccuracy</span></span>|<span data-ttu-id="d13cf-123">Double</span><span class="sxs-lookup"><span data-stu-id="d13cf-123">Double</span></span>|<span data-ttu-id="d13cf-124">Точность долготы и широты (м)</span><span class="sxs-lookup"><span data-stu-id="d13cf-124">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="d13cf-125">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="d13cf-125">verticalAccuracy</span></span>|<span data-ttu-id="d13cf-126">Double</span><span class="sxs-lookup"><span data-stu-id="d13cf-126">Double</span></span>|<span data-ttu-id="d13cf-127">Точность высоты (м)</span><span class="sxs-lookup"><span data-stu-id="d13cf-127">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="d13cf-128">heading</span><span class="sxs-lookup"><span data-stu-id="d13cf-128">heading</span></span>|<span data-ttu-id="d13cf-129">Double</span><span class="sxs-lookup"><span data-stu-id="d13cf-129">Double</span></span>|<span data-ttu-id="d13cf-130">Направление от географического севера (градусов)</span><span class="sxs-lookup"><span data-stu-id="d13cf-130">Heading in degrees from true north</span></span>|
|<span data-ttu-id="d13cf-131">speed</span><span class="sxs-lookup"><span data-stu-id="d13cf-131">speed</span></span>|<span data-ttu-id="d13cf-132">Double</span><span class="sxs-lookup"><span data-stu-id="d13cf-132">Double</span></span>|<span data-ttu-id="d13cf-133">Скорость передвижения устройства (м/с)</span><span class="sxs-lookup"><span data-stu-id="d13cf-133">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="d13cf-134">Связи</span><span class="sxs-lookup"><span data-stu-id="d13cf-134">Relationships</span></span>
<span data-ttu-id="d13cf-135">Нет</span><span class="sxs-lookup"><span data-stu-id="d13cf-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d13cf-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d13cf-136">JSON Representation</span></span>
<span data-ttu-id="d13cf-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d13cf-137">Here is a JSON representation of the resource.</span></span>
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



