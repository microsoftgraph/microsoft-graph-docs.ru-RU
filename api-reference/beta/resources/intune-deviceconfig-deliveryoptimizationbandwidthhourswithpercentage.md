---
title: Тип ресурса Деливерйоптимизатионбандвидсхаурсвисперцентаже
description: Предельная пропускная способность в процентах с рабочими часами.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 85008f7aee3c2f06536ef838df04e56ede36ed46
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420583"
---
# <a name="deliveryoptimizationbandwidthhourswithpercentage-resource-type"></a><span data-ttu-id="9fcb7-103">Тип ресурса Деливерйоптимизатионбандвидсхаурсвисперцентаже</span><span class="sxs-lookup"><span data-stu-id="9fcb7-103">deliveryOptimizationBandwidthHoursWithPercentage resource type</span></span>

<span data-ttu-id="9fcb7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fcb7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9fcb7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fcb7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9fcb7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9fcb7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fcb7-107">Предельная пропускная способность в процентах с рабочими часами.</span><span class="sxs-lookup"><span data-stu-id="9fcb7-107">Bandwidth limit as a percentage with business hours.</span></span>


<span data-ttu-id="9fcb7-108">Наследуется от [деливерйоптимизатионбандвидс](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="9fcb7-108">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9fcb7-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="9fcb7-109">Properties</span></span>
|<span data-ttu-id="9fcb7-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="9fcb7-110">Property</span></span>|<span data-ttu-id="9fcb7-111">Тип</span><span class="sxs-lookup"><span data-stu-id="9fcb7-111">Type</span></span>|<span data-ttu-id="9fcb7-112">Описание</span><span class="sxs-lookup"><span data-stu-id="9fcb7-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fcb7-113">бандвидсбаккграундперцентажехаурс</span><span class="sxs-lookup"><span data-stu-id="9fcb7-113">bandwidthBackgroundPercentageHours</span></span>|[<span data-ttu-id="9fcb7-114">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="9fcb7-114">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="9fcb7-115">Процент загрузки в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="9fcb7-115">Background download percentage hours.</span></span>|
|<span data-ttu-id="9fcb7-116">бандвидсфореграундперцентажехаурс</span><span class="sxs-lookup"><span data-stu-id="9fcb7-116">bandwidthForegroundPercentageHours</span></span>|[<span data-ttu-id="9fcb7-117">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="9fcb7-117">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="9fcb7-118">Процентное соотношение загрузки в процентах.</span><span class="sxs-lookup"><span data-stu-id="9fcb7-118">Foreground download percentage hours.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9fcb7-119">Связи</span><span class="sxs-lookup"><span data-stu-id="9fcb7-119">Relationships</span></span>
<span data-ttu-id="9fcb7-120">Нет</span><span class="sxs-lookup"><span data-stu-id="9fcb7-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9fcb7-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9fcb7-121">JSON Representation</span></span>
<span data-ttu-id="9fcb7-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9fcb7-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthHoursWithPercentage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthHoursWithPercentage",
  "bandwidthBackgroundPercentageHours": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit",
    "bandwidthBeginBusinessHours": 1024,
    "bandwidthEndBusinessHours": 1024,
    "bandwidthPercentageDuringBusinessHours": 1024,
    "bandwidthPercentageOutsideBusinessHours": 1024
  },
  "bandwidthForegroundPercentageHours": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit",
    "bandwidthBeginBusinessHours": 1024,
    "bandwidthEndBusinessHours": 1024,
    "bandwidthPercentageDuringBusinessHours": 1024,
    "bandwidthPercentageOutsideBusinessHours": 1024
  }
}
```



