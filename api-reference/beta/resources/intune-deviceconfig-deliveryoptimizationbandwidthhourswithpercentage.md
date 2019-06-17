---
title: Тип ресурса Деливерйоптимизатионбандвидсхаурсвисперцентаже
description: Предельная пропускная способность в процентах с рабочими часами.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d1ad2bbfef3a055a4d5449f7f165bd4bf2f9a07a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979699"
---
# <a name="deliveryoptimizationbandwidthhourswithpercentage-resource-type"></a><span data-ttu-id="70aa5-103">Тип ресурса Деливерйоптимизатионбандвидсхаурсвисперцентаже</span><span class="sxs-lookup"><span data-stu-id="70aa5-103">deliveryOptimizationBandwidthHoursWithPercentage resource type</span></span>

> <span data-ttu-id="70aa5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70aa5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70aa5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="70aa5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70aa5-106">Предельная пропускная способность в процентах с рабочими часами.</span><span class="sxs-lookup"><span data-stu-id="70aa5-106">Bandwidth limit as a percentage with business hours.</span></span>


<span data-ttu-id="70aa5-107">Наследуется от [деливерйоптимизатионбандвидс](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="70aa5-107">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="70aa5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="70aa5-108">Properties</span></span>
|<span data-ttu-id="70aa5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="70aa5-109">Property</span></span>|<span data-ttu-id="70aa5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="70aa5-110">Type</span></span>|<span data-ttu-id="70aa5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="70aa5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70aa5-112">Бандвидсбаккграундперцентажехаурс</span><span class="sxs-lookup"><span data-stu-id="70aa5-112">bandwidthBackgroundPercentageHours</span></span>|[<span data-ttu-id="70aa5-113">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="70aa5-113">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="70aa5-114">Процент загрузки в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="70aa5-114">Background download percentage hours.</span></span>|
|<span data-ttu-id="70aa5-115">Бандвидсфореграундперцентажехаурс</span><span class="sxs-lookup"><span data-stu-id="70aa5-115">bandwidthForegroundPercentageHours</span></span>|[<span data-ttu-id="70aa5-116">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="70aa5-116">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="70aa5-117">Процентное соотношение загрузки в процентах.</span><span class="sxs-lookup"><span data-stu-id="70aa5-117">Foreground download percentage hours.</span></span>|

## <a name="relationships"></a><span data-ttu-id="70aa5-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="70aa5-118">Relationships</span></span>
<span data-ttu-id="70aa5-119">Нет</span><span class="sxs-lookup"><span data-stu-id="70aa5-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="70aa5-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="70aa5-120">JSON Representation</span></span>
<span data-ttu-id="70aa5-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="70aa5-121">Here is a JSON representation of the resource.</span></span>
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





