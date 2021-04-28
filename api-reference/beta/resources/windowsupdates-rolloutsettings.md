---
title: тип ресурса rolloutSettings
description: Параметры, как служба развертывает обновление со временем.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 705eeae189d9159c07d3c115c77383a207eae6db
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068076"
---
# <a name="rolloutsettings-resource-type"></a><span data-ttu-id="3d3b5-103">тип ресурса rolloutSettings</span><span class="sxs-lookup"><span data-stu-id="3d3b5-103">rolloutSettings resource type</span></span>

<span data-ttu-id="3d3b5-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="3d3b5-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d3b5-105">Параметры, как служба развертывает обновление со временем.</span><span class="sxs-lookup"><span data-stu-id="3d3b5-105">Settings controlling how the service deploys an update over time.</span></span>

## <a name="properties"></a><span data-ttu-id="3d3b5-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3d3b5-106">Properties</span></span>
|<span data-ttu-id="3d3b5-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d3b5-107">Property</span></span>|<span data-ttu-id="3d3b5-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3d3b5-108">Type</span></span>|<span data-ttu-id="3d3b5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3d3b5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d3b5-110">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3d3b5-110">startDateTime</span></span>|<span data-ttu-id="3d3b5-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d3b5-111">DateTimeOffset</span></span>|<span data-ttu-id="3d3b5-112">Дата, с которой устройства в развертывании начинают получать обновление.</span><span class="sxs-lookup"><span data-stu-id="3d3b5-112">Date on which devices in the deployment start receiving the update.</span></span> <span data-ttu-id="3d3b5-113">Если не установлено, развертывание начинается сразу после назначения устройств.</span><span class="sxs-lookup"><span data-stu-id="3d3b5-113">When not set, the deployment starts as soon as devices are assigned.</span></span>|
|<span data-ttu-id="3d3b5-114">devicesPerOffer</span><span class="sxs-lookup"><span data-stu-id="3d3b5-114">devicesPerOffer</span></span>|<span data-ttu-id="3d3b5-115">Int32</span><span class="sxs-lookup"><span data-stu-id="3d3b5-115">Int32</span></span>| <span data-ttu-id="3d3b5-116">Указывает количество устройств, предлагаемых одновременно.</span><span class="sxs-lookup"><span data-stu-id="3d3b5-116">Specifies the number of devices that are offered at the same time.</span></span> <span data-ttu-id="3d3b5-117">Не влияет при **наборе endDateTime.**</span><span class="sxs-lookup"><span data-stu-id="3d3b5-117">Has no effect when **endDateTime** is set.</span></span> <span data-ttu-id="3d3b5-118">Если **endDateTime и** **devicesPerOffer** не настроены, все устройства в развертывании одновременно предлагают контент.</span><span class="sxs-lookup"><span data-stu-id="3d3b5-118">When **endDateTime** and **devicesPerOffer** are both not set, all devices in the deployment are offered content at the same time.</span></span>|
|<span data-ttu-id="3d3b5-119">durationBetweenOffers</span><span class="sxs-lookup"><span data-stu-id="3d3b5-119">durationBetweenOffers</span></span>|<span data-ttu-id="3d3b5-120">String</span><span class="sxs-lookup"><span data-stu-id="3d3b5-120">String</span></span>|<span data-ttu-id="3d3b5-121">Указывает продолжительность между каждым набором устройств, которые предлагают обновление.</span><span class="sxs-lookup"><span data-stu-id="3d3b5-121">Specifies duration between each set of devices being offered the update.</span></span> <span data-ttu-id="3d3b5-122">Оказывает влияние при определении **endDateTime** или **devicesPerOffer.**</span><span class="sxs-lookup"><span data-stu-id="3d3b5-122">Has an effect when **endDateTime** or **devicesPerOffer** are defined.</span></span> <span data-ttu-id="3d3b5-123">Значение по умолчанию `P1D` (1 день).</span><span class="sxs-lookup"><span data-stu-id="3d3b5-123">Default value is `P1D` (1 day).</span></span>|
|<span data-ttu-id="3d3b5-124">endDateTime</span><span class="sxs-lookup"><span data-stu-id="3d3b5-124">endDateTime</span></span>|<span data-ttu-id="3d3b5-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d3b5-125">DateTimeOffset</span></span>|<span data-ttu-id="3d3b5-126">Указывает дату, до которой всем устройствам в развертывании предлагается обновление.</span><span class="sxs-lookup"><span data-stu-id="3d3b5-126">Specifies the date before which all devices currently in the deployment are offered the update.</span></span> <span data-ttu-id="3d3b5-127">Устройства, добавленные после этой даты, предлагаются немедленно.</span><span class="sxs-lookup"><span data-stu-id="3d3b5-127">Devices added after this date are offered immediately.</span></span> <span data-ttu-id="3d3b5-128">Если **endDateTime и** **devicesPerOffer** не настроены, все устройства в развертывании одновременно предлагают контент.</span><span class="sxs-lookup"><span data-stu-id="3d3b5-128">When **endDateTime** and **devicesPerOffer** are both not set, all devices in the deployment are offered content at the same time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d3b5-129">Связи</span><span class="sxs-lookup"><span data-stu-id="3d3b5-129">Relationships</span></span>
<span data-ttu-id="3d3b5-130">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3d3b5-130">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d3b5-131">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3d3b5-131">JSON representation</span></span>
<span data-ttu-id="3d3b5-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3d3b5-132">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.rolloutSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.rolloutSettings",
  "startDateTime": "String",
  "durationBetweenOffers": "String",
  "endDateTime": "String (timestamp)",
  "devicesPerOffer": "Integer"
}
```

