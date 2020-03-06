---
title: Тип ресурса deviceGeoLocation
description: Расположение устройства
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 48c0b4224225c70a9f5c4a636e1e15e4ddea3364
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533298"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="a8ff8-103">Тип ресурса deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="a8ff8-103">deviceGeoLocation resource type</span></span>

<span data-ttu-id="a8ff8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8ff8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a8ff8-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a8ff8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8ff8-106">Расположение устройства</span><span class="sxs-lookup"><span data-stu-id="a8ff8-106">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="a8ff8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a8ff8-107">Properties</span></span>
|<span data-ttu-id="a8ff8-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8ff8-108">Property</span></span>|<span data-ttu-id="a8ff8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a8ff8-109">Type</span></span>|<span data-ttu-id="a8ff8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a8ff8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8ff8-111">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8ff8-111">lastCollectedDateTime</span></span>|<span data-ttu-id="a8ff8-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8ff8-112">DateTimeOffset</span></span>|<span data-ttu-id="a8ff8-113">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="a8ff8-113">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="a8ff8-114">longitude</span><span class="sxs-lookup"><span data-stu-id="a8ff8-114">longitude</span></span>|<span data-ttu-id="a8ff8-115">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="a8ff8-115">Double</span></span>|<span data-ttu-id="a8ff8-116">Долгота расположения устройства</span><span class="sxs-lookup"><span data-stu-id="a8ff8-116">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="a8ff8-117">latitude</span><span class="sxs-lookup"><span data-stu-id="a8ff8-117">latitude</span></span>|<span data-ttu-id="a8ff8-118">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="a8ff8-118">Double</span></span>|<span data-ttu-id="a8ff8-119">Широта расположения устройства</span><span class="sxs-lookup"><span data-stu-id="a8ff8-119">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="a8ff8-120">altitude</span><span class="sxs-lookup"><span data-stu-id="a8ff8-120">altitude</span></span>|<span data-ttu-id="a8ff8-121">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="a8ff8-121">Double</span></span>|<span data-ttu-id="a8ff8-122">Высота (метров над уровнем моря)</span><span class="sxs-lookup"><span data-stu-id="a8ff8-122">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="a8ff8-123">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="a8ff8-123">horizontalAccuracy</span></span>|<span data-ttu-id="a8ff8-124">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="a8ff8-124">Double</span></span>|<span data-ttu-id="a8ff8-125">Точность долготы и широты (м)</span><span class="sxs-lookup"><span data-stu-id="a8ff8-125">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="a8ff8-126">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="a8ff8-126">verticalAccuracy</span></span>|<span data-ttu-id="a8ff8-127">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="a8ff8-127">Double</span></span>|<span data-ttu-id="a8ff8-128">Точность высоты (м)</span><span class="sxs-lookup"><span data-stu-id="a8ff8-128">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="a8ff8-129">heading</span><span class="sxs-lookup"><span data-stu-id="a8ff8-129">heading</span></span>|<span data-ttu-id="a8ff8-130">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="a8ff8-130">Double</span></span>|<span data-ttu-id="a8ff8-131">Направление от географического севера (градусов)</span><span class="sxs-lookup"><span data-stu-id="a8ff8-131">Heading in degrees from true north</span></span>|
|<span data-ttu-id="a8ff8-132">speed</span><span class="sxs-lookup"><span data-stu-id="a8ff8-132">speed</span></span>|<span data-ttu-id="a8ff8-133">Double</span><span class="sxs-lookup"><span data-stu-id="a8ff8-133">Double</span></span>|<span data-ttu-id="a8ff8-134">Скорость передвижения устройства (м/с)</span><span class="sxs-lookup"><span data-stu-id="a8ff8-134">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8ff8-135">Связи</span><span class="sxs-lookup"><span data-stu-id="a8ff8-135">Relationships</span></span>
<span data-ttu-id="a8ff8-136">Нет</span><span class="sxs-lookup"><span data-stu-id="a8ff8-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8ff8-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a8ff8-137">JSON Representation</span></span>
<span data-ttu-id="a8ff8-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8ff8-138">Here is a JSON representation of the resource.</span></span>
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




