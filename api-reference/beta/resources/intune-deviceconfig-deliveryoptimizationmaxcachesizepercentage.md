---
title: Тип ресурса Деливерйоптимизатионмакскачесизеперцентаже
description: 'Оптимизация доставки: максимальный размер кэша типы в процентах.'
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6df7f0cdb84af15e9b4cea0856abcc75e7b2812c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48085152"
---
# <a name="deliveryoptimizationmaxcachesizepercentage-resource-type"></a><span data-ttu-id="a16f4-103">Тип ресурса Деливерйоптимизатионмакскачесизеперцентаже</span><span class="sxs-lookup"><span data-stu-id="a16f4-103">deliveryOptimizationMaxCacheSizePercentage resource type</span></span>

<span data-ttu-id="a16f4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a16f4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a16f4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a16f4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a16f4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a16f4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a16f4-107">Оптимизация доставки: максимальный размер кэша типы в процентах.</span><span class="sxs-lookup"><span data-stu-id="a16f4-107">Delivery Optimization Max cache size percentage types.</span></span>


<span data-ttu-id="a16f4-108">Наследуется от [деливерйоптимизатионмакскачесизе](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span><span class="sxs-lookup"><span data-stu-id="a16f4-108">Inherits from [deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a16f4-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="a16f4-109">Properties</span></span>
|<span data-ttu-id="a16f4-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="a16f4-110">Property</span></span>|<span data-ttu-id="a16f4-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a16f4-111">Type</span></span>|<span data-ttu-id="a16f4-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a16f4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a16f4-113">максимумкачесизеперцентаже</span><span class="sxs-lookup"><span data-stu-id="a16f4-113">maximumCacheSizePercentage</span></span>|<span data-ttu-id="a16f4-114">Int32</span><span class="sxs-lookup"><span data-stu-id="a16f4-114">Int32</span></span>|<span data-ttu-id="a16f4-115">Задает максимальный размер кэша, который может использовать оптимизация доставки, в процентах от размера диска (1-100).</span><span class="sxs-lookup"><span data-stu-id="a16f4-115">Specifies the maximum cache size that Delivery Optimization can utilize, as a percentage of disk size (1-100).</span></span> <span data-ttu-id="a16f4-116">Допустимые значения — от 1 до 100</span><span class="sxs-lookup"><span data-stu-id="a16f4-116">Valid values 1 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="a16f4-117">Связи</span><span class="sxs-lookup"><span data-stu-id="a16f4-117">Relationships</span></span>
<span data-ttu-id="a16f4-118">Нет</span><span class="sxs-lookup"><span data-stu-id="a16f4-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a16f4-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a16f4-119">JSON Representation</span></span>
<span data-ttu-id="a16f4-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a16f4-120">Here is a JSON representation of the resource.</span></span>
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






