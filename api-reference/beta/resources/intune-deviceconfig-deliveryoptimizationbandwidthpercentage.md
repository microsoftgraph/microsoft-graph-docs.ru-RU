---
title: Тип ресурса Деливерйоптимизатионбандвидсперцентаже
description: Пределы пропускной способности, указанные в процентах.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 481e3f4c7b39d702302848424420902722021cdd
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420528"
---
# <a name="deliveryoptimizationbandwidthpercentage-resource-type"></a><span data-ttu-id="751bc-103">Тип ресурса Деливерйоптимизатионбандвидсперцентаже</span><span class="sxs-lookup"><span data-stu-id="751bc-103">deliveryOptimizationBandwidthPercentage resource type</span></span>

<span data-ttu-id="751bc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="751bc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="751bc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="751bc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="751bc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="751bc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="751bc-107">Пределы пропускной способности, указанные в процентах.</span><span class="sxs-lookup"><span data-stu-id="751bc-107">Bandwidth limits specified as a percentage.</span></span>


<span data-ttu-id="751bc-108">Наследуется от [деливерйоптимизатионбандвидс](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="751bc-108">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="751bc-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="751bc-109">Properties</span></span>
|<span data-ttu-id="751bc-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="751bc-110">Property</span></span>|<span data-ttu-id="751bc-111">Тип</span><span class="sxs-lookup"><span data-stu-id="751bc-111">Type</span></span>|<span data-ttu-id="751bc-112">Описание</span><span class="sxs-lookup"><span data-stu-id="751bc-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="751bc-113">максимумбаккграундбандвидсперцентаже</span><span class="sxs-lookup"><span data-stu-id="751bc-113">maximumBackgroundBandwidthPercentage</span></span>|<span data-ttu-id="751bc-114">Int32</span><span class="sxs-lookup"><span data-stu-id="751bc-114">Int32</span></span>|<span data-ttu-id="751bc-115">Указывает максимальную пропускную способность загрузки в фоновом режиме, которую оптимизация доставки использует для всех параллельных операций загрузки в процентах от доступной пропускной способности загрузки (0-100).</span><span class="sxs-lookup"><span data-stu-id="751bc-115">Specifies the maximum background download bandwidth that Delivery Optimization uses across all concurrent download activities as a percentage of available download bandwidth (0-100).</span></span> <span data-ttu-id="751bc-116">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="751bc-116">Valid values 0 to 100</span></span>
<span data-ttu-id="751bc-117">Значение по умолчанию 0 (ноль) означает, что оптимизация доставки динамически изменяется для использования доступной полосы пропускания для загрузки в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="751bc-117">The default value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for background downloads.</span></span> <span data-ttu-id="751bc-118">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="751bc-118">Valid values 0 to 100</span></span>|
|<span data-ttu-id="751bc-119">максимумфореграундбандвидсперцентаже</span><span class="sxs-lookup"><span data-stu-id="751bc-119">maximumForegroundBandwidthPercentage</span></span>|<span data-ttu-id="751bc-120">Int32</span><span class="sxs-lookup"><span data-stu-id="751bc-120">Int32</span></span>|<span data-ttu-id="751bc-121">Указывает максимальную полосу пропускания при загрузке переднего плана, которую оптимизация доставки использует для всех параллельных операций загрузки в процентах от доступной пропускной способности загрузки (0-100).</span><span class="sxs-lookup"><span data-stu-id="751bc-121">Specifies the maximum foreground download bandwidth that Delivery Optimization uses across all concurrent download activities as a percentage of available download bandwidth (0-100).</span></span> <span data-ttu-id="751bc-122">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="751bc-122">Valid values 0 to 100</span></span>
<span data-ttu-id="751bc-123">Значение по умолчанию 0 (ноль) означает, что оптимизация доставки динамически изменяется, чтобы использовать доступную пропускную способность для загрузки в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="751bc-123">The default value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for foreground downloads.</span></span> <span data-ttu-id="751bc-124">Допустимые значения: от 0 до 100.</span><span class="sxs-lookup"><span data-stu-id="751bc-124">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="751bc-125">Связи</span><span class="sxs-lookup"><span data-stu-id="751bc-125">Relationships</span></span>
<span data-ttu-id="751bc-126">Нет</span><span class="sxs-lookup"><span data-stu-id="751bc-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="751bc-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="751bc-127">JSON Representation</span></span>
<span data-ttu-id="751bc-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="751bc-128">Here is a JSON representation of the resource.</span></span>
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



