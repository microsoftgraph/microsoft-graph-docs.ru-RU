---
title: Тип ресурса Деливерйоптимизатионмакскачесизеабсолуте
description: 'Максимальный размер кэша для оптимизации доставки: абсолютный тип.'
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a15b1bfea6da2af43c360ff143d8bb55bc44f6b6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420459"
---
# <a name="deliveryoptimizationmaxcachesizeabsolute-resource-type"></a><span data-ttu-id="b229c-103">Тип ресурса Деливерйоптимизатионмакскачесизеабсолуте</span><span class="sxs-lookup"><span data-stu-id="b229c-103">deliveryOptimizationMaxCacheSizeAbsolute resource type</span></span>

<span data-ttu-id="b229c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b229c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b229c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b229c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b229c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b229c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b229c-107">Максимальный размер кэша для оптимизации доставки: абсолютный тип.</span><span class="sxs-lookup"><span data-stu-id="b229c-107">Delivery Optimization max cache size absolute type.</span></span>


<span data-ttu-id="b229c-108">Наследуется от [деливерйоптимизатионмакскачесизе](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span><span class="sxs-lookup"><span data-stu-id="b229c-108">Inherits from [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b229c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="b229c-109">Properties</span></span>
|<span data-ttu-id="b229c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="b229c-110">Property</span></span>|<span data-ttu-id="b229c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="b229c-111">Type</span></span>|<span data-ttu-id="b229c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b229c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b229c-113">максимумкачесизеингигабитес</span><span class="sxs-lookup"><span data-stu-id="b229c-113">maximumCacheSizeInGigabytes</span></span>|<span data-ttu-id="b229c-114">Int64</span><span class="sxs-lookup"><span data-stu-id="b229c-114">Int64</span></span>|<span data-ttu-id="b229c-115">Задает максимальный размер кэша оптимизации доставки в ГБ.</span><span class="sxs-lookup"><span data-stu-id="b229c-115">Specifies the maximum size in GB of Delivery Optimization cache.</span></span> <span data-ttu-id="b229c-116">Допустимые значения — от 0 до 4294967295</span><span class="sxs-lookup"><span data-stu-id="b229c-116">Valid values 0 to 4294967295</span></span>
<span data-ttu-id="b229c-117">Значение 0 (ноль) означает "неограниченный" кэш.</span><span class="sxs-lookup"><span data-stu-id="b229c-117">The value 0 (zero) means "unlimited" cache.</span></span> <span data-ttu-id="b229c-118">При оптимизации доставки кэш очищается, когда на устройстве заканчивается свободное место на диске.</span><span class="sxs-lookup"><span data-stu-id="b229c-118">Delivery Optimization will clear the cache when the device is running low on disk space.</span></span> <span data-ttu-id="b229c-119">Допустимые значения — от 0 до 4294967295</span><span class="sxs-lookup"><span data-stu-id="b229c-119">Valid values 0 to 4294967295</span></span>|

## <a name="relationships"></a><span data-ttu-id="b229c-120">Связи</span><span class="sxs-lookup"><span data-stu-id="b229c-120">Relationships</span></span>
<span data-ttu-id="b229c-121">Нет</span><span class="sxs-lookup"><span data-stu-id="b229c-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b229c-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b229c-122">JSON Representation</span></span>
<span data-ttu-id="b229c-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b229c-123">Here is a JSON representation of the resource.</span></span>
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



