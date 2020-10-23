---
title: Тип ресурса Деливерйоптимизатионбандвидсхаурсвисперцентаже
description: Предельная пропускная способность в процентах с рабочими часами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7fb685f87e602eb6312d3e80e441b2c064ec327b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696232"
---
# <a name="deliveryoptimizationbandwidthhourswithpercentage-resource-type"></a><span data-ttu-id="19308-103">Тип ресурса Деливерйоптимизатионбандвидсхаурсвисперцентаже</span><span class="sxs-lookup"><span data-stu-id="19308-103">deliveryOptimizationBandwidthHoursWithPercentage resource type</span></span>

<span data-ttu-id="19308-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19308-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="19308-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19308-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19308-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="19308-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19308-107">Предельная пропускная способность в процентах с рабочими часами.</span><span class="sxs-lookup"><span data-stu-id="19308-107">Bandwidth limit as a percentage with business hours.</span></span>


<span data-ttu-id="19308-108">Наследуется от [деливерйоптимизатионбандвидс](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="19308-108">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="19308-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="19308-109">Properties</span></span>
|<span data-ttu-id="19308-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="19308-110">Property</span></span>|<span data-ttu-id="19308-111">Тип</span><span class="sxs-lookup"><span data-stu-id="19308-111">Type</span></span>|<span data-ttu-id="19308-112">Описание</span><span class="sxs-lookup"><span data-stu-id="19308-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19308-113">бандвидсбаккграундперцентажехаурс</span><span class="sxs-lookup"><span data-stu-id="19308-113">bandwidthBackgroundPercentageHours</span></span>|[<span data-ttu-id="19308-114">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="19308-114">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="19308-115">Процент загрузки в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="19308-115">Background download percentage hours.</span></span>|
|<span data-ttu-id="19308-116">бандвидсфореграундперцентажехаурс</span><span class="sxs-lookup"><span data-stu-id="19308-116">bandwidthForegroundPercentageHours</span></span>|[<span data-ttu-id="19308-117">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="19308-117">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="19308-118">Процентное соотношение загрузки в процентах.</span><span class="sxs-lookup"><span data-stu-id="19308-118">Foreground download percentage hours.</span></span>|

## <a name="relationships"></a><span data-ttu-id="19308-119">Связи</span><span class="sxs-lookup"><span data-stu-id="19308-119">Relationships</span></span>
<span data-ttu-id="19308-120">Нет</span><span class="sxs-lookup"><span data-stu-id="19308-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="19308-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="19308-121">JSON Representation</span></span>
<span data-ttu-id="19308-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19308-122">Here is a JSON representation of the resource.</span></span>
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





