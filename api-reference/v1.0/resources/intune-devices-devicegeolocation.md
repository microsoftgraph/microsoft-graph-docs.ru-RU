---
title: Тип ресурса deviceGeoLocation
description: Расположение устройства
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: eb11f4c8d4d2ce87d28d92f13e359ce213c3ca9c
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356984"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="f449a-103">Тип ресурса deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="f449a-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="f449a-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f449a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f449a-105">Расположение устройства</span><span class="sxs-lookup"><span data-stu-id="f449a-105">Device location</span></span>

## <a name="properties"></a><span data-ttu-id="f449a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f449a-106">Properties</span></span>
|<span data-ttu-id="f449a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f449a-107">Property</span></span>|<span data-ttu-id="f449a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f449a-108">Type</span></span>|<span data-ttu-id="f449a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f449a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f449a-110">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="f449a-110">lastCollectedDateTime</span></span>|<span data-ttu-id="f449a-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f449a-111">DateTimeOffset</span></span>|<span data-ttu-id="f449a-112">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="f449a-112">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="f449a-113">longitude</span><span class="sxs-lookup"><span data-stu-id="f449a-113">longitude</span></span>|<span data-ttu-id="f449a-114">Двойное</span><span class="sxs-lookup"><span data-stu-id="f449a-114">Double</span></span>|<span data-ttu-id="f449a-115">Долгота расположения устройства</span><span class="sxs-lookup"><span data-stu-id="f449a-115">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="f449a-116">latitude</span><span class="sxs-lookup"><span data-stu-id="f449a-116">latitude</span></span>|<span data-ttu-id="f449a-117">Двойное</span><span class="sxs-lookup"><span data-stu-id="f449a-117">Double</span></span>|<span data-ttu-id="f449a-118">Широта расположения устройства</span><span class="sxs-lookup"><span data-stu-id="f449a-118">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="f449a-119">altitude</span><span class="sxs-lookup"><span data-stu-id="f449a-119">altitude</span></span>|<span data-ttu-id="f449a-120">Двойное</span><span class="sxs-lookup"><span data-stu-id="f449a-120">Double</span></span>|<span data-ttu-id="f449a-121">Высота (метров над уровнем моря)</span><span class="sxs-lookup"><span data-stu-id="f449a-121">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="f449a-122">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="f449a-122">horizontalAccuracy</span></span>|<span data-ttu-id="f449a-123">Двойное</span><span class="sxs-lookup"><span data-stu-id="f449a-123">Double</span></span>|<span data-ttu-id="f449a-124">Точность долготы и широты (м)</span><span class="sxs-lookup"><span data-stu-id="f449a-124">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="f449a-125">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="f449a-125">verticalAccuracy</span></span>|<span data-ttu-id="f449a-126">Двойное</span><span class="sxs-lookup"><span data-stu-id="f449a-126">Double</span></span>|<span data-ttu-id="f449a-127">Точность высоты (м)</span><span class="sxs-lookup"><span data-stu-id="f449a-127">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="f449a-128">heading</span><span class="sxs-lookup"><span data-stu-id="f449a-128">heading</span></span>|<span data-ttu-id="f449a-129">Двойное</span><span class="sxs-lookup"><span data-stu-id="f449a-129">Double</span></span>|<span data-ttu-id="f449a-130">Направление от географического севера (градусов)</span><span class="sxs-lookup"><span data-stu-id="f449a-130">Heading in degrees from true north</span></span>|
|<span data-ttu-id="f449a-131">speed</span><span class="sxs-lookup"><span data-stu-id="f449a-131">speed</span></span>|<span data-ttu-id="f449a-132">Double</span><span class="sxs-lookup"><span data-stu-id="f449a-132">Double</span></span>|<span data-ttu-id="f449a-133">Скорость передвижения устройства (м/с)</span><span class="sxs-lookup"><span data-stu-id="f449a-133">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="f449a-134">Связи</span><span class="sxs-lookup"><span data-stu-id="f449a-134">Relationships</span></span>
<span data-ttu-id="f449a-135">Нет</span><span class="sxs-lookup"><span data-stu-id="f449a-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f449a-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f449a-136">JSON Representation</span></span>
<span data-ttu-id="f449a-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f449a-137">Here is a JSON representation of the resource.</span></span>
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




