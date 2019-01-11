---
title: Тип ресурса deviceGeoLocation
description: Расположение устройства
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: dd81a0665d3d85a10488f78245449d265c85a8cc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845264"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="53a4a-103">Тип ресурса deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="53a4a-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="53a4a-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="53a4a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="53a4a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53a4a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="53a4a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="53a4a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="53a4a-107">Расположение устройства</span><span class="sxs-lookup"><span data-stu-id="53a4a-107">Device location</span></span>
## <a name="properties"></a><span data-ttu-id="53a4a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="53a4a-108">Properties</span></span>
|<span data-ttu-id="53a4a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="53a4a-109">Property</span></span>|<span data-ttu-id="53a4a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="53a4a-110">Type</span></span>|<span data-ttu-id="53a4a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="53a4a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53a4a-112">lastCollectedDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="53a4a-112">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="53a4a-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53a4a-113">DateTimeOffset</span></span>|<span data-ttu-id="53a4a-114">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="53a4a-114">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="53a4a-115">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="53a4a-115">lastCollectedDateTime</span></span>|<span data-ttu-id="53a4a-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53a4a-116">DateTimeOffset</span></span>|<span data-ttu-id="53a4a-117">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="53a4a-117">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="53a4a-118">longitude</span><span class="sxs-lookup"><span data-stu-id="53a4a-118">longitude</span></span>|<span data-ttu-id="53a4a-119">Double</span><span class="sxs-lookup"><span data-stu-id="53a4a-119">Double</span></span>|<span data-ttu-id="53a4a-120">Долгота расположения устройства</span><span class="sxs-lookup"><span data-stu-id="53a4a-120">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="53a4a-121">latitude</span><span class="sxs-lookup"><span data-stu-id="53a4a-121">latitude</span></span>|<span data-ttu-id="53a4a-122">Double</span><span class="sxs-lookup"><span data-stu-id="53a4a-122">Double</span></span>|<span data-ttu-id="53a4a-123">Широта расположения устройства</span><span class="sxs-lookup"><span data-stu-id="53a4a-123">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="53a4a-124">altitude</span><span class="sxs-lookup"><span data-stu-id="53a4a-124">altitude</span></span>|<span data-ttu-id="53a4a-125">Double</span><span class="sxs-lookup"><span data-stu-id="53a4a-125">Double</span></span>|<span data-ttu-id="53a4a-126">Высота (метров над уровнем моря)</span><span class="sxs-lookup"><span data-stu-id="53a4a-126">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="53a4a-127">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="53a4a-127">horizontalAccuracy</span></span>|<span data-ttu-id="53a4a-128">Double</span><span class="sxs-lookup"><span data-stu-id="53a4a-128">Double</span></span>|<span data-ttu-id="53a4a-129">Точность долготы и широты (м)</span><span class="sxs-lookup"><span data-stu-id="53a4a-129">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="53a4a-130">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="53a4a-130">verticalAccuracy</span></span>|<span data-ttu-id="53a4a-131">Double</span><span class="sxs-lookup"><span data-stu-id="53a4a-131">Double</span></span>|<span data-ttu-id="53a4a-132">Точность высоты (м)</span><span class="sxs-lookup"><span data-stu-id="53a4a-132">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="53a4a-133">heading</span><span class="sxs-lookup"><span data-stu-id="53a4a-133">heading</span></span>|<span data-ttu-id="53a4a-134">Double</span><span class="sxs-lookup"><span data-stu-id="53a4a-134">Double</span></span>|<span data-ttu-id="53a4a-135">Направление от географического севера (градусов)</span><span class="sxs-lookup"><span data-stu-id="53a4a-135">Heading in degrees from true north</span></span>|
|<span data-ttu-id="53a4a-136">speed</span><span class="sxs-lookup"><span data-stu-id="53a4a-136">speed</span></span>|<span data-ttu-id="53a4a-137">Double</span><span class="sxs-lookup"><span data-stu-id="53a4a-137">Double</span></span>|<span data-ttu-id="53a4a-138">Скорость передвижения устройства (м/с)</span><span class="sxs-lookup"><span data-stu-id="53a4a-138">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="53a4a-139">Связи</span><span class="sxs-lookup"><span data-stu-id="53a4a-139">Relationships</span></span>
<span data-ttu-id="53a4a-140">Нет</span><span class="sxs-lookup"><span data-stu-id="53a4a-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="53a4a-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="53a4a-141">JSON Representation</span></span>
<span data-ttu-id="53a4a-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53a4a-142">Here is a JSON representation of the resource.</span></span>
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





