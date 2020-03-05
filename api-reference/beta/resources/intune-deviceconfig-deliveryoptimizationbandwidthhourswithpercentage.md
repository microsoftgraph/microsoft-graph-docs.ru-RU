---
title: Тип ресурса Деливерйоптимизатионбандвидсхаурсвисперцентаже
description: Предельная пропускная способность в процентах с рабочими часами.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dd7035bbd57e8deb5e80fdc4cfa770c559e30ef0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526806"
---
# <a name="deliveryoptimizationbandwidthhourswithpercentage-resource-type"></a><span data-ttu-id="1785f-103">Тип ресурса Деливерйоптимизатионбандвидсхаурсвисперцентаже</span><span class="sxs-lookup"><span data-stu-id="1785f-103">deliveryOptimizationBandwidthHoursWithPercentage resource type</span></span>

<span data-ttu-id="1785f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1785f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1785f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1785f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1785f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1785f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1785f-107">Предельная пропускная способность в процентах с рабочими часами.</span><span class="sxs-lookup"><span data-stu-id="1785f-107">Bandwidth limit as a percentage with business hours.</span></span>


<span data-ttu-id="1785f-108">Наследуется от [деливерйоптимизатионбандвидс](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="1785f-108">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1785f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="1785f-109">Properties</span></span>
|<span data-ttu-id="1785f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="1785f-110">Property</span></span>|<span data-ttu-id="1785f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="1785f-111">Type</span></span>|<span data-ttu-id="1785f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1785f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1785f-113">бандвидсбаккграундперцентажехаурс</span><span class="sxs-lookup"><span data-stu-id="1785f-113">bandwidthBackgroundPercentageHours</span></span>|[<span data-ttu-id="1785f-114">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="1785f-114">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="1785f-115">Процент загрузки в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="1785f-115">Background download percentage hours.</span></span>|
|<span data-ttu-id="1785f-116">бандвидсфореграундперцентажехаурс</span><span class="sxs-lookup"><span data-stu-id="1785f-116">bandwidthForegroundPercentageHours</span></span>|[<span data-ttu-id="1785f-117">deliveryOptimizationBandwidthBusinessHoursLimit</span><span class="sxs-lookup"><span data-stu-id="1785f-117">deliveryOptimizationBandwidthBusinessHoursLimit</span></span>](../resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit.md)|<span data-ttu-id="1785f-118">Процентное соотношение загрузки в процентах.</span><span class="sxs-lookup"><span data-stu-id="1785f-118">Foreground download percentage hours.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1785f-119">Связи</span><span class="sxs-lookup"><span data-stu-id="1785f-119">Relationships</span></span>
<span data-ttu-id="1785f-120">Нет</span><span class="sxs-lookup"><span data-stu-id="1785f-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1785f-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1785f-121">JSON Representation</span></span>
<span data-ttu-id="1785f-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1785f-122">Here is a JSON representation of the resource.</span></span>
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



