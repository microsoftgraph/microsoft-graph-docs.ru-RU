---
title: Тип ресурса deviceGeoLocation
description: Расположение устройства
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 248af3f66a78e3197a3f966225e864f5583f8597
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940955"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="c94dd-103">Тип ресурса deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="c94dd-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="c94dd-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c94dd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c94dd-105">Расположение устройства</span><span class="sxs-lookup"><span data-stu-id="c94dd-105">Device location</span></span>
## <a name="properties"></a><span data-ttu-id="c94dd-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c94dd-106">Properties</span></span>
|<span data-ttu-id="c94dd-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c94dd-107">Property</span></span>|<span data-ttu-id="c94dd-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c94dd-108">Type</span></span>|<span data-ttu-id="c94dd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c94dd-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c94dd-110">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="c94dd-110">lastCollectedDateTime</span></span>|<span data-ttu-id="c94dd-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c94dd-111">DateTimeOffset</span></span>|<span data-ttu-id="c94dd-112">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="c94dd-112">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="c94dd-113">longitude</span><span class="sxs-lookup"><span data-stu-id="c94dd-113">longitude</span></span>|<span data-ttu-id="c94dd-114">Double</span><span class="sxs-lookup"><span data-stu-id="c94dd-114">Double</span></span>|<span data-ttu-id="c94dd-115">Долгота расположения устройства</span><span class="sxs-lookup"><span data-stu-id="c94dd-115">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="c94dd-116">latitude</span><span class="sxs-lookup"><span data-stu-id="c94dd-116">latitude</span></span>|<span data-ttu-id="c94dd-117">Double</span><span class="sxs-lookup"><span data-stu-id="c94dd-117">Double</span></span>|<span data-ttu-id="c94dd-118">Широта расположения устройства</span><span class="sxs-lookup"><span data-stu-id="c94dd-118">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="c94dd-119">altitude</span><span class="sxs-lookup"><span data-stu-id="c94dd-119">altitude</span></span>|<span data-ttu-id="c94dd-120">Double</span><span class="sxs-lookup"><span data-stu-id="c94dd-120">Double</span></span>|<span data-ttu-id="c94dd-121">Высота (метров над уровнем моря)</span><span class="sxs-lookup"><span data-stu-id="c94dd-121">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="c94dd-122">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="c94dd-122">horizontalAccuracy</span></span>|<span data-ttu-id="c94dd-123">Double</span><span class="sxs-lookup"><span data-stu-id="c94dd-123">Double</span></span>|<span data-ttu-id="c94dd-124">Точность долготы и широты (м)</span><span class="sxs-lookup"><span data-stu-id="c94dd-124">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="c94dd-125">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="c94dd-125">verticalAccuracy</span></span>|<span data-ttu-id="c94dd-126">Double</span><span class="sxs-lookup"><span data-stu-id="c94dd-126">Double</span></span>|<span data-ttu-id="c94dd-127">Точность высоты (м)</span><span class="sxs-lookup"><span data-stu-id="c94dd-127">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="c94dd-128">heading</span><span class="sxs-lookup"><span data-stu-id="c94dd-128">heading</span></span>|<span data-ttu-id="c94dd-129">Double</span><span class="sxs-lookup"><span data-stu-id="c94dd-129">Double</span></span>|<span data-ttu-id="c94dd-130">Направление от географического севера (градусов)</span><span class="sxs-lookup"><span data-stu-id="c94dd-130">Heading in degrees from true north</span></span>|
|<span data-ttu-id="c94dd-131">speed</span><span class="sxs-lookup"><span data-stu-id="c94dd-131">speed</span></span>|<span data-ttu-id="c94dd-132">Double</span><span class="sxs-lookup"><span data-stu-id="c94dd-132">Double</span></span>|<span data-ttu-id="c94dd-133">Скорость передвижения устройства (м/с)</span><span class="sxs-lookup"><span data-stu-id="c94dd-133">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="c94dd-134">Связи</span><span class="sxs-lookup"><span data-stu-id="c94dd-134">Relationships</span></span>
<span data-ttu-id="c94dd-135">Нет</span><span class="sxs-lookup"><span data-stu-id="c94dd-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c94dd-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c94dd-136">JSON Representation</span></span>
<span data-ttu-id="c94dd-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c94dd-137">Here is a JSON representation of the resource.</span></span>
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



