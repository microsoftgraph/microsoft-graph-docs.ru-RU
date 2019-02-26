---
title: Тип ресурса Деливерйоптимизатионмакскачесизеперцентаже
description: 'Оптимизация доставки: максимальный размер кэша типы в процентах.'
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7579b95d0adefb09c9312596f4604fe9d5b05548
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177835"
---
# <a name="deliveryoptimizationmaxcachesizepercentage-resource-type"></a><span data-ttu-id="92bb6-103">Тип ресурса Деливерйоптимизатионмакскачесизеперцентаже</span><span class="sxs-lookup"><span data-stu-id="92bb6-103">deliveryOptimizationMaxCacheSizePercentage resource type</span></span>

> <span data-ttu-id="92bb6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92bb6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92bb6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="92bb6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92bb6-106">Оптимизация доставки: максимальный размер кэша типы в процентах.</span><span class="sxs-lookup"><span data-stu-id="92bb6-106">Delivery Optimization Max cache size percentage types.</span></span>


<span data-ttu-id="92bb6-107">НаСледуется от [деливерйоптимизатионмакскачесизе](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span><span class="sxs-lookup"><span data-stu-id="92bb6-107">Inherits from [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span></span>

## <a name="properties"></a><span data-ttu-id="92bb6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="92bb6-108">Properties</span></span>
|<span data-ttu-id="92bb6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="92bb6-109">Property</span></span>|<span data-ttu-id="92bb6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="92bb6-110">Type</span></span>|<span data-ttu-id="92bb6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="92bb6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92bb6-112">Максимумкачесизеперцентаже</span><span class="sxs-lookup"><span data-stu-id="92bb6-112">maximumCacheSizePercentage</span></span>|<span data-ttu-id="92bb6-113">Int32</span><span class="sxs-lookup"><span data-stu-id="92bb6-113">Int32</span></span>|<span data-ttu-id="92bb6-114">Задает максимальный размер кэша, который может использовать оптимизация доставки, в процентах от размера диска (1-100).</span><span class="sxs-lookup"><span data-stu-id="92bb6-114">Specifies the maximum cache size that Delivery Optimization can utilize, as a percentage of disk size (1-100).</span></span> <span data-ttu-id="92bb6-115">Допустимые значения — от 1 до 100</span><span class="sxs-lookup"><span data-stu-id="92bb6-115">Valid values 1 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="92bb6-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="92bb6-116">Relationships</span></span>
<span data-ttu-id="92bb6-117">Нет</span><span class="sxs-lookup"><span data-stu-id="92bb6-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="92bb6-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="92bb6-118">JSON Representation</span></span>
<span data-ttu-id="92bb6-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92bb6-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSizePercentage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationMaxCacheSizePercentage",
  "maximumCacheSizePercentage": 1024
}
```




