---
title: Тип ресурса Деливерйоптимизатионбандвидсперцентаже
description: Пределы пропускной способности, указанные в процентах.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3186e573b40cdaa4d56ace97a2ff985d7589db86
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696225"
---
# <a name="deliveryoptimizationbandwidthpercentage-resource-type"></a><span data-ttu-id="0e6cc-103">Тип ресурса Деливерйоптимизатионбандвидсперцентаже</span><span class="sxs-lookup"><span data-stu-id="0e6cc-103">deliveryOptimizationBandwidthPercentage resource type</span></span>

<span data-ttu-id="0e6cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e6cc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0e6cc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e6cc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e6cc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0e6cc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e6cc-107">Пределы пропускной способности, указанные в процентах.</span><span class="sxs-lookup"><span data-stu-id="0e6cc-107">Bandwidth limits specified as a percentage.</span></span>


<span data-ttu-id="0e6cc-108">Наследуется от [деливерйоптимизатионбандвидс](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span><span class="sxs-lookup"><span data-stu-id="0e6cc-108">Inherits from [deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0e6cc-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="0e6cc-109">Properties</span></span>
|<span data-ttu-id="0e6cc-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e6cc-110">Property</span></span>|<span data-ttu-id="0e6cc-111">Тип</span><span class="sxs-lookup"><span data-stu-id="0e6cc-111">Type</span></span>|<span data-ttu-id="0e6cc-112">Описание</span><span class="sxs-lookup"><span data-stu-id="0e6cc-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e6cc-113">максимумбаккграундбандвидсперцентаже</span><span class="sxs-lookup"><span data-stu-id="0e6cc-113">maximumBackgroundBandwidthPercentage</span></span>|<span data-ttu-id="0e6cc-114">Int32</span><span class="sxs-lookup"><span data-stu-id="0e6cc-114">Int32</span></span>|<span data-ttu-id="0e6cc-115">Указывает максимальную пропускную способность загрузки в фоновом режиме, которую оптимизация доставки использует для всех параллельных операций загрузки в процентах от доступной пропускной способности загрузки (0-100).</span><span class="sxs-lookup"><span data-stu-id="0e6cc-115">Specifies the maximum background download bandwidth that Delivery Optimization uses across all concurrent download activities as a percentage of available download bandwidth (0-100).</span></span> <span data-ttu-id="0e6cc-116">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="0e6cc-116">Valid values 0 to 100</span></span>
<span data-ttu-id="0e6cc-117">Значение по умолчанию 0 (ноль) означает, что оптимизация доставки динамически изменяется для использования доступной полосы пропускания для загрузки в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="0e6cc-117">The default value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for background downloads.</span></span> <span data-ttu-id="0e6cc-118">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="0e6cc-118">Valid values 0 to 100</span></span>|
|<span data-ttu-id="0e6cc-119">максимумфореграундбандвидсперцентаже</span><span class="sxs-lookup"><span data-stu-id="0e6cc-119">maximumForegroundBandwidthPercentage</span></span>|<span data-ttu-id="0e6cc-120">Int32</span><span class="sxs-lookup"><span data-stu-id="0e6cc-120">Int32</span></span>|<span data-ttu-id="0e6cc-121">Указывает максимальную полосу пропускания при загрузке переднего плана, которую оптимизация доставки использует для всех параллельных операций загрузки в процентах от доступной пропускной способности загрузки (0-100).</span><span class="sxs-lookup"><span data-stu-id="0e6cc-121">Specifies the maximum foreground download bandwidth that Delivery Optimization uses across all concurrent download activities as a percentage of available download bandwidth (0-100).</span></span> <span data-ttu-id="0e6cc-122">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="0e6cc-122">Valid values 0 to 100</span></span>
<span data-ttu-id="0e6cc-123">Значение по умолчанию 0 (ноль) означает, что оптимизация доставки динамически изменяется, чтобы использовать доступную пропускную способность для загрузки в фоновом режиме.</span><span class="sxs-lookup"><span data-stu-id="0e6cc-123">The default value 0 (zero) means that Delivery Optimization dynamically adjusts to use the available bandwidth for foreground downloads.</span></span> <span data-ttu-id="0e6cc-124">Допустимые значения: от 0 до 100.</span><span class="sxs-lookup"><span data-stu-id="0e6cc-124">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e6cc-125">Связи</span><span class="sxs-lookup"><span data-stu-id="0e6cc-125">Relationships</span></span>
<span data-ttu-id="0e6cc-126">Нет</span><span class="sxs-lookup"><span data-stu-id="0e6cc-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e6cc-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0e6cc-127">JSON Representation</span></span>
<span data-ttu-id="0e6cc-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0e6cc-128">Here is a JSON representation of the resource.</span></span>
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





