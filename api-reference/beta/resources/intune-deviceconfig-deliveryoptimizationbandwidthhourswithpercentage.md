---
title: Тип ресурса Деливерйоптимизатионбандвидсхаурсвисперцентаже
description: Предельная пропускная способность в процентах с рабочими часами.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 69656b0336dc09b2aa0a2f97cfe781347f5adc88
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333410"
---
# <a name="deliveryoptimizationbandwidthhourswithpercentage-resource-type"></a><span data-ttu-id="c2917-103">Тип ресурса Деливерйоптимизатионбандвидсхаурсвисперцентаже</span><span class="sxs-lookup"><span data-stu-id="c2917-103">deliveryOptimizationBandwidthHoursWithPercentage resource type</span></span>

> <span data-ttu-id="c2917-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2917-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2917-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2917-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2917-106">Предельная пропускная способность в процентах с рабочими часами.</span><span class="sxs-lookup"><span data-stu-id="c2917-106">Bandwidth limit as a percentage with business hours.</span></span>


<span data-ttu-id="c2917-107">Наследуется от [деливерйоптимизатионбандвидс](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="c2917-107">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c2917-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2917-108">Properties</span></span>
|<span data-ttu-id="c2917-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2917-109">Property</span></span>|<span data-ttu-id="c2917-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c2917-110">Type</span></span>|<span data-ttu-id="c2917-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c2917-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2917-112">бандвидсбаккграундперцентажехаурс</span><span class="sxs-lookup"><span data-stu-id="c2917-112">bandwidthBackgroundPercentageHours</span></span>|[<span data-ttu-id="c2917-113">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="c2917-113">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="c2917-114">Процент загрузки в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="c2917-114">Background download percentage hours.</span></span>|
|<span data-ttu-id="c2917-115">бандвидсфореграундперцентажехаурс</span><span class="sxs-lookup"><span data-stu-id="c2917-115">bandwidthForegroundPercentageHours</span></span>|[<span data-ttu-id="c2917-116">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="c2917-116">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="c2917-117">Процентное соотношение загрузки в процентах.</span><span class="sxs-lookup"><span data-stu-id="c2917-117">Foreground download percentage hours.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2917-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="c2917-118">Relationships</span></span>
<span data-ttu-id="c2917-119">Нет</span><span class="sxs-lookup"><span data-stu-id="c2917-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2917-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2917-120">JSON Representation</span></span>
<span data-ttu-id="c2917-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2917-121">Here is a JSON representation of the resource.</span></span>
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



