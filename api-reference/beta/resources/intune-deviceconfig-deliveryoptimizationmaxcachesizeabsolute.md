---
title: Тип ресурса Деливерйоптимизатионмакскачесизеабсолуте
description: 'Максимальный размер кэша для оптимизации доставки: абсолютный тип.'
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bfeb2e4279e9858f9fd8f923657c8e32bf129396
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979587"
---
# <a name="deliveryoptimizationmaxcachesizeabsolute-resource-type"></a><span data-ttu-id="91dd4-103">Тип ресурса Деливерйоптимизатионмакскачесизеабсолуте</span><span class="sxs-lookup"><span data-stu-id="91dd4-103">deliveryOptimizationMaxCacheSizeAbsolute resource type</span></span>

> <span data-ttu-id="91dd4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91dd4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91dd4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="91dd4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91dd4-106">Максимальный размер кэша для оптимизации доставки: абсолютный тип.</span><span class="sxs-lookup"><span data-stu-id="91dd4-106">Delivery Optimization max cache size absolute type.</span></span>


<span data-ttu-id="91dd4-107">Наследуется от [деливерйоптимизатионмакскачесизе](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span><span class="sxs-lookup"><span data-stu-id="91dd4-107">Inherits from [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span></span>

## <a name="properties"></a><span data-ttu-id="91dd4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="91dd4-108">Properties</span></span>
|<span data-ttu-id="91dd4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="91dd4-109">Property</span></span>|<span data-ttu-id="91dd4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="91dd4-110">Type</span></span>|<span data-ttu-id="91dd4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="91dd4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91dd4-112">Максимумкачесизеингигабитес</span><span class="sxs-lookup"><span data-stu-id="91dd4-112">maximumCacheSizeInGigabytes</span></span>|<span data-ttu-id="91dd4-113">Int64</span><span class="sxs-lookup"><span data-stu-id="91dd4-113">Int64</span></span>|<span data-ttu-id="91dd4-114">Задает максимальный размер кэша оптимизации доставки в ГБ.</span><span class="sxs-lookup"><span data-stu-id="91dd4-114">Specifies the maximum size in GB of Delivery Optimization cache.</span></span> <span data-ttu-id="91dd4-115">Допустимые значения — от 0 до 4294967295</span><span class="sxs-lookup"><span data-stu-id="91dd4-115">Valid values 0 to 4294967295</span></span>
<span data-ttu-id="91dd4-116">Значение 0 (ноль) означает "неограниченный" кэш.</span><span class="sxs-lookup"><span data-stu-id="91dd4-116">The value 0 (zero) means "unlimited" cache.</span></span> <span data-ttu-id="91dd4-117">При оптимизации доставки кэш очищается, когда на устройстве заканчивается свободное место на диске.</span><span class="sxs-lookup"><span data-stu-id="91dd4-117">Delivery Optimization will clear the cache when the device is running low on disk space.</span></span> <span data-ttu-id="91dd4-118">Допустимые значения — от 0 до 4294967295</span><span class="sxs-lookup"><span data-stu-id="91dd4-118">Valid values 0 to 4294967295</span></span>|

## <a name="relationships"></a><span data-ttu-id="91dd4-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="91dd4-119">Relationships</span></span>
<span data-ttu-id="91dd4-120">Нет</span><span class="sxs-lookup"><span data-stu-id="91dd4-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="91dd4-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="91dd4-121">JSON Representation</span></span>
<span data-ttu-id="91dd4-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="91dd4-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSizeAbsolute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationMaxCacheSizeAbsolute",
  "maximumCacheSizeInGigabytes": 1024
}
```





