---
title: Тип ресурса Деливерйоптимизатионбандвидсперцентаже
description: Пределы проПускной способности, указанные в процентах.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7fb30ca54911723c619c8199ca32a9542772a6da
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177863"
---
# <a name="deliveryoptimizationbandwidthpercentage-resource-type"></a><span data-ttu-id="27caf-103">Тип ресурса Деливерйоптимизатионбандвидсперцентаже</span><span class="sxs-lookup"><span data-stu-id="27caf-103">deliveryOptimizationBandwidthPercentage resource type</span></span>

> <span data-ttu-id="27caf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27caf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27caf-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="27caf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27caf-106">Пределы проПускной способности, указанные в процентах.</span><span class="sxs-lookup"><span data-stu-id="27caf-106">Bandwidth limits specified as a percentage.</span></span>


<span data-ttu-id="27caf-107">НаСледуется от [деливерйоптимизатионбандвидс](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="27caf-107">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="27caf-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="27caf-108">Properties</span></span>
|<span data-ttu-id="27caf-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="27caf-109">Property</span></span>|<span data-ttu-id="27caf-110">Тип</span><span class="sxs-lookup"><span data-stu-id="27caf-110">Type</span></span>|<span data-ttu-id="27caf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="27caf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27caf-112">Максимумбаккграундбандвидсперцентаже</span><span class="sxs-lookup"><span data-stu-id="27caf-112">maximumBackgroundBandwidthPercentage</span></span>|<span data-ttu-id="27caf-113">Int32</span><span class="sxs-lookup"><span data-stu-id="27caf-113">Int32</span></span>|<span data-ttu-id="27caf-114">Указывает максимальную пропускную способность загрузки в фоновом режиме, которую оптимизация доставки использует для всех параллельных операций загрузки в процентах от доступной пропускной способности загрузки (0-100).</span><span class="sxs-lookup"><span data-stu-id="27caf-114">Specifies the maximum background download bandwidth that Delivery Optimization uses across all concurrent download activities as a percentage of available download bandwidth (0-100).</span></span> <span data-ttu-id="27caf-115">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="27caf-115">Valid values 0 to 100</span></span>
<span data-ttu-id="27caf-116">Значение по умолчанию 0 (ноль) означает, что оптимизация доставки динамически изменяется для использования доступной полосы пропускания для загрузки в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="27caf-116">The default value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for background downloads.</span></span> <span data-ttu-id="27caf-117">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="27caf-117">Valid values 0 to 100</span></span>|
|<span data-ttu-id="27caf-118">Максимумфореграундбандвидсперцентаже</span><span class="sxs-lookup"><span data-stu-id="27caf-118">maximumForegroundBandwidthPercentage</span></span>|<span data-ttu-id="27caf-119">Int32</span><span class="sxs-lookup"><span data-stu-id="27caf-119">Int32</span></span>|<span data-ttu-id="27caf-120">Указывает максимальную полосу пропускания при загрузке переднего плана, которую оптимизация доставки использует для всех параллельных операций загрузки в процентах от доступной пропускной способности загрузки (0-100).</span><span class="sxs-lookup"><span data-stu-id="27caf-120">Specifies the maximum foreground download bandwidth that Delivery Optimization uses across all concurrent download activities as a percentage of available download bandwidth (0-100).</span></span> <span data-ttu-id="27caf-121">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="27caf-121">Valid values 0 to 100</span></span>
<span data-ttu-id="27caf-122">Значение по умолчанию 0 (ноль) означает, что оптимизация доставки динамически изменяется, чтобы использовать доступную пропускную способность для загрузки в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="27caf-122">The default value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for foreground downloads.</span></span> <span data-ttu-id="27caf-123">Допустимые значения: от 0 до 100.</span><span class="sxs-lookup"><span data-stu-id="27caf-123">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="27caf-124">Связи</span><span class="sxs-lookup"><span data-stu-id="27caf-124">Relationships</span></span>
<span data-ttu-id="27caf-125">Нет</span><span class="sxs-lookup"><span data-stu-id="27caf-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="27caf-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="27caf-126">JSON Representation</span></span>
<span data-ttu-id="27caf-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27caf-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthPercentage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthPercentage",
  "maximumBackgroundBandwidthPercentage": 1024,
  "maximumForegroundBandwidthPercentage": 1024
}
```




