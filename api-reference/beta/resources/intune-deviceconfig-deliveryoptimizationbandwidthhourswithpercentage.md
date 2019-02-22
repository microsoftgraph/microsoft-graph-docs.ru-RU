---
title: Тип ресурса Деливерйоптимизатионбандвидсхаурсвисперцентаже
description: Предельная проПускная способность в процентах с рабочими часами.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7fb4fa251e9f1cb936da0ada158050df42e0aab6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30178243"
---
# <a name="deliveryoptimizationbandwidthhourswithpercentage-resource-type"></a><span data-ttu-id="0955d-103">Тип ресурса Деливерйоптимизатионбандвидсхаурсвисперцентаже</span><span class="sxs-lookup"><span data-stu-id="0955d-103">deliveryOptimizationBandwidthHoursWithPercentage resource type</span></span>

> <span data-ttu-id="0955d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0955d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0955d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0955d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0955d-106">Предельная проПускная способность в процентах с рабочими часами.</span><span class="sxs-lookup"><span data-stu-id="0955d-106">Bandwidth limit as a percentage with business hours.</span></span>


<span data-ttu-id="0955d-107">НаСледуется от [деливерйоптимизатионбандвидс](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="0955d-107">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0955d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0955d-108">Properties</span></span>
|<span data-ttu-id="0955d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0955d-109">Property</span></span>|<span data-ttu-id="0955d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0955d-110">Type</span></span>|<span data-ttu-id="0955d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0955d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0955d-112">Бандвидсбаккграундперцентажехаурс</span><span class="sxs-lookup"><span data-stu-id="0955d-112">bandwidthBackgroundPercentageHours</span></span>|[<span data-ttu-id="0955d-113">Деливерйоптимизатионбандвидсбусинесшаурслимит</span><span class="sxs-lookup"><span data-stu-id="0955d-113">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="0955d-114">Процент загрузки в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="0955d-114">Background download percentage hours.</span></span>|
|<span data-ttu-id="0955d-115">Бандвидсфореграундперцентажехаурс</span><span class="sxs-lookup"><span data-stu-id="0955d-115">bandwidthForegroundPercentageHours</span></span>|[<span data-ttu-id="0955d-116">Деливерйоптимизатионбандвидсбусинесшаурслимит</span><span class="sxs-lookup"><span data-stu-id="0955d-116">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="0955d-117">Процентное соотношение загрузки в процентах.</span><span class="sxs-lookup"><span data-stu-id="0955d-117">Foreground download percentage hours.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0955d-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="0955d-118">Relationships</span></span>
<span data-ttu-id="0955d-119">Нет</span><span class="sxs-lookup"><span data-stu-id="0955d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0955d-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0955d-120">JSON Representation</span></span>
<span data-ttu-id="0955d-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0955d-121">Here is a JSON representation of the resource.</span></span>
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




