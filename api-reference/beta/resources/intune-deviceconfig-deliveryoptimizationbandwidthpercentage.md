---
title: Тип ресурса Деливерйоптимизатионбандвидсперцентаже
description: Пределы пропускной способности, указанные в процентах.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c4179dad06705f0ec1ba3f2dc9ea87ad44f4948c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081561"
---
# <a name="deliveryoptimizationbandwidthpercentage-resource-type"></a><span data-ttu-id="403ed-103">Тип ресурса Деливерйоптимизатионбандвидсперцентаже</span><span class="sxs-lookup"><span data-stu-id="403ed-103">deliveryOptimizationBandwidthPercentage resource type</span></span>

<span data-ttu-id="403ed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="403ed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="403ed-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="403ed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="403ed-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="403ed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="403ed-107">Пределы пропускной способности, указанные в процентах.</span><span class="sxs-lookup"><span data-stu-id="403ed-107">Bandwidth limits specified as a percentage.</span></span>


<span data-ttu-id="403ed-108">Наследуется от [деливерйоптимизатионбандвидс](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="403ed-108">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="403ed-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="403ed-109">Properties</span></span>
|<span data-ttu-id="403ed-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="403ed-110">Property</span></span>|<span data-ttu-id="403ed-111">Тип</span><span class="sxs-lookup"><span data-stu-id="403ed-111">Type</span></span>|<span data-ttu-id="403ed-112">Описание</span><span class="sxs-lookup"><span data-stu-id="403ed-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="403ed-113">максимумбаккграундбандвидсперцентаже</span><span class="sxs-lookup"><span data-stu-id="403ed-113">maximumBackgroundBandwidthPercentage</span></span>|<span data-ttu-id="403ed-114">Int32</span><span class="sxs-lookup"><span data-stu-id="403ed-114">Int32</span></span>|<span data-ttu-id="403ed-115">Указывает максимальную пропускную способность загрузки в фоновом режиме, которую оптимизация доставки использует для всех параллельных операций загрузки в процентах от доступной пропускной способности загрузки (0-100).</span><span class="sxs-lookup"><span data-stu-id="403ed-115">Specifies the maximum background download bandwidth that Delivery Optimization uses across all concurrent download activities as a percentage of available download bandwidth (0-100).</span></span> <span data-ttu-id="403ed-116">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="403ed-116">Valid values 0 to 100</span></span>
<span data-ttu-id="403ed-117">Значение по умолчанию 0 (ноль) означает, что оптимизация доставки динамически изменяется для использования доступной полосы пропускания для загрузки в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="403ed-117">The default value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for background downloads.</span></span> <span data-ttu-id="403ed-118">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="403ed-118">Valid values 0 to 100</span></span>|
|<span data-ttu-id="403ed-119">максимумфореграундбандвидсперцентаже</span><span class="sxs-lookup"><span data-stu-id="403ed-119">maximumForegroundBandwidthPercentage</span></span>|<span data-ttu-id="403ed-120">Int32</span><span class="sxs-lookup"><span data-stu-id="403ed-120">Int32</span></span>|<span data-ttu-id="403ed-121">Указывает максимальную полосу пропускания при загрузке переднего плана, которую оптимизация доставки использует для всех параллельных операций загрузки в процентах от доступной пропускной способности загрузки (0-100).</span><span class="sxs-lookup"><span data-stu-id="403ed-121">Specifies the maximum foreground download bandwidth that Delivery Optimization uses across all concurrent download activities as a percentage of available download bandwidth (0-100).</span></span> <span data-ttu-id="403ed-122">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="403ed-122">Valid values 0 to 100</span></span>
<span data-ttu-id="403ed-123">Значение по умолчанию 0 (ноль) означает, что оптимизация доставки динамически изменяется, чтобы использовать доступную пропускную способность для загрузки в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="403ed-123">The default value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for foreground downloads.</span></span> <span data-ttu-id="403ed-124">Допустимые значения: от 0 до 100.</span><span class="sxs-lookup"><span data-stu-id="403ed-124">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="403ed-125">Связи</span><span class="sxs-lookup"><span data-stu-id="403ed-125">Relationships</span></span>
<span data-ttu-id="403ed-126">Нет</span><span class="sxs-lookup"><span data-stu-id="403ed-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="403ed-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="403ed-127">JSON Representation</span></span>
<span data-ttu-id="403ed-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="403ed-128">Here is a JSON representation of the resource.</span></span>
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






