---
title: Тип ресурса Деливерйоптимизатионмакскачесизеабсолуте
description: 'Максимальный размер кэша для оптимизации доставки: абсолютный тип.'
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 182ae08fba3081cfda2ca645efc384983cfca4c3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42793396"
---
# <a name="deliveryoptimizationmaxcachesizeabsolute-resource-type"></a><span data-ttu-id="8040f-103">Тип ресурса Деливерйоптимизатионмакскачесизеабсолуте</span><span class="sxs-lookup"><span data-stu-id="8040f-103">deliveryOptimizationMaxCacheSizeAbsolute resource type</span></span>

> <span data-ttu-id="8040f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8040f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8040f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8040f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8040f-106">Максимальный размер кэша для оптимизации доставки: абсолютный тип.</span><span class="sxs-lookup"><span data-stu-id="8040f-106">Delivery Optimization max cache size absolute type.</span></span>


<span data-ttu-id="8040f-107">Наследуется от [деливерйоптимизатионмакскачесизе](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span><span class="sxs-lookup"><span data-stu-id="8040f-107">Inherits from [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8040f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8040f-108">Properties</span></span>
|<span data-ttu-id="8040f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8040f-109">Property</span></span>|<span data-ttu-id="8040f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8040f-110">Type</span></span>|<span data-ttu-id="8040f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8040f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8040f-112">максимумкачесизеингигабитес</span><span class="sxs-lookup"><span data-stu-id="8040f-112">maximumCacheSizeInGigabytes</span></span>|<span data-ttu-id="8040f-113">Int64</span><span class="sxs-lookup"><span data-stu-id="8040f-113">Int64</span></span>|<span data-ttu-id="8040f-114">Задает максимальный размер кэша оптимизации доставки в ГБ.</span><span class="sxs-lookup"><span data-stu-id="8040f-114">Specifies the maximum size in GB of Delivery Optimization cache.</span></span> <span data-ttu-id="8040f-115">Допустимые значения — от 0 до 4294967295</span><span class="sxs-lookup"><span data-stu-id="8040f-115">Valid values 0 to 4294967295</span></span>
<span data-ttu-id="8040f-116">Значение 0 (ноль) означает "неограниченный" кэш.</span><span class="sxs-lookup"><span data-stu-id="8040f-116">The value 0 (zero) means "unlimited" cache.</span></span> <span data-ttu-id="8040f-117">При оптимизации доставки кэш очищается, когда на устройстве заканчивается свободное место на диске.</span><span class="sxs-lookup"><span data-stu-id="8040f-117">Delivery Optimization will clear the cache when the device is running low on disk space.</span></span> <span data-ttu-id="8040f-118">Допустимые значения — от 0 до 4294967295</span><span class="sxs-lookup"><span data-stu-id="8040f-118">Valid values 0 to 4294967295</span></span>|

## <a name="relationships"></a><span data-ttu-id="8040f-119">Связи</span><span class="sxs-lookup"><span data-stu-id="8040f-119">Relationships</span></span>
<span data-ttu-id="8040f-120">Нет</span><span class="sxs-lookup"><span data-stu-id="8040f-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8040f-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8040f-121">JSON Representation</span></span>
<span data-ttu-id="8040f-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8040f-122">Here is a JSON representation of the resource.</span></span>
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



