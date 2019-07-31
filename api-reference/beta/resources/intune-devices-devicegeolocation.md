---
title: Тип ресурса deviceGeoLocation
description: Расположение устройства
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 70d2f943adee1710c56900191111b3c724bf5e8b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968493"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="ac23c-103">Тип ресурса deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="ac23c-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="ac23c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac23c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ac23c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ac23c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac23c-106">Расположение устройства</span><span class="sxs-lookup"><span data-stu-id="ac23c-106">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="ac23c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ac23c-107">Properties</span></span>
|<span data-ttu-id="ac23c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac23c-108">Property</span></span>|<span data-ttu-id="ac23c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ac23c-109">Type</span></span>|<span data-ttu-id="ac23c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ac23c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac23c-111">Ластколлектеддатетимеутк</span><span class="sxs-lookup"><span data-stu-id="ac23c-111">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="ac23c-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac23c-112">DateTimeOffset</span></span>|<span data-ttu-id="ac23c-113">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="ac23c-113">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="ac23c-114">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="ac23c-114">lastCollectedDateTime</span></span>|<span data-ttu-id="ac23c-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac23c-115">DateTimeOffset</span></span>|<span data-ttu-id="ac23c-116">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="ac23c-116">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="ac23c-117">longitude</span><span class="sxs-lookup"><span data-stu-id="ac23c-117">longitude</span></span>|<span data-ttu-id="ac23c-118">Двойное</span><span class="sxs-lookup"><span data-stu-id="ac23c-118">Double</span></span>|<span data-ttu-id="ac23c-119">Долгота расположения устройства</span><span class="sxs-lookup"><span data-stu-id="ac23c-119">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="ac23c-120">latitude</span><span class="sxs-lookup"><span data-stu-id="ac23c-120">latitude</span></span>|<span data-ttu-id="ac23c-121">Двойное</span><span class="sxs-lookup"><span data-stu-id="ac23c-121">Double</span></span>|<span data-ttu-id="ac23c-122">Широта расположения устройства</span><span class="sxs-lookup"><span data-stu-id="ac23c-122">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="ac23c-123">altitude</span><span class="sxs-lookup"><span data-stu-id="ac23c-123">altitude</span></span>|<span data-ttu-id="ac23c-124">Двойное</span><span class="sxs-lookup"><span data-stu-id="ac23c-124">Double</span></span>|<span data-ttu-id="ac23c-125">Высота (метров над уровнем моря)</span><span class="sxs-lookup"><span data-stu-id="ac23c-125">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="ac23c-126">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="ac23c-126">horizontalAccuracy</span></span>|<span data-ttu-id="ac23c-127">Двойное</span><span class="sxs-lookup"><span data-stu-id="ac23c-127">Double</span></span>|<span data-ttu-id="ac23c-128">Точность долготы и широты (м)</span><span class="sxs-lookup"><span data-stu-id="ac23c-128">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="ac23c-129">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="ac23c-129">verticalAccuracy</span></span>|<span data-ttu-id="ac23c-130">Двойное</span><span class="sxs-lookup"><span data-stu-id="ac23c-130">Double</span></span>|<span data-ttu-id="ac23c-131">Точность высоты (м)</span><span class="sxs-lookup"><span data-stu-id="ac23c-131">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="ac23c-132">heading</span><span class="sxs-lookup"><span data-stu-id="ac23c-132">heading</span></span>|<span data-ttu-id="ac23c-133">Двойное</span><span class="sxs-lookup"><span data-stu-id="ac23c-133">Double</span></span>|<span data-ttu-id="ac23c-134">Направление от географического севера (градусов)</span><span class="sxs-lookup"><span data-stu-id="ac23c-134">Heading in degrees from true north</span></span>|
|<span data-ttu-id="ac23c-135">speed</span><span class="sxs-lookup"><span data-stu-id="ac23c-135">speed</span></span>|<span data-ttu-id="ac23c-136">Double</span><span class="sxs-lookup"><span data-stu-id="ac23c-136">Double</span></span>|<span data-ttu-id="ac23c-137">Скорость передвижения устройства (м/с)</span><span class="sxs-lookup"><span data-stu-id="ac23c-137">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac23c-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="ac23c-138">Relationships</span></span>
<span data-ttu-id="ac23c-139">Нет</span><span class="sxs-lookup"><span data-stu-id="ac23c-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac23c-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ac23c-140">JSON Representation</span></span>
<span data-ttu-id="ac23c-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac23c-141">Here is a JSON representation of the resource.</span></span>
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





