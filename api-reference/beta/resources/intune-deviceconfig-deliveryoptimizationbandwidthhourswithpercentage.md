---
title: Тип ресурса Деливерйоптимизатионбандвидсхаурсвисперцентаже
description: Предельная проПускная способность в процентах с рабочими часами.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ecb024d15ee5d4e748d57e1b895c9418feadd52a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31802739"
---
# <a name="deliveryoptimizationbandwidthhourswithpercentage-resource-type"></a><span data-ttu-id="6c07b-103">Тип ресурса Деливерйоптимизатионбандвидсхаурсвисперцентаже</span><span class="sxs-lookup"><span data-stu-id="6c07b-103">deliveryOptimizationBandwidthHoursWithPercentage resource type</span></span>

> <span data-ttu-id="6c07b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c07b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c07b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6c07b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c07b-106">Предельная проПускная способность в процентах с рабочими часами.</span><span class="sxs-lookup"><span data-stu-id="6c07b-106">Bandwidth limit as a percentage with business hours.</span></span>


<span data-ttu-id="6c07b-107">НаСледуется от [деливерйоптимизатионбандвидс](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="6c07b-107">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6c07b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6c07b-108">Properties</span></span>
|<span data-ttu-id="6c07b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c07b-109">Property</span></span>|<span data-ttu-id="6c07b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6c07b-110">Type</span></span>|<span data-ttu-id="6c07b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6c07b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c07b-112">Бандвидсбаккграундперцентажехаурс</span><span class="sxs-lookup"><span data-stu-id="6c07b-112">bandwidthBackgroundPercentageHours</span></span>|[<span data-ttu-id="6c07b-113">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="6c07b-113">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="6c07b-114">Процент загрузки в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="6c07b-114">Background download percentage hours.</span></span>|
|<span data-ttu-id="6c07b-115">Бандвидсфореграундперцентажехаурс</span><span class="sxs-lookup"><span data-stu-id="6c07b-115">bandwidthForegroundPercentageHours</span></span>|[<span data-ttu-id="6c07b-116">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="6c07b-116">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="6c07b-117">Процентное соотношение загрузки в процентах.</span><span class="sxs-lookup"><span data-stu-id="6c07b-117">Foreground download percentage hours.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c07b-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="6c07b-118">Relationships</span></span>
<span data-ttu-id="6c07b-119">Нет</span><span class="sxs-lookup"><span data-stu-id="6c07b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c07b-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6c07b-120">JSON Representation</span></span>
<span data-ttu-id="6c07b-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6c07b-121">Here is a JSON representation of the resource.</span></span>
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





