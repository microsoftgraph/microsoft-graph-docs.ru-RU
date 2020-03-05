---
title: Тип ресурса deviceGeoLocation
description: Расположение устройства
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7417f5020fd7496a2daecde3ffbeb6e7391eaf08
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528645"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="64f90-103">Тип ресурса deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="64f90-103">deviceGeoLocation resource type</span></span>

<span data-ttu-id="64f90-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="64f90-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64f90-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64f90-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64f90-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64f90-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64f90-107">Расположение устройства</span><span class="sxs-lookup"><span data-stu-id="64f90-107">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="64f90-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="64f90-108">Properties</span></span>
|<span data-ttu-id="64f90-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="64f90-109">Property</span></span>|<span data-ttu-id="64f90-110">Тип</span><span class="sxs-lookup"><span data-stu-id="64f90-110">Type</span></span>|<span data-ttu-id="64f90-111">Описание</span><span class="sxs-lookup"><span data-stu-id="64f90-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64f90-112">ластколлектеддатетимеутк</span><span class="sxs-lookup"><span data-stu-id="64f90-112">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="64f90-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64f90-113">DateTimeOffset</span></span>|<span data-ttu-id="64f90-114">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="64f90-114">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="64f90-115">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="64f90-115">lastCollectedDateTime</span></span>|<span data-ttu-id="64f90-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64f90-116">DateTimeOffset</span></span>|<span data-ttu-id="64f90-117">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="64f90-117">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="64f90-118">longitude</span><span class="sxs-lookup"><span data-stu-id="64f90-118">longitude</span></span>|<span data-ttu-id="64f90-119">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="64f90-119">Double</span></span>|<span data-ttu-id="64f90-120">Долгота расположения устройства</span><span class="sxs-lookup"><span data-stu-id="64f90-120">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="64f90-121">latitude</span><span class="sxs-lookup"><span data-stu-id="64f90-121">latitude</span></span>|<span data-ttu-id="64f90-122">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="64f90-122">Double</span></span>|<span data-ttu-id="64f90-123">Широта расположения устройства</span><span class="sxs-lookup"><span data-stu-id="64f90-123">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="64f90-124">altitude</span><span class="sxs-lookup"><span data-stu-id="64f90-124">altitude</span></span>|<span data-ttu-id="64f90-125">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="64f90-125">Double</span></span>|<span data-ttu-id="64f90-126">Высота (метров над уровнем моря)</span><span class="sxs-lookup"><span data-stu-id="64f90-126">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="64f90-127">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="64f90-127">horizontalAccuracy</span></span>|<span data-ttu-id="64f90-128">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="64f90-128">Double</span></span>|<span data-ttu-id="64f90-129">Точность долготы и широты (м)</span><span class="sxs-lookup"><span data-stu-id="64f90-129">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="64f90-130">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="64f90-130">verticalAccuracy</span></span>|<span data-ttu-id="64f90-131">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="64f90-131">Double</span></span>|<span data-ttu-id="64f90-132">Точность высоты (м)</span><span class="sxs-lookup"><span data-stu-id="64f90-132">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="64f90-133">heading</span><span class="sxs-lookup"><span data-stu-id="64f90-133">heading</span></span>|<span data-ttu-id="64f90-134">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="64f90-134">Double</span></span>|<span data-ttu-id="64f90-135">Направление от географического севера (градусов)</span><span class="sxs-lookup"><span data-stu-id="64f90-135">Heading in degrees from true north</span></span>|
|<span data-ttu-id="64f90-136">speed</span><span class="sxs-lookup"><span data-stu-id="64f90-136">speed</span></span>|<span data-ttu-id="64f90-137">Double</span><span class="sxs-lookup"><span data-stu-id="64f90-137">Double</span></span>|<span data-ttu-id="64f90-138">Скорость передвижения устройства (м/с)</span><span class="sxs-lookup"><span data-stu-id="64f90-138">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="64f90-139">Связи</span><span class="sxs-lookup"><span data-stu-id="64f90-139">Relationships</span></span>
<span data-ttu-id="64f90-140">Нет</span><span class="sxs-lookup"><span data-stu-id="64f90-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="64f90-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="64f90-141">JSON Representation</span></span>
<span data-ttu-id="64f90-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64f90-142">Here is a JSON representation of the resource.</span></span>
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



