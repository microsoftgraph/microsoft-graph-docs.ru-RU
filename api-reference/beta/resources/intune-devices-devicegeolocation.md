---
title: Тип ресурса deviceGeoLocation
description: Расположение устройства
ms.openlocfilehash: 2ab7f777d00b891ceb7aae127ac87868aec582cc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076392"
---
# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="446dc-103">Тип ресурса deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="446dc-103">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="446dc-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="446dc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="446dc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="446dc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="446dc-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="446dc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="446dc-107">Расположение устройства</span><span class="sxs-lookup"><span data-stu-id="446dc-107">Device location</span></span>
## <a name="properties"></a><span data-ttu-id="446dc-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="446dc-108">Properties</span></span>
|<span data-ttu-id="446dc-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="446dc-109">Property</span></span>|<span data-ttu-id="446dc-110">Тип</span><span class="sxs-lookup"><span data-stu-id="446dc-110">Type</span></span>|<span data-ttu-id="446dc-111">Description</span><span class="sxs-lookup"><span data-stu-id="446dc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="446dc-112">lastCollectedDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="446dc-112">lastCollectedDateTimeUtc</span></span>|<span data-ttu-id="446dc-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="446dc-113">DateTimeOffset</span></span>|<span data-ttu-id="446dc-114">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="446dc-114">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="446dc-115">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="446dc-115">lastCollectedDateTime</span></span>|<span data-ttu-id="446dc-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="446dc-116">DateTimeOffset</span></span>|<span data-ttu-id="446dc-117">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="446dc-117">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="446dc-118">longitude</span><span class="sxs-lookup"><span data-stu-id="446dc-118">longitude</span></span>|<span data-ttu-id="446dc-119">Double</span><span class="sxs-lookup"><span data-stu-id="446dc-119">Double</span></span>|<span data-ttu-id="446dc-120">Долгота расположения устройства</span><span class="sxs-lookup"><span data-stu-id="446dc-120">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="446dc-121">latitude</span><span class="sxs-lookup"><span data-stu-id="446dc-121">latitude</span></span>|<span data-ttu-id="446dc-122">Double</span><span class="sxs-lookup"><span data-stu-id="446dc-122">Double</span></span>|<span data-ttu-id="446dc-123">Широта расположения устройства</span><span class="sxs-lookup"><span data-stu-id="446dc-123">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="446dc-124">altitude</span><span class="sxs-lookup"><span data-stu-id="446dc-124">altitude</span></span>|<span data-ttu-id="446dc-125">Double</span><span class="sxs-lookup"><span data-stu-id="446dc-125">Double</span></span>|<span data-ttu-id="446dc-126">Высота (метров над уровнем моря)</span><span class="sxs-lookup"><span data-stu-id="446dc-126">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="446dc-127">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="446dc-127">horizontalAccuracy</span></span>|<span data-ttu-id="446dc-128">Double</span><span class="sxs-lookup"><span data-stu-id="446dc-128">Double</span></span>|<span data-ttu-id="446dc-129">Точность долготы и широты (м)</span><span class="sxs-lookup"><span data-stu-id="446dc-129">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="446dc-130">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="446dc-130">verticalAccuracy</span></span>|<span data-ttu-id="446dc-131">Double</span><span class="sxs-lookup"><span data-stu-id="446dc-131">Double</span></span>|<span data-ttu-id="446dc-132">Точность высоты (м)</span><span class="sxs-lookup"><span data-stu-id="446dc-132">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="446dc-133">heading</span><span class="sxs-lookup"><span data-stu-id="446dc-133">heading</span></span>|<span data-ttu-id="446dc-134">Double</span><span class="sxs-lookup"><span data-stu-id="446dc-134">Double</span></span>|<span data-ttu-id="446dc-135">Направление от географического севера (градусов)</span><span class="sxs-lookup"><span data-stu-id="446dc-135">Heading in degrees from true north</span></span>|
|<span data-ttu-id="446dc-136">speed</span><span class="sxs-lookup"><span data-stu-id="446dc-136">speed</span></span>|<span data-ttu-id="446dc-137">Double</span><span class="sxs-lookup"><span data-stu-id="446dc-137">Double</span></span>|<span data-ttu-id="446dc-138">Скорость передвижения устройства (м/с)</span><span class="sxs-lookup"><span data-stu-id="446dc-138">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="446dc-139">Связи</span><span class="sxs-lookup"><span data-stu-id="446dc-139">Relationships</span></span>
<span data-ttu-id="446dc-140">Нет</span><span class="sxs-lookup"><span data-stu-id="446dc-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="446dc-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="446dc-141">JSON Representation</span></span>
<span data-ttu-id="446dc-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="446dc-142">Here is a JSON representation of the resource.</span></span>
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





